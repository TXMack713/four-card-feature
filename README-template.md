# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![file:///home/txmack713/Downloads/FireShot/FireShot%20Capture%20002%20-%20Frontend%20Mentor%20-%203-column%20preview%20card%20component%20-%20127.0.0.1.png]

### Links

- Solution URL: [GitHub/TXMack713](https://github.com/TXMack713/four-card-feature/)
- Live Site URL: [GitHub Pages] (https://txmack713.github.io/four-card-feature/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Mobile-first workflow

### What I learned

I learned that including the html element in your resets distorts how the page is rendered. I removed the html element from my page reset after some trial and error while struggling to get a nav bar to remain sticky while working on an MDN CSS exercise.

I initially tried laying out the page using CSS Flexbox, but was unable to achieve the responsiveness and element positioning I was expecting. I chose to switch to CSS Grid and was able to place the container, divs and div items exactly where I wanted.

Also, by submitting my solution on frontendmentor.io, I was able to look and compare my solution to others and noticed that there were some design details that I missed and was able to revist and address.

Having the static page hosted on GitHub pages allowed me to see how differently browsers rendered the same content. The Brave, Edge and Google browsers all rendered the page in mobile and desktop layouts as expected, but the Firefox browser extended the section elements fully to the top and bottom of the page. By removing the html element from my page reset and adding a 5% margin to the body element the page created the gap based on the CSS Grid inputs within the container element. However, the page still rendered the content fairly large compared to the other browsers.

```css
body {
    margin: 5% auto;
    height: 100%;
  }
  .container {
    display: grid;
    grid-template-columns: 12.5% 25% 25% 25% 12.5%;
    grid-template-rows: 20% 60% 20%;
    margin: 0 auto;
    padding: 0;
    block-size: 100%;
    justify-content: center;
    align-content: center;
    overflow: auto;
    max-inline-size: 1440px;
  }
```

### Continued development

- I've worked through Flexbox Zombies and am currently working through Grid Critters in an effort to perfect my layout skills. This lesson taught me that I still have a ways to go with in learning how to move knowing the syntax to being able to expertly position items on the page as expected.

### Useful resources
- The MDN Web Docs (https://developer.mozilla.org/en-US/) proved to be invaluable for quick lookups regarding the different values for certain properties, specifically with centering the content as expected within the containers.

## Author

- Website - [Anthony Mack](https://txmack713.github.io/four-card-feature/)
- Frontend Mentor - [@TXMack713](https://www.frontendmentor.io/profile/txmack713)

### Acknowledgements

- 