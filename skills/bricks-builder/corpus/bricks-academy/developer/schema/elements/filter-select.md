---
title: "Filter - Select Schema"
description: "Schema for Bricks Filter - Select element"
canonical: "https://academy.bricksbuilder.io/developer/schema/elements/filter-select/"
markdownUrl: "https://academy.bricksbuilder.io/developer/schema/elements/filter-select.md"
pageType: "article"
section: "developer"
category: "schema"
lastmod: "2026-09-30T17:19:56.000Z"
---
import SchemaJson from '../../../../../components/SchemaJson.astro'

| Property | Value |
|---|---|
| `name` | filter-select |
| `category` | general |
| `tag` | div |
| `nestable` | false |

<SchemaJson path="elements/filter-select.json" />

## Controls

| Key | Type | Label | CSS |
|---|---|---|---|
| `filterQueryId` | query-list | Target query | — |
| `filterNiceName` | text | URL parameter | — |
| `filterApplyOn` | select | Apply on | — |
| `filterAction` | select | Action | — |
| `filterSource` | select | Source | — |
| `sourceFieldType` | select | Field type | — |
| `wpPostField` | select | Field | — |
| `wpUserField` | select | Field | — |
| `wpTermField` | select | Field | — |
| `filterTaxonomy` | select | Taxonomy | — |
| `filterTaxonomyOrderBy` | select | Order by | — |
| `filterTaxonomyOrderMetaKey` | text | Order meta key | — |
| `filterTaxonomyOrder` | select | filterTaxonomyOrder | — |
| `filterTermInclude` | select | filterTermInclude | — |
| `filterTermExclude` | select | filterTermExclude | — |
| `filterTermTopLevel` | checkbox | Top level terms only | — |
| `filterHideCount` | checkbox | Hide count | — |
| `filterHideEmpty` | checkbox | Hide empty | — |
| `filterHierarchical` | checkbox | Hierarchical | — |
| `filterChildIndentation` | text | Indent | — |
| `fieldProvider` | select | Provider | — |
| `customFieldKey` | text | Meta key | — |
| `fieldCompareOperator` | select | Compare | — |
| `fieldCompareType` | select | Compare type | — |
| `filterMultiLogic` | select | Multiple options | — |
| `filterLabelAll` | text | Label | — |
| `labelMapping` | select | Label | — |
| `customLabelMapping` | repeater | Label | — |
| `populatedOptionsOrderBy` | select | Order by | — |
| `populatedOptionsOrder` | select | populatedOptionsOrder | — |
| `sortOptions` | repeater | Sort options | — |
| `perPageOptions` | text | Options | — |
| `filterActivePrefix` | text | Prefix | — |
| `filterActiveSuffix` | text | Suffix | — |
| `filterActiveTitle` | text | Title | — |
| `placeholder` | text | Selection placeholder | — |
| `choicesJs` | checkbox | Enhanced select | — |
| `choicesPosition` | select | Dropdown position | — |
| `choicesSearch` | checkbox | Enable search | — |
| `choicesSearchBackground` | color | Background color | `background-color` on `input[type="search"]` |
| `choicesSearchPlaceholder` | text | Search placeholder | — |
| `choicesSearchInputTypography` | typography | Input | `font` on `.bricks-choices__input` |
| `choicesSearchInputPadding` | text | Input | `--choices-brx-search-input-padding` |
| `choicesNoResultsText` | text | No results | — |
| `choicesNoChoicesText` | text | No choices | — |
| `enableMultiple` | checkbox | Multiple options | — |
| `choicesPillGap` | number | Pill | `--choices-multiple-item-margin` |
| `choicesPillBackground` | color | Pill | `--choices-primary-color` |
| `choicesPillBorder` | border | Pill | `border` on `.bricks-choices__list--multiple .bricks-choices__item` |
| `choicesPillTypography` | typography | Pill | `font` on `.bricks-choices__list--multiple .bricks-choices__item` |
| `choicesPadding` | text | Padding | `--choices-inner-padding` |
| `choicesBackgroundColor` | color | Background | `--choices-bg-color` |
| `choicesBorderBase` | text | Border | `--choices-base-border` |
| `choicesBorderColor` | color | Border color | `--choices-keyline-color`, `border-color` on `.bricks-choices__inner, .bricks-choices__list--dropdown`, `border-color` on `.bricks-choices.is-focused .bricks-choices__inner, .bricks-choices.is-open .bricks-choices__inner, .bricks-choices.is-open .bricks-choices__list--dropdown` |
| `choicesBorderRadius` | number | Border radius | `--choices-border-radius` |
| `choicesFontSize` | number | Font size | `--choices-font-size` |
| `choicesTextColor` | color | Text color | `--choices-brx-text-color` |
| `choicesSearchTypography` | typography | Placeholder | `font` on `.bricks-choices__placeholder`, `font` on `.bricks-choices__input::placeholder` |
| `choicesPlaceholderOpacity` | number | Placeholder | `--choices-placeholder-opacity` |
| `choicesArrowColor` | color | Arrow color | `--choices-text-color` |
| `choicesItemPadding` | text | Padding | `--choices-dropdown-item-padding` |
| `choicesDropdownBackground` | color | Background | `--choices-bg-color-dropdown` |
| `choicesHighlightBackground` | color | Highlight | `--choices-highlighted-color` |
| `choicesHighlightTextColor` | color | Highlight | `--choices-brx-highlighted-text-color` |
| `choicesDisabledBackground` | color | Disabled | `--choices-brx-bg-color-disabled` |
| `choicesDisabledTextColor` | color | Disabled | `--choices-brx-text-color-disabled` |

