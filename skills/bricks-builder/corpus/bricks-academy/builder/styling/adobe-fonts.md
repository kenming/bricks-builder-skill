---
title: "Integration: Adobe Fonts"
description: "Connect Adobe Fonts to Bricks so your project can use synced Typekit fonts inside the builder and on the frontend."
canonical: "https://academy.bricksbuilder.io/builder/styling/adobe-fonts/"
markdownUrl: "https://academy.bricksbuilder.io/builder/styling/adobe-fonts.md"
pageType: "article"
section: "builder"
category: "styling"
lastmod: "2026-09-30T17:19:56.000Z"
---
## How to use Adobe Fonts with Bricks

All you need to do is provide Bricks with your Adobe Fonts "Project ID".

First, visit the "web projects" section inside your Adobe Fonts account: [https://fonts.adobe.com/my_fonts#web_projects-section](https://fonts.adobe.com/my_fonts#web_projects-section)

Each of your web projects contains a unique "Project ID".

Copy the project ID of the web project whose fonts you want to use on your Bricks site.



![](imgs/bricks-adobe-fonts-web-project-id-187730bd1a.png)

<figcaption>

Copy the project ID into your clipboard

</figcaption>



Next, inside your WordPress dashboard, go to `Bricks > Settings > API keys` and paste the project ID into the "Adobe fonts (Project ID)" input field. Then save your settings.



![](imgs/bricks-adobe-fonts-project-id-saved-3c1bca985c.png)

<figcaption>

Click "Sync fonts" to fetch all fonts of this project

</figcaption>



Next to the project ID input, a "Sync fonts" button should now be visible. Click it to fetch the Adobe fonts of this project. A success message should appear & the "Published Adobe fonts" counter should reflect the number of published fonts.



![](imgs/bricks-adobe-fonts-synced-9d4ecd442e.png)

<figcaption>

Fonts are now synced & available in the builder

</figcaption>



Those fonts are now available inside the builder in any `font-family` dropdown:

![](imgs/bricks-adobe-fonts-in-bricks-b87c84c96d.png)

Syncing an Adobe Fonts project only makes its fonts available in Bricks typography controls. To apply and load an Adobe font on the frontend, select it in a typography setting, such as an element, global class, Theme Style, page setting, or template setting.

Bricks loads the Adobe Fonts project CSS only when an Adobe font from the synced project is detected in the generated page CSS.

:::note
NOTE: Bricks recognizes when you use an Adobe font that is also available as a Google font. Bricks will load only the Adobe font to prevent loading this font from Google as well.
:::

## Variable fonts {#font-variation-settings}

Bricks also provides a new `font-variation-settings`. This CSS property allows you to control the four-letter axis names of a variable Adobe font. Such as the `wght`, `wdth`, `slnt`, and `ital`.

For more information about the specifics please visit [https://developer.mozilla.org/en-US/docs/Web/CSS/font-variation-settings](https://developer.mozilla.org/en-US/docs/Web/CSS/font-variation-settings)



![](imgs/bricks-adobe-fonts-variable-font-variation-settings-b62aa43f92.png)

<figcaption>

Variable Adobe font with a custom font-weight (axis: "wght") of 535

</figcaption>



You can view available variable Adobe fonts by selecting "Variable Fonts" under "Font technology on [https://fonts.adobe.com/fonts](https://fonts.adobe.com/fonts).

:::note
NOTE: This new `font-variation-settings` is also available for [custom fonts](/builder/styling/custom-fonts/). For Google Fonts, Bricks can collect multiple variation axes from the selected font and your typography settings; the available axes depend on the font and the Google Fonts API.
:::
