# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Links

- Solution URL: [https://github.com/lesandra007/product-preview-card-component-main](https://github.com/lesandra007/product-preview-card-component-main)
- Live Site URL: [https://transcendent-sfogliatella-883205.netlify.app/](https://transcendent-sfogliatella-883205.netlify.app/)

## My process

### Built with

- [Visual Studio Code](https://code.visualstudio.com/) - to write code
- [Netlify](https://www.netlify.com/) - to deploy website

### What I learned

html and css basics! This is my first html/css project!

Responsive layouts with grid display and media:
```css
.product {
    --content-padding: 1.5rem;
    --content-spacing: 1rem;

    display: grid;
    
    background-color: var(--clr-neutral-100);
    border-radius: 0.5rem;
    overflow: hidden;
    max-width: 600px;
}

@media(min-width: 600px){
    .product{
        --content-padding: 2rem;
        grid-template-columns: 1fr 1fr;
    }
}
```
Responsive between desktop and mobile images depending on size:
```html
<picture class="product__img">
        <source srcset="images/image-product-desktop.jpg" media="(min-width: 600px)">
        <img src="images/image-product-mobile.jpg" 
          alt="Gabrielle Essence perfume bottole laying flat on a table">
      </picture>
```

### Useful resources

- [Kevin Powell's Solution](https://www.youtube.com/watch?v=B2WL6KkqhLQ) - A solution for this challenge.
- [Josh Comeau's CSS reset](https://www.joshwcomeau.com/css/custom-css-reset/) - Contains code for more responsive images; no more overflow.
- [Visually Hidden](https://www.scottohara.me/blog/2017/04/14/inclusively-hidden.html) - Contains code that allows for text to be visually hidden while being accessible to a screen reader.

## Acknowledgments

Solution by Kevin Powell.
