<h1 align="center">Shoe Product Page | devChallenges</h1>

<div align="center">
  Solution for the <a href="https://devchallenges.io/" target="_blank">devChallenges.io</a> product page challenge.
</div>

<div align="center">
  <h3>
    <a href="#">Demo</a>
    <span> | </span>
    <a href="#">Solution</a>
    <span> | </span>
    <a href="https://devchallenges.io/" target="_blank">Challenge</a>
  </h3>
</div>

## Table of Contents

- [Overview](#overview)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Built with](#built-with)
- [Features](#features)
- [Author](#author)

## Overview

![screenshot](https://media.discordapp.net/attachments/1464634656463786118/1566922513152213082/Captura_de_tela_de_2026-11-02_18-10-02.png?ex=6aea4dcf&is=6ae8fc4f&hm=ccb7bfbada6653f6f75b9591ae59b632a3338f5499a0f461bd349e673c08fa39&=&format=webp&quality=lossless)

A responsive product page for the Nike Air Zoom Pegasus 38 running shoe. The page presents the product image, description, highlights, selected color and size, price, and purchase-related buttons.

The layout is designed mobile-first: on smaller screens, the product image and information are stacked vertically. On wider screens, CSS Grid places them side by side.

### What I learned

During this project, I practiced structuring a product page and adapting its layout to different screen sizes:

- **CSS Grid:** Used `grid-template-columns` to change the main layout from one column to two columns on larger screens.
- **Responsive design:** Applied media queries with `min-width` breakpoints to adjust spacing, image dimensions, and the product information layout.
- **Flexbox:** Used Flexbox to organize the breadcrumb navigation, product details, highlights, and action buttons.
- **Responsive images:** Used the HTML `<picture>` and `<source>` elements to provide different image sources depending on the viewport width.
- **Image sizing:** Practiced using `max-width`, `max-height`, and `height: auto` to control the product image without forcing a fixed height.
- **Google Fonts:** Imported and used the `Outfit` font.

Example of the responsive main layout:

```css
main {
  display: grid;
  grid-template-columns: 1fr;
  gap: 30px;
  justify-items: center;
}

@media (min-width: 1024px) {
  main {
    grid-template-columns: 1fr 2fr;
    align-items: start;
    justify-items: flex-end;
    gap: 45px;
  }
}
```

### Useful resources

- [Google Fonts - Outfit](https://fonts.google.com/specimen/Outfit) - Font used throughout the page.
- [MDN Web Docs - CSS Grid](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_grid_layout) - Reference for creating the main page layout.
- [MDN Web Docs - Flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_flexible_box_layout) - Reference for arranging elements within the product information area.
- [MDN Web Docs - The picture element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/picture) - Reference for using responsive image sources.
- [MDN Web Docs - Media queries](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_media_queries/Using_media_queries) - Reference for adapting styles to different viewport sizes.

### Built with

- Semantic HTML5
- CSS3 (Vanilla CSS)
- CSS Grid
- Flexbox
- Media Queries
- HTML `<picture>` and `<source>` elements
- Google Fonts (`Outfit`)

## Features

- **Responsive layout:** Product image and information are stacked on smaller screens and displayed side by side on screens wider than 1024px.
- **Product presentation:** Includes a product title, description, and highlights.
- **Product details:** Displays the selected color, size, and price.
- **Product image:** Uses the `<picture>` element to select an image source based on viewport width.
- **Purchase interface:** Includes “Add to cart” and “Add to wishlist” buttons.
- **Typography:** Uses the Outfit font from Google Fonts.

> Note: The purchase and wishlist buttons are currently visual elements; no cart or wishlist functionality is implemented in the provided code.

## Author

- Coded by **Victor C. Ricci**
- GitHub [@victorricci23](https://github.com/victorricci23)
