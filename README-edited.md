# Frontend Mentor - Profile card component solution

This is a solution to the [Profile card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/profile-card-component-cfArpWshJ). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

- Build out the project to the designs provided

### Screenshot

Mobile view
![](./06mobile_view.png)

Desktop view
![](./06desktop_view.png)


### Links

- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned

1. On position of the background image

At first, I tried to used % as the reference to set the position of the background. But it turns out that % is not based on only the width of container but (container's width - image width) * percentage = the "margin" of the background to the container.

Reference: https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwi8_Y22o4H2AhVEL6YKHSA9DJsQFnoECAYQAQ&url=https%3A%2F%2Fdeveloper.mozilla.org%2Fen-US%2Fdocs%2FWeb%2FCSS%2Fbackground-position&usg=AOvVaw0_gDhbPq5SnLKzsqGo51Lz


But be careful, if background-attachment was set to fixed, the container will be viewport.   
https://developer.mozilla.org/en-US/docs/Web/CSS/background-attachment

```css
body {
  background-image: url("./images/bg-pattern-top.svg"),
                    url("./images/bg-pattern-bottom.svg");
  background-position: top -50vh right 50vw,
                        bottom -50vh left 50vw;
  background-repeat: no-repeat;
}
```

### Continued development

Would like to understand more on why not using px and rem/ em instead.

## Author

- Frontend Mentor - [@Ma1021](https://www.frontendmentor.io/profile/Ma0121)