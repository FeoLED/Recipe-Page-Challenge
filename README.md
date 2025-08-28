# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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


## Overview

### Screenshot

![](assets/computer_view.png)


### Links

- Solution URL: ![GitHub repo]((https://github.com/FeoLED/Recipe-Page-Challenge )
- Live Site URL: ![GitHub Pages Site](https://feoled.github.io/Recipe-Page-Challenge/)

## My process

### Built with

- Semantic HTML5 markup
- Flexbox
- Mobile-first workflow
- Fonts served by Bunny Fonts 


### What I learned

While working on this, I got to experiment with the calc() function. A few days before starting this project, I learned about various CSS functions, and I tried to apply
what I learned. I have to say is very convenient for responsive design. For example, for screens over 900px wide, I applied the following to the main element:

```css
.main{
    width:calc(1vh*40);
}
```
This allows the element to adapt to the size of the screen or browser window.

Another thing I learned, or more like "revisited" was the position property. While working on the mobile layout, I had to exempt the image (img) element from
the padding from its main parent. I tried different approaches, from changing the width (which worked somewhat) to playing with negative margins and padding.
The final solution was to apply  position: relative; to both the main and the img element. I then changed the image's width to account for the padding on its parent container:

```css
.picture{
    width: calc(100% + 2em);
    position: relative;
    border-radius: 0px;
}
```
There were other changes related to the main element's width, padding, and other elements, all focused on the mobile layout. I used @media queries to apply the changes. 


### Continued development

I want to point out how useful the calc() function is, and how cumbersome it was to find the proper solution for the image in the mobile layout. Even if it worked, I'm not quite 
familiar with positioning. I'll try to apply more of these techniques in the future. 

*(A small aside: While the solution worked, I found the process of using positioning to be unintuitive. It's an area I look forward to understanding better in future projects.)*

### Useful resources

- [This question on Stack Overflow](https://stackoverflow.com/questions/64665752/how-to-get-image-to-ignore-parent-div-padding) - Here they discuss a similar problem... I experimented with different values until I got the result I wanted, which is a good approach to get the hang of these CSS concepts.

## Author

- Website - [FeoLED](https://github.com/FeoLED)
- Frontend Mentor - [@FeoLED](https://www.frontendmentor.io/profile/FeoLED)
