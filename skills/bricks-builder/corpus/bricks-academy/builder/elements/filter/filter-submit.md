---
title: "Filter submit"
description: "Creates submit/reset buttons for filter forms. Provides control over when filters are applied - either as a submit button to apply all filters at once, or as a."
canonical: "https://academy.bricksbuilder.io/builder/elements/filter/filter-submit/"
markdownUrl: "https://academy.bricksbuilder.io/builder/elements/filter/filter-submit.md"
pageType: "article"
section: "builder"
category: "elements"
lastmod: "2026-09-16T10:41:20.000Z"
---
Creates submit/reset buttons for filter forms. Provides control over when filters are applied - either as a submit button to apply all filters at once, or as a reset button to clear all active filters. Supports redirection to specific URLs after submission.

## Settings

- **Target query** (query-list) - Select the query this filter should target. Only post queries are supported in this version.
- **Action** (select) - Button behavior. Options: Submit (apply filters), Reset (clear filters).
- **Redirect to** (text) - URL to redirect to after applying filters (Submit action only).
- **Open in new tab** (checkbox) - Open redirect URL in new tab (Submit action only).
- **Exclude filter IDs** (text, Bricks 2.4) - Comma-separated Bricks element IDs of filters to preserve when resetting (Reset action only).
- **Hide if no active filter** (checkbox) - Hide the reset button when no filters it can reset are active. Excluded filters do not keep the button visible. Adds .brx-no-active-filter class for styling (Reset action only).
- **Button** - Settings for the submit/reset button.
  - **Text** (text) - Button text. Default: Filter.
  - **Size** (select) - Button size preset. Options: Default, Small, Medium, Large, Extra Large.
  - **Style** (select) - Button style. Options: None, Primary, Secondary, Success, Info, Warning, Danger, Dark, Light. Default: Primary.
  - **Circle** (checkbox) - Make button circular.
  - **Outline** (checkbox) - Use outline button style.
  - **Icon** (icon) - Icon to display on the button.
  - **Icon color** (color) - Color of the button icon.
  - **Icon size** (number) - Size of the button icon.

## Preserve a search while resetting refinements

Set **Action** to **Reset**, then enter the Search filter's Bricks element ID in **Exclude filter IDs**. For example, enter `q1w2e3,mn9456` to preserve two filters. Use the filter elements' IDs, not the target query ID or URL parameter names.

Reset clears the other filters for the target query while keeping the excluded values, such as the visitor's search term. With **Hide if no active filter** enabled, the reset button hides once only excluded filters remain active.

This setting is separate from the exclusion list on the Active Filters element, which controls which filters appear in that element.

:::tip[Developer reference]
See the [Filter - Submit / Reset Schema](/developer/schema/elements/filter-submit/) for the schema snapshot and Bricks 2.4 settings reference.
:::
