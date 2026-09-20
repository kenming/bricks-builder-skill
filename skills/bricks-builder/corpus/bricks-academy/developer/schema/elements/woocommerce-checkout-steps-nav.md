---
title: "Checkout Steps Navigation Schema"
description: "Schema for Bricks Checkout steps navigation element"
canonical: "https://academy.bricksbuilder.io/developer/schema/elements/woocommerce-checkout-steps-nav/"
markdownUrl: "https://academy.bricksbuilder.io/developer/schema/elements/woocommerce-checkout-steps-nav.md"
pageType: "article"
section: "developer"
category: "schema"
lastmod: "2026-09-16T10:41:20.000Z"
---
import SchemaJson from '../../../../../components/SchemaJson.astro'

| Property | Value |
|---|---|
| `name` | woocommerce-checkout-steps-nav |
| `category` | woocommerce_checkout |
| `tag` | div |
| `nestable` | true |

<SchemaJson path="elements/woocommerce-checkout-steps-nav.json" />

## Controls

| Key | Type | Label | CSS |
|---|---|---|---|
| `showStepNumber` | checkbox | Show step number | — |
| `wrapperDisplay` | select | Display | `display` on `.brx-checkout-steps-nav-list` |
| `wrapperDirection` | direction | Direction | `flex-direction` on `.brx-checkout-steps-nav-list` |
| `wrapperJustifyContent` | justify-content | Justify content | `justify-content` on `.brx-checkout-steps-nav-list` |
| `wrapperAlignItems` | align-items | Align items | `align-items` on `.brx-checkout-steps-nav-list` |
| `wrapperWrap` | select | wrapperWrap | `flex-wrap` on `.brx-checkout-steps-nav-list` |
| `wrapperWidth` | number | Width | `width` on `.brx-checkout-steps-nav-list` |
| `wrapperGap` | number | Gap | `gap` on `.brx-checkout-steps-nav-list` |
| `itemTypography` | typography | Typography | `font` on `.brxe-woocommerce-checkout-step-nav-item` |
| `stepNumberPlacement` | select | Placement | `order` on `.brx-checkout-steps-nav-list[data-brx-show-steps] .brxe-woocommerce-checkout-step-nav-item::before` |
| `stepNumberInlineOffsetStart` | number | Inline start offset | `margin-inline-start` on `.brx-checkout-steps-nav-list[data-brx-show-steps] .brxe-woocommerce-checkout-step-nav-item::before` |
| `stepNumberInlineOffsetEnd` | number | Inline end offset | `margin-inline-end` on `.brx-checkout-steps-nav-list[data-brx-show-steps] .brxe-woocommerce-checkout-step-nav-item::before` |
| `stepNumberBlockOffset` | number | Block offset | `margin-block-start` on `.brx-checkout-steps-nav-list[data-brx-show-steps] .brxe-woocommerce-checkout-step-nav-item::before` |
| `stepNumberTypography` | typography | Typography | `font` on `.brx-checkout-steps-nav-list[data-brx-show-steps] .brxe-woocommerce-checkout-step-nav-item::before` |
| `itemActiveTypography` | typography | Typography | `font` on `.brxe-woocommerce-checkout-step-nav-item.is-active, .brxe-woocommerce-checkout-step-nav-item.brx-builder-active-nav-item` |
| `itemCompletedTypography` | typography | Typography | `font` on `.brxe-woocommerce-checkout-step-nav-item.is-completed` |
| `wrapperMargin` | spacing | Margin | `margin` on `.brx-checkout-steps-nav-list` |
| `wrapperPadding` | spacing | Padding | `padding` on `.brx-checkout-steps-nav-list` |
| `wrapperBackgroundColor` | color | Background color | `background-color` on `.brx-checkout-steps-nav-list` |
| `wrapperBorder` | border | Border | `border` on `.brx-checkout-steps-nav-list` |
| `wrapperBoxShadow` | box-shadow | Box shadow | `box-shadow` on `.brx-checkout-steps-nav-list` |
| `wrapperTypography` | typography | Typography | `font` on `.brx-checkout-steps-nav-list` |
| `itemMargin` | spacing | Margin | `margin` on `.brxe-woocommerce-checkout-step-nav-item` |
| `itemPadding` | spacing | Padding | `padding` on `.brxe-woocommerce-checkout-step-nav-item` |
| `itemBackgroundColor` | color | Background color | `background-color` on `.brxe-woocommerce-checkout-step-nav-item` |
| `itemBorder` | border | Border | `border` on `.brxe-woocommerce-checkout-step-nav-item` |
| `itemBoxShadow` | box-shadow | Box shadow | `box-shadow` on `.brxe-woocommerce-checkout-step-nav-item` |
| `stepNumberMargin` | spacing | Margin | `margin` on `.brx-checkout-steps-nav-list[data-brx-show-steps] .brxe-woocommerce-checkout-step-nav-item::before` |
| `stepNumberPadding` | spacing | Padding | `padding` on `.brx-checkout-steps-nav-list[data-brx-show-steps] .brxe-woocommerce-checkout-step-nav-item::before` |
| `stepNumberBackgroundColor` | color | Background color | `background-color` on `.brx-checkout-steps-nav-list[data-brx-show-steps] .brxe-woocommerce-checkout-step-nav-item::before` |
| `stepNumberBorder` | border | Border | `border` on `.brx-checkout-steps-nav-list[data-brx-show-steps] .brxe-woocommerce-checkout-step-nav-item::before` |
| `stepNumberBoxShadow` | box-shadow | Box shadow | `box-shadow` on `.brx-checkout-steps-nav-list[data-brx-show-steps] .brxe-woocommerce-checkout-step-nav-item::before` |
| `itemActiveBackgroundColor` | color | Background color | `background-color` on `.brxe-woocommerce-checkout-step-nav-item.is-active, .brxe-woocommerce-checkout-step-nav-item.brx-builder-active-nav-item` |
| `itemActiveBorder` | border | Border | `border` on `.brxe-woocommerce-checkout-step-nav-item.is-active, .brxe-woocommerce-checkout-step-nav-item.brx-builder-active-nav-item` |
| `itemActiveBoxShadow` | box-shadow | Box shadow | `box-shadow` on `.brxe-woocommerce-checkout-step-nav-item.is-active, .brxe-woocommerce-checkout-step-nav-item.brx-builder-active-nav-item` |
| `itemCompletedBackgroundColor` | color | Background color | `background-color` on `.brxe-woocommerce-checkout-step-nav-item.is-completed` |
| `itemCompletedBorder` | border | Border | `border` on `.brxe-woocommerce-checkout-step-nav-item.is-completed` |
| `itemCompletedBoxShadow` | box-shadow | Box shadow | `box-shadow` on `.brxe-woocommerce-checkout-step-nav-item.is-completed` |

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
