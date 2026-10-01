---
title: "Filter: bricks/media_browser/health/file_status"
description: "Report the file status of offloaded attachments to Bricks Media Health without treating a missing local copy as a broken file."
canonical: "https://academy.bricksbuilder.io/developer/hooks/filters/bricks-media-browser-health-file-status/"
markdownUrl: "https://academy.bricksbuilder.io/developer/hooks/filters/bricks-media-browser-health-file-status.md"
pageType: "article"
section: "developer"
category: "hooks"
lastmod: "2026-09-30T17:19:56.000Z"
---
Bricks 2.4 uses `bricks/media_browser/health/file_status` to let media integrations override the original attachment's file status in Media Health.

By default, Bricks checks the attached file on the local filesystem. An offload integration can return a status based on its own storage records when the local copy has been removed.

## Parameters

| Parameter | Type | Description |
| --- | --- | --- |
| `$state` | string | Status detected by Bricks before this filter runs. |
| `$attachment_id` | int | WordPress attachment ID. |
| `$file` | string or false | Attached file path returned by `get_attached_file()`. |
| `$url` | string or false | Attachment URL returned by `wp_get_attachment_url()`. |

Register the callback with four accepted arguments. Return one of these strings:

| Return value | Meaning | Broken-file check |
| --- | --- | --- |
| `exists` | The original file is available. | Does not flag the original as broken. |
| `missing` | The original file is absent. | Flags it as broken. |
| `unreadable` | The original file cannot be read. | Flags it as broken. |
| `empty` | The original file has no content. | Flags it as broken. |
| `unknown` | The integration cannot determine availability. | Does not flag the original as broken. |

The broken-file check must be enabled for those issues to be reported. Bricks sanitizes the returned value and treats unsupported values as `unknown`. An `unknown` result is not confirmation that the file is healthy.

## Example: use a provider's stored status

Add the filter in your integration plugin. This example assumes your own offload process records a verified status in an attachment meta field named `_my_offload_file_state`. Replace that field and lookup with your provider's actual status source. Bricks does not create or refresh this metadata.

```php
add_filter( 'bricks/media_browser/health/file_status', function( $state, $attachment_id, $file, $url ) {
    $provider_state = get_post_meta( $attachment_id, '_my_offload_file_state', true );

    // Leave attachments outside this integration unchanged.
    if ( $provider_state === '' ) {
        return $state;
    }

    $allowed = [ 'exists', 'missing', 'unreadable', 'empty', 'unknown' ];

    return in_array( $provider_state, $allowed, true ) ? $provider_state : 'unknown';
}, 10, 4 );
```

Only return `exists` when the provider has confirmed that the remote original is available. An attachment URL alone does not prove the file exists. Keep stored results current when files are uploaded, removed, or moved; avoid a separate remote request for every attachment during a scan.

## Scope and repair limits

The filter changes classification of the original file. It does not download offloaded media, supply a remote file size, or make local repair actions work on remote files.

Image-size checks can still inspect local derivative files. Operations such as image regeneration and optimization require a readable local source within the uploads directory. Restore a local copy through your offload integration before attempting repairs that require it.
