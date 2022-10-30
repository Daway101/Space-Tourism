# Frontend Mentor - Space tourism website solution

This is a solution to the [Space tourism website challenge on Frontend Mentor](https://www.frontendmentor.io/solutions/semantic-html5-markup-css-custom-properties-flexbox-css-grid-js-MG9Ykfje8v). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- View the optimal layout for each of the website's pages depending on their device's screen size
- See hover states for all interactive elements on the page
- View each page and be able to toggle between the tabs to see new information

### Screenshot

![](https://github.com/Daway101/Space-Tourism/blob/main/assets/screenshot/Desktop%20-%20Home.png)
![](https://github.com/Daway101/Space-Tourism/blob/main/assets/screenshot/Mobile%20-%20Menu.png)
![](https://github.com/Daway101/Space-Tourism/blob/main/assets/screenshot/Mobile%20-%20Technology%20-%20A.png)
![](https://github.com/Daway101/Space-Tourism/blob/main/assets/screenshot/Tablet%20-%20Destination%20-%20A.png)

### Links

- Solution URL: [Click here](https://www.frontendmentor.io/solutions/semantic-html5-markup-css-custom-properties-flexbox-css-grid-js-MG9Ykfje8v)
- Live Site URL: [Click here](https://daway101.github.io/Space-Tourism/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Flexbox
- Mobile-first workflow
- JavaScript

### What I learned

I was able to test my HTML, CSS and JavaScript skills by building out a responsive, multi-page site featuring a homepage, buttons, a navigation bar, tabs, keyboard navigation and underline, dot and number indicators. This project helped me get better at using custom properties, variables in CSS, utility classes, resets, responsiveness, CSS logical properties and values using block or inline to describe in which direction they flow. I also got better at adjusting the screen layout(mobile, medium, large screen) using media queries and CSS properties to align items and content. It also helped me practice my Javascript and create an effective design system. Moreover, I was able to build my skills for accessibility to wider web-visitors by practicing using methods like Eventlistener, queryselector, setAttribute.

I really enjoyed learning about these things in particular: 

- How to activate tabs, navigate keyboard and specify tab order. 
- How to Add functionality using JavaScript.

```js
const tabList = document.querySelector('[role="tablist"]');
const tabs = tabList.querySelectorAll('[role="tab"]');

let tabFocus = 0;

tabList.addEventListener('keydown', (e) => {
    const keydownLeft = 37;
    const keydownRight = 39;
    
    // change the tabindex of the current tab to -1
    if (e.keyCode === keydownLeft || e.keyCode === keydownRight) {
        tabs[tabFocus].setAttribute("tabindex", -1);
    }
    
    // if the right key is pushed, move to the next tab on the right
    if (e.keyCode === keydownRight) {
        tabFocus++;
        console.log(tabFocus)
    }
    
    // if the left key is pushed, move to the next tab on the left
    if (e.keyCode === keydownLeft) {
        tabFocus--;
        console.log(tabFocus)
    }
}
```
----

### Continued development

I would definitely like to rebuild this website with react and sass. I would also like to continue using variables and utility classes in my CSS, and progress further with JavaScript, etc



### Useful resources

- [Scrimba](https://www.scrimba.com) - I used this course, and followed all the modules to build this project.
- [Stackoverflow](https://stackoverflow.com/) - This helped me for many issues I have faced during the development of the project.
- [W3Schools](https://www.w3schools.com/) - Same as **Stackoverflow** , this helped me to understand some fundamental things about CSS and JS.
- [MDN Web Docs](https://developer.mozilla.org/en-US/) - Same as **Stackoverflow** , this helped me to understand some fundamental things about CSS and JS.


## Author

- LinkedIn - [Dawa Tsering](https://www.linkedin.com/in/dawatsering/)

## Acknowledgments

This project helped me have a deep understanding of CSS, responsive design and the knowledge to build an interactive site which users will adore using detailed designs in Figma to craft a site which looks amazing on a variety of screen sizes and browsers. Thanks to the course and the very relevant advice of Kevin Powell!
