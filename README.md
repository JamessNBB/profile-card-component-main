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
- [Acknowledgments](#acknowledgments)


## Overview

### The challenge

- Build out the project to the designs provided

### Screenshot

![Desktop-view screenshot](screenshots/desktop-view.png)

![Mobile-view screenshot](screenshots/mobile-view.png)

### Links

- Solution URL: [Solution URL](https://github.com/JamessNBB/profile-card-component-main.git)
- Live Site URL: [Live site URL](https://jamessnbb.github.io/profile-card-component-main/)


## My process

### Built with

- HTML
- CSS 


### What I learned

I struggled a lot trying to position the bg-pattern-top and bg-patter-botttom images on the page. The challenge was not really the positioning itself but rather containing the images within it so that the width and height of the page does not increase. When I insert the images, the horizontal and vertical scroll appears, and this is not what I wanted. I tried using an overlay but it did not work. I also tried using different units of measurement for the width and height of the "main-container" element such as vw, vh, and percentages, but the bg-pattern-bottom image was still appearing in full scale and not cutting off at the end of the page, thereby causing the vertical and horizontal scrolls to appear. 

I pretty much gave up at this point, until I learned about the "overflow" CSS property:

```css
.main-container {
  overflow: hidden;
}
```

With this, I was able to properly place the images at their right positions without them appearing in their full scale and increasing the width and height of the page and causing the vertical and horizontal scrolls to appear, but instead, they cut off at the end of the page, just as desired. 


### Continued development
I would like to conitnue to develop more on the proper usage of HTML semantics and advanced CSS properties.


### Useful resources

- [W3Schools](https://www.w3schools.com/) - Excellent place to get you started on your programming journey. It helped me understand some basic HTML elements and CSS properties.


## Author

- GitHub - [James](https://github.com/JamessNBB)
- Frontend Mentor - [@JamessNBB](https://www.frontendmentor.io/profile/JamessNBB)


## Acknowledgments

I'd like to acknowledge [Chaoo Charles](https://youtu.be/ZezbT_12e3k?si=3MS84y8CfuQ3R7p6). Seeing his solution made me realize what I was missing. I was able to learn about the "overflow: hidden;" CSS property, which I incorporated into my solution and got my desired outcome.