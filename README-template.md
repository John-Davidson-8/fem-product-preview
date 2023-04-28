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
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

- Create a responsive card which moves from one column into two on a wider screen.

### Screenshot

![![Alt text](../../../Desktop/Screenshot%202023-04-28%20at%2014.33.30.png)](./screenshot.jpg)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

- This is the first time I used the picture element. I feel it worked well. The html code is below.

- Also the first time I used "visually hidden" accessibility function. Reason for use was the previous price of the product had a strikethrough. This obviously would not be adequate for folk who are visually impaired. The code would make the strikethrough be read out by screen reader. The code is below.

```html
<picture class="product__img">
  <source
    srcset="images/image-product-desktop.jpg"
    media="(min-width: 600px)"
  />
  <img
    src="./images/image-product-mobile.jpg"
    alt="Gabrielle Essence perfume bottle laying flat on a table"
  />
</picture>
```

```css
.visually-hidden:not(:focus):not(:active) {
  clip: rect(0 0 0 0);
  clip-path: inset(50%);
  height: 1px;
  overflow: hidden;
  position: absolute;
  white-space: nowrap;
  width: 1px;
}
```

### Continued development

Continued development must include layout issues using CSS Flex-box.

### Useful resources

- [Example resource 1](https://www.youtube.com/watch?v=B2WL6KkqhLQ&t=1s) - Kevin Powell creates this project on his Youtube channel. It was he taught me the accessibility code "visually hidden."

## Author

- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/John-Davidson-8)
