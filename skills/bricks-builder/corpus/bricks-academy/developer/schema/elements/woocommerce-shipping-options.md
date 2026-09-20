---
title: "Shipping Options Schema"
description: "Schema for Bricks Shipping options element"
canonical: "https://academy.bricksbuilder.io/developer/schema/elements/woocommerce-shipping-options/"
markdownUrl: "https://academy.bricksbuilder.io/developer/schema/elements/woocommerce-shipping-options.md"
pageType: "article"
section: "developer"
category: "schema"
lastmod: "2026-09-16T10:41:20.000Z"
---
import SchemaJson from '../../../../../components/SchemaJson.astro'

| Property | Value |
|---|---|
| `name` | woocommerce-shipping-options |
| `category` | woocommerce_checkout |
| `tag` | div |
| `nestable` | false |

<SchemaJson path="elements/woocommerce-shipping-options.json" />

## Controls

| Key | Type | Label | CSS |
|---|---|---|---|
| `showPackageTitle` | checkbox | Show package title | — |
| `emptyMessage` | text | Empty message | — |
| `controlFlexDirection` | direction | Direction | `flex-direction` on `.brx-shipping-options__control` |
| `controlJustifyContent` | justify-content | Justify content | `justify-content` on `.brx-shipping-options__control` |
| `controlAlignItems` | align-items | Align items | `align-items` on `.brx-shipping-options__control` |
| `controlGap` | number | Gap | `gap` on `.brx-shipping-options__control` |
| `packageTitleTypography` | typography | Title typography | `font` on `.brx-shipping-options__package-title` |
| `packageTitleColor` | color | Title color | `color` on `.brx-shipping-options__package-title` |
| `optionGap` | number | Gap | `gap` on `.brx-shipping-options__label-group` |
| `optionHoverBackgroundColor` | color | Hover background color | `background-color` on `.brx-shipping-options__option:hover` |
| `optionCheckedBackgroundColor` | color | Background color | `background-color` |
| `optionCheckedBorder` | border | Border | `border` |
| `optionCheckedBoxShadow` | box-shadow | Box shadow | `box-shadow` |
| `labelTypography` | typography | Typography | `font` on `.brx-shipping-options__label` |
| `labelColor` | color | Color | `color` on `.brx-shipping-options__label` |
| `labelCheckedTypography` | typography | Typography | `font` |
| `labelCheckedColor` | color | Color | `color` |
| `secondaryTypography` | typography | Typography | `font` on `.brx-shipping-options__secondary-label` |
| `secondaryColor` | color | Color | `color` on `.brx-shipping-options__secondary-label` |
| `secondaryCheckedTypography` | typography | Typography | `font` |
| `secondaryCheckedColor` | color | Color | `color` |
| `packageMargin` | spacing | Margin | `margin` on `.brx-shipping-options__package` |
| `packagePadding` | spacing | Padding | `padding` on `.brx-shipping-options__package` |
| `packageBackgroundColor` | color | Background color | `background-color` on `.brx-shipping-options__package` |
| `packageBorder` | border | Border | `border` on `.brx-shipping-options__package` |
| `packageBoxShadow` | box-shadow | Box shadow | `box-shadow` on `.brx-shipping-options__package` |
| `optionMargin` | spacing | Margin | `margin` on `.brx-shipping-options__option` |
| `optionPadding` | spacing | Padding | `padding` on `.brx-shipping-options__option` |
| `optionBackgroundColor` | color | Background color | `background-color` on `.brx-shipping-options__option` |
| `optionBorder` | border | Border | `border` on `.brx-shipping-options__option` |
| `optionBoxShadow` | box-shadow | Box shadow | `box-shadow` on `.brx-shipping-options__option` |

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
