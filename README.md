# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview] (#overview)
  - [The challenge] (#the challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)

## Overview

The overview is to build a product preview card component with html and css.

### Screenshot

![mobile image of perfume bottle](images/screenshot-mobile.png)

![desktop image of perfume bottle](images/screenshot-desktop.png)

### Links

- Solution URL: https://fem-product-preview-edit.netlify.app/
- Live Site URL: https://github.com/John-Davidson-8?tab=repositories

## My process

My process in this my first Frontend Mentor challenge was to follow Kevin Powell as he created this component, pushed it to Github and deployed on Netlify -- https://www.youtube.com/watch?v=B2WL6KkqhLQ. My process included using the provided Figma sketches.

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

The reason I watched Kevin was not so much to help me with the general coding of the component but to become familiar with the following:

- process of initialising the repo and deploying to Github and Netlify.
- I learned a variety coding practices including setting up global css for a small project.
- Also, the picture tag and source tag in html and how to put a media query within was a revelation to me! I have copied and pasted the code directly below in the html section.
- Kevin also showed how to set "visually hidden" information for accessability. In this project two prices sit next to each other, the previous price has been scored out, and the new discounted price is larger and a different color. A visually impaired person would only hear the two prices one after the other from the software reading the component. We inserted "current price," and "original price" to be read by screen reader, but hidden visually.

```html
<picture class="product-img">
  <source
    srcset="images/image-product-desktop.jpg"
    media="(min-width: 600px)"
  />
  <img src="./images/image-product-mobile.jpg" alt="perfume image" />
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

```html
<div class="flex-group">
  <p class="product-price">
    <span class="visually-hidden">Current price:</span>
    $149.99
  </p>
  <p class="product-original-price">
    <span class="visually-hidden">Original price</span>
    <s>$169.99</s>
  </p>
</div>
```

### Continued Development

- CSS Flexbox and CSS Grid need to be learned before moving on to Tailwind or any other library.
- Continue using terminal, Github and Netlify until it becomes second nature.
- Next challenge is to create a Frontend Mentor project without following a tutor.
- Continue to learn how to write README's. This not only helps other folk understand my code better, but also helps me understand my code better as it is a fantastic means of self reflection. Writing about coding is a wonderfull way to learn how to communicate coherently within a team discutssing code.

### Useful resources - [Example resource 1](https://www.example.com)

- Kevin Powell created the project, pushed it to Github and deployed it Netlify. Here is his excellent Youtube channel link https://www.youtube.com/watch?v=B2WL6KkqhLQ

- John Smilga has taught me HTML and CSS with his Udemy course. https://www.udemy.com/course/in-depth-html-css-course-build-responsive-websites/

- Coding Addict is John Smilga's excellent Youtube channel with many great frontend resources. https://www.youtube.com/@CodingAddict.

- Most of the Git and Github process I have learned from Colte Steele's excellent Udemy course https://www.udemy.com/course/git-and-github-bootcamp/.
