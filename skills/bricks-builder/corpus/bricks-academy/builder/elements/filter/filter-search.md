---
title: "Filter search"
description: "Provides a live AJAX search input for real-time content filtering. Searches through post content, titles, and custom fields without page refresh. Features."
canonical: "https://academy.bricksbuilder.io/builder/elements/filter/filter-search/"
markdownUrl: "https://academy.bricksbuilder.io/builder/elements/filter/filter-search.md"
pageType: "article"
section: "builder"
category: "elements"
lastmod: "2026-09-30T17:19:56.000Z"
---
Provides a live AJAX search input for real-time content filtering. Searches through post content, titles, and custom fields without page refresh. Features debouncing, minimum character requirements, and optional clear functionality.

**Tip:** Perfect for creating instant search experiences. Use the debounce setting to control API call frequency, and minimum characters to improve performance.

## Settings

- **Target query** (query-list) - Select the query this filter should target. Only post queries are supported in this version.
- **URL parameter** (text) - Define a unique, more readable URL parameter name for this filter.
- **Apply on** (select) - Choose when to apply the filter. Options: Input (immediate), Submit (button click or Enter). Default: Input.
- **Debounce (ms)** (number) - Delay before triggering search after typing stops. Default: 500ms.
- **Min. characters** (number) - Minimum characters required to trigger search. Default: 3.
- **Enter action** (select, Bricks 2.4) - Choose **AJAX search** (default) or **Redirect to URL**. Requires a target query.
- **Trigger Filter Submit interactions** (checkbox, Bricks 2.4) - Run the target query's Filter Submit start/end interactions when Enter triggers an AJAX search. Disabled by default and available when Enter action is AJAX search.
- **Redirect to** (text, Bricks 2.4) - Destination URL when Enter action is Redirect to URL. Active filters for the same query are appended as URL parameters.
- **Open in new tab** (checkbox, Bricks 2.4) - Open the Enter-key redirect in a new tab. Available when a redirect URL is set.
- **Input** - Settings for the search input field.
  - **Placeholder** (text) - Placeholder text for the search input. Default: Search.
  - **Placeholder typography** (typography) - Typography for placeholder text.
  - **Label** (text) - Optional label text above the input field.
  - **Label typography** (typography) - Typography for the label text.
- **Icon (Clear)** - Settings for the clear/reset icon.
  - **Icon** (icon) - Icon to display for clearing the search.
  - **Icon color** (color) - Color of the clear icon.
  - **Icon size** (number) - Size of the clear icon.
- **Active filter** - Settings for active filter display.
  - **Prefix** (text) - Text to display before filter value.
  - **Suffix** (text) - Text to display after filter value.
  - **Title** (text) - Custom title attribute for filter links.

## Search with Enter

Pressing Enter runs the configured action immediately, including when **Apply on** is set to **Submit**. Enter bypasses the typing debounce and minimum character threshold.

For a search field that takes visitors to another results page, select a **Target query**, set **Enter action** to **Redirect to URL**, and enter the destination under **Redirect to**. Configure the destination's filters to recognize the same URL parameter names. Leave **Open in new tab** off to navigate in the current tab. An empty redirect URL falls back to an AJAX search.

For an AJAX search that should close an Offcanvas after submission, enable **Trigger Filter Submit interactions** and use the [Filter Submit interaction triggers](/builder/features/interactions/#filter-submit-triggers). Ordinary typing does not trigger these submit interactions. The redirect action does not run them.

:::tip[Developer reference]
See the [Filter - Search Schema](/developer/schema/elements/filter-search/) for the schema snapshot and Bricks 2.4 settings reference.
:::
