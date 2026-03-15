# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](./screenshot.jpg)

### Links

- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS Flexbox
- Responsive design with media queries
- Google Fonts (Fraunces & Montserrat)
- Mobile-friendly layout

### What I learned

**Flexbox for card layout** — I used `display: flex` on the `.card` to place the image and content side by side on desktop, then switched to `flex-direction: column` inside a media query for mobile.

**Selective border-radius** — Instead of rounding all corners of the card image, I used the longhand properties to only round the left corners on desktop, so it sits flush with the card edge:

```css
border-top-left-radius: 10px;
border-bottom-left-radius: 10px;
```

On mobile, I switched to the shorthand to only round the top corners:

```css
border-radius: 10px 10px 0 0;
```

**`object-fit: cover`** — This kept the product image filling its container without stretching or distorting it, which was especially important on mobile where I set a `max-height`.

**Hover state on the button** — I used a CSS transition to smoothly change the button background color on hover:

```css
transition: background-color 0.3s ease;
```

### Continued development

- Getting more comfortable with responsive design and knowing when to use `max-width` vs `width`
- Practicing more with CSS custom properties (variables) to manage colors in one place
- Learning more about accessibility — things like focus states for keyboard users and proper alt text

## Author

- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
