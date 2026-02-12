# Frontend Mentor - Single price grid component solution

This is a solution to the [Single price grid component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/single-price-grid-component-5ce41129d0ff452fec5abbbc). Frontend Mentor challenges help me improve my coding skills by building realistic projects.

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

## Overview

### The challenge

The brief for this project was to build out the single price grid component and get it looking as close to the design as possible, starting with the following assets:

- Figma design file for mobile, tablet, and desktop layouts
- JPEG design files for mobile and desktop layouts
- Style guide for fonts, colors, etc.
- Optimized image assets
- HTML file with pre-written content

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- See a hover state on desktop for the Sign Up call-to-action

### Screenshot

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it.

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- [Live Site](https://sabineemden.github.io/fm-single-price-grid-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

I used CSS Grid for the responsive layout of the component. The mobile design has one column. For the tablet and desktop design, the layout changes to two columns with the first row spanning both columns.

In the mobile design, the hight of the first row is determined by its content. The second and third row have equal hight. I was able to match the design by using the `auto` keyword for the height of the first row and `1fr` for the second and third row.

```css
.component {
  display: grid;
  grid-template-rows: auto 1fr 1fr;
  max-width: 24rem;
  /* ... */
}
```

For the tablet and desktop design, the grid changes to two rows with heights determined by their content and two columns of equal width.

```css
@media (min-width: 48em) {
  .component {
    grid-template: auto auto / 1fr 1fr;
    max-width: 40rem;
  }
  /* ... */
}
```

### Continued development

My CSS Grid skills are still a bit rusty. I need to do a more thorough review of the topic.

If this was a real-life project, I would want to talk to the designer and ask whether there was any chance to increase the color contrasts to make the text more readable and meet web accessibility standards.

### Useful resources

- [Essential Visually Hidden CSS Techniques for Web Accessibility](https://www.a11y-collective.com/blog/visually-hidden/) - I found the code snippet for the visually hidden text in this article.

## Author

I'm an aspiring web developer and a former chemist. What I bring from chemistry to software development is a systematic approach to problem solving and the perseverance to not give up easily.

- Frontend Mentor - [SabineEmden](https://www.frontendmentor.io/profile/SabineEmden)
- Personal Website - [Sabine Emden](https://www.sabineemden.com/)
- Mastodon - [@sabineemden](https://social.tchncs.de/@sabineemden)

## Acknowledgments

This project uses Josh Comeau's [CSS Reset](https://www.joshwcomeau.com/css/custom-css-reset/).

The font family in this project is [Karla](https://fonts.google.com/specimen/Karla). The fonts are licensed under the [Open Font License](https://openfontlicense.org/open-font-license-official-text/).
