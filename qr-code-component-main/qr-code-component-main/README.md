# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)

## Overview

### Screenshot

![](./preview.jpg)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties (Variables)
- Google Fonts (`Outfit`)
- Flexbox
- Mobile-first workflow

### What I learned

In this project, I practiced building a responsive card component and explored key CSS layout & sizing concepts.

#### 1. CSS Box Sizing Boundaries: `width`, `max-width`, and `min-width`

- **`width`**: Defines an explicit fixed width for an element (e.g. `width: 320px`). If the screen size is smaller than this value, the element may cause horizontal scrolling.
- **`max-width`**: Prevents an element from exceeding a maximum limit while allowing it to shrink responsively on smaller viewports (e.g. `max-width: 320px`).
- **`min-width`**: Sets a lower bound for an element's size, preventing it from becoming smaller than specified even if the parent container shrinks.

#### 2. Intrinsic Content Sizing: `fit-content`, `max-content`, and `min-content`

- **`min-content`**: Shrinks the container to the smallest possible width without overflowing content (for text content, it wraps at every word boundary).
- **`max-content`**: Expands the container to fit all content on a single line without wrapping, regardless of available container space.
- **`fit-content`**: Uses available space like `max-content` up to the width of the parent container, but wraps text naturally when reaching the container bound instead of overflowing.

#### Code Snippet Showcase

```html
<section class="qr-container">
  <img src="./images/image-qr-code.png" alt="Qr bar code" class="qr-image">
  <article class="qr-specification">
    <h2 class="specification-head">
      Improve your front-end skills by building projects
    </h2>
    <p class="specification-para">
      Scan the QR code to visit Frontend Mentor and take your coding skills to the next level
    </p>
  </article>
</section>
```

```css
:root {
  --webpage-primary-background-color: rgb(199, 222, 222);
}

.qr-container {
  width: min-content;
  max-width: 320px;
  margin: 50px auto;
  padding: 15px;
  border-radius: 10px;
  background-color: white;
}
```

### Useful resources

- [MDN Web Docs - CSS `width`](https://developer.mozilla.org/en-US/docs/Web/CSS/width) - Great guide explaining `min-content`, `max-content`, and `fit-content`.
- [CSS-Tricks - A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - Useful visual guide for centering and aligning elements in CSS.

### AI Collaboration

- Used AI assistance for code review, feedback on semantic HTML structure, and organizing technical learnings into documentation.

## Author

- Frontend Mentor - [Abhinav Kumar](https://www.frontendmentor.io/profile/yourusername)
