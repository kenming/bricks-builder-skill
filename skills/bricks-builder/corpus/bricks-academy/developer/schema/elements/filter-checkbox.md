---
title: "Filter - Checkbox Schema"
description: "Schema for Bricks Filter - Checkbox element"
canonical: "https://academy.bricksbuilder.io/developer/schema/elements/filter-checkbox/"
markdownUrl: "https://academy.bricksbuilder.io/developer/schema/elements/filter-checkbox.md"
pageType: "article"
section: "developer"
category: "schema"
lastmod: "2026-09-30T17:19:56.000Z"
---
import SchemaJson from '../../../../../components/SchemaJson.astro'

| Property | Value |
|---|---|
| `name` | filter-checkbox |
| `category` | general |
| `tag` | div |
| `nestable` | false |

<SchemaJson path="elements/filter-checkbox.json" />

## Controls

| Key | Type | Label | CSS |
|---|---|---|---|
| `filterQueryId` | query-list | Target query | — |
| `filterNiceName` | text | URL parameter | — |
| `filterApplyOn` | select | Apply on | — |
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
| `filterCountNoBracket` | checkbox | Hide count bracket | — |
| `filterHierarchical` | checkbox | Hierarchical | — |
| `filterAutoCheckChildren` | checkbox | Auto toggle child terms | — |
| `filterChildIndentation` | text | Indent | — |
| `filterChildIndentationGap` | number | Indent | `margin-inline-start` on `[class*="depth-"]:not([class*="depth-0"])` |
| `fieldProvider` | select | Provider | — |
| `customFieldKey` | text | Meta key | — |
| `fieldCompareOperator` | select | Compare | — |
| `fieldCompareType` | select | Compare type | — |
| `filterMultiLogic` | select | Multiple options | — |
| `filterGroupLabel` | text | Group label | — |
| `labelMapping` | select | Label | — |
| `customLabelMapping` | repeater | Label | — |
| `populatedOptionsOrderBy` | select | Order by | — |
| `populatedOptionsOrder` | select | populatedOptionsOrder | — |
| `displayMode` | select | Mode | — |
| `optionsGap` | number | Option | `--brx-options-gap` |
| `buttonOptionsGap` | number | Option | `--brx-btn-options-gap` |
| `optionsTypography` | typography | Option | `font` on `.brx-option-text` |
| `countAlignEnd` | checkbox | Count | — |
| `countTypography` | typography | Count | `font` on `.brx-option-count` |
| `buttonSize` | select | Size | — |
| `buttonStyle` | select | Style | — |
| `buttonCircle` | checkbox | Circle | — |
| `buttonOutline` | checkbox | Outline | — |
| `buttonBackgroundColor` | color | Background color | `background-color` on `&[data-mode="button"] .bricks-button` |
| `buttonBorder` | border | Border | `border-color` on `&[data-mode="button"] .bricks-button` |
| `buttonTypography` | typography | Typography | `font` on `&[data-mode="button"] .bricks-button` |
| `buttonActiveBackgroundColor` | color | Background color | `background-color` on `&[data-mode="button"] .bricks-button.brx-option-active` |
| `buttonActiveBorder` | border | Border | `border-color` on `&[data-mode="button"] .bricks-button.brx-option-active` |
| `buttonActiveTypography` | typography | Typography | `font` on `&[data-mode="button"] .bricks-button.brx-option-active` |
| `filterActivePrefix` | text | Prefix | — |
| `filterActiveSuffix` | text | Suffix | — |
| `filterActiveTitle` | text | Title | — |
| `limitOptions` | number | Visible options limit | — |
| `showMoreText` | text | Show more | — |
| `showLessText` | text | Show less | — |
| `showMoreButtonSize` | select | Size | — |
| `showMoreButtonStyle` | select | Style | — |
| `showMoreButtonCircle` | checkbox | Circle | — |
| `showMoreButtonOutline` | checkbox | Outline | — |
| `showMoreButtonBackgroundColor` | color | Background color | `background-color` on `.brx-show-more-less-button` |
| `showMoreButtonBorder` | border | Border | `border-color` on `.brx-show-more-less-button` |
| `showMoreButtonTypography` | typography | Typography | `font` on `.bricks-button.brx-show-more-less-button` |

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
