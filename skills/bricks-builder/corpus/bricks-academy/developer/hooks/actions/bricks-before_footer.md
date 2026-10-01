---
title: "Action: bricks_before_footer"
description: "Runs before Bricks renders the footer template."
canonical: "https://academy.bricksbuilder.io/developer/hooks/actions/bricks-before_footer/"
markdownUrl: "https://academy.bricksbuilder.io/developer/hooks/actions/bricks-before_footer.md"
pageType: "article"
section: "developer"
category: "hooks"
lastmod: "2026-09-30T17:19:56.000Z"
---
Runs before Bricks renders the footer template. Use it to output markup or run logic immediately before footer rendering.

## Example usage

```php
add_action( 'bricks_before_footer', function() {
    echo '<div class="before-footer-cta">Need help?</div>';
} );
```
