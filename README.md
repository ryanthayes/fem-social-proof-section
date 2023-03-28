# Frontend Mentor - Social proof section solution

This is a solution to the [Social proof section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-proof-section-6e0qTv_bA). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout for the section depending on their device's screen size

### Screenshot

![](./solution.png)

### Links

- [Solution](https://github.com/ryanthayes/fem-social-proof-section)
- [Live URL](https://ryanthayes.github.io/fem-social-proof-section)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

This one took some time to figure out. At first I didn't look in the assets folder and didn't realize there was an SVG for the stars. I thought I needed to use font awesome icons. I tried that at first and it did work, but wasn't exact. Then I realized there was an SVG file in the assets folder. However, I didn't want FIVE img elements in my HTML for each rating. So, instead I used ::before that I learned following a tutorial with Kevin Powell to bring the images in through CSS. This led to much cleaner HTML code. I am actually surprised it worked.


```css
.stars::before {
    content: 
    url(images/icon-star.svg) ' ' url(images/icon-star.svg) ' ' url(images/icon-star.svg) ' ' url(images/icon-star.svg) ' ' url(images/icon-star.svg);
}
```

### Continued development

I am still not as confident with grid compared to flex. I tried to create this whole project as one big grid with two rows. But I struggled for over an hour trying to get the "cards" to move to different grid columns on the second row. 

I tried grid areas. I tried grid-column-rows. All three "cards" just stayed in the first column of the second row. I could move the two divs on the top row, but no success on the bottom row. So, I ended up using a separate grid for the bottom row.

## Author

- Github - [@ryanthayes](https://github.com/ryanthayes)
- Frontend Mentor - [@ryanthayes](https://www.frontendmentor.io/profile/ryanthayes)