## Inherited CSS controls

Shared CSS controls available on all elements. Keys are prefixed with `_` and support responsive/pseudo-class variants via colon syntax (e.g. `_typography:tablet_portrait:hover`).

| Key | Type | Label | CSS |
|---|---|---|---|
| `_content` | text | Content | `content` |
| `_margin` | spacing | Margin | `margin` |
| `_padding` | spacing | Padding | `padding` |
| `_width` | number | Width | `width` |
| `_widthMin` | number | Min. width | `min-width` |
| `_widthMax` | number | Max. width | `max-width` |
| `_height` | number | Height | `height` |
| `_heightMin` | number | Min. height | `min-height` |
| `_heightMax` | number | Max. height | `max-height` |
| `_aspectRatio` | text | Aspect ratio | `aspect-ratio` |
| `_position` | select | Position | `position` |
| `_top` | number | _top | `top` |
| `_right` | number | Right | `right` |
| `_bottom` | number | Bottom | `bottom` |
| `_left` | number | Left | `left` |
| `_zIndex` | number | Z-index | `z-index` |
| `_order` | number | _order | `order` |
| `_display` | select | Display | `display`, `align-items` |
| `_visibility` | select | Visibility | `visibility` |
| `_overflow` | text | Overflow | `overflow` |
| `_opacity` | number | Opacity | `opacity` |
| `_cursor` | select | Cursor | `cursor` |
| `_isolation` | select | Isolation | `isolation` |
| `_mixBlendMode` | select | Mix blend mode | `mix-blend-mode` |
| `_pointerEvents` | text | Pointer events | `pointer-events` |
| `_perspective` | number | Perspective | `perspective` |
| `_perspectiveOrigin` | text | Perspective origin | `perspective-origin` |
| `_gridItemJustifySelf` | align-items | Justify self | `justify-self` |
| `_flexDirection` | direction | Direction | `flex-direction` |
| `_alignSelf` | align-items | Align self | `align-self` |
| `_justifyContent` | justify-content | Align main axis | `justify-content` |
| `_alignItems` | align-items | Align cross axis | `align-items` |
| `_gap` | number | Gap | `gap` |
| `_flexGrow` | number | Flex grow | `flex-grow` |
| `_flexShrink` | number | Flex shrink | `flex-shrink` |
| `_flexBasis` | text | Flex basis | `flex-basis` |
| `_useMasonry` | checkbox | %s layout | — |
| `_masonryColumn` | number | Columns | `--columns` |
| `_masonryGutter` | number | Spacing | `--gutter` |
| `_masonryHorizontalOrder` | checkbox | Horizontal order | — |
| `_masonryTransitionDuration` | number | Transition | — |
| `_masonryTransitionMode` | select | Reveal animation | — |
| `_typography` | typography | _typography | `font` |
| `_background` | background | _background | `background` |
| `_shapeDividers` | repeater | Custom shape | — |
| `_gradient` | gradient | _gradient | `background-image` |
| `_border` | border | Border | `border` |
| `_boxShadow` | box-shadow | Box shadow | `box-shadow` |
| `_transform` | transform | Transform | `transform` |
| `_transformOrigin` | text | Transform origin | `transform-origin` |
| `_motionElementParallax` | checkbox | Element parallax | — |
| `_motionElementParallaxSpeedX` | number | Horizontal speed | `--brx-motion-parallax-speed-x` |
| `_motionElementParallaxSpeedY` | number | Vertical speed | `--brx-motion-parallax-speed-y` |
| `_motionBackgroundParallax` | checkbox | Background parallax | — |
| `_motionBackgroundParallaxSpeed` | number | Background speed | `--brx-motion-background-speed` |
| `_motionStartVisiblePercent` | number | Parallax start point | — |
| `_cssCustom` | code | Custom CSS | — |
| `_cssClasses` | text | CSS classes | — |
| `_cssId` | text | CSS ID | — |
| `_cssFilters` | filters | CSS Filters | `filter` |
| `_cssTransition` | text | Transition | `transition` |
| `_attributes` | repeater | Name | — |
| `_scrollSnapType` | select | Type | `scroll-snap-type` on `html`, `scroll-snap-align` on `.brxe-section` |
| `_scrollSnapAlign` | select | Align | `scroll-snap-align` on `.brxe-section` |
| `_scrollSnapStop` | select | Stop | `scroll-snap-stop` on `.brxe-section` |
