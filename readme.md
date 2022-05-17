# Frontend Mentor - QR code component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
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

This goal of this project is to develop a simple webpage having a NFT preview card component and styling it.


### Screenshot

[screenshot of cloned webpage](img/screenshot.png)


### Links

- Live Site URL: [Live site URL](https://itachidorri.github.io/nft-preview-card-component/)

## My process
1. Building the html structure for the project.
2. Adding CSS to the project.
3. Finding solution to errors on resources such as google,'w3schools' etc.
4. Implementing solutions.


### Built with

- Semantic HTML5 markup
- CSS properties
- [Google Fonts](https://fonts.google.com/) - For fonts


### What I learned

Styling page cleverly using CSS properties:
1. border - creating visible border on the side of stacked divisions only to give them a split look.

2. floats & clears - These helped to stack HTML divisions horizontally.

```html
<div class="card-footer">
  <img class="pp" src="img/image-avatar.png" alt="profile picture">
  <p class="creator-name ">Creation of <span class="hover">Jules Wyvern</span></p>
</div>
```

```css
.pp{
  height: 25px;
  width: 25px;
  float: left;
  border-radius: 50px;
  border: 1px solid white;
}

.creator-name{
  float: left;
  padding-left: 10px;
  font-size: 13px;
  margin-top: 5px;
}
```
Here, using float the two divisions are stacked horizontally.
Check [screenshot](img/float-eg.jpg)


3. Making image appear when hovered on something - Main properties used in this feature were 'position ', 'transition' & 'opacity' properties

```html
<div class="picture">
  <img class="coin" src="img/image-equilibrium.jpg" alt="cube shape equillibrium coin">
  <div class="overlay">
    <img class="view" src="img/view.png" alt="view icon">
  </div>
</div>
```

```css
.overlay{
  position: absolute;
  top: 0;
  bottom: 0;
  left: 0;
  right: 0;
  height: 100%;
  width: 100%;
  opacity: 0;
  transition: .5s ease;
  background-color: rgb(104, 231, 247);
  border-radius: 5%;
}

.picture:hover .overlay{
  opacity: .5;
}
```
Here, to create such effect, a new division is created alongside the '<img class="coin">'. An image is also added to the new '<div>'. However, it is kept hidden unless a mouse is hovered over it.


4. Utility classes - In short, these are such classes that can be used many times. An example is as follows:

```CSS
.hover:hover{
  color: rgb(104, 231, 247);
}
```

Here, the class 'hover' can be used on any portion of the webpage as per user's want.


### Continued development

To gain proper understanding of making an image appear when hovered on something.


### Useful resources

- [Google fonts](https://fonts.google.com/specimen/Outfit) - This helped to use a variety of fonts to beautify a website.

- [W3 schools](https://www.w3schools.com) - A nice website to learn bothe basic & clever 'HTML' & 'CSS' tricks.


## Author

- Frontend Mentor - [@Itachidorri](https://www.frontendmentor.io/profile/Itachidorri)
- Github - [Itachidorri](https://github.com/Itachidorri)


## Acknowledgments

I am grateful to the developers of 'front-end mentor' to make projects available for a newbie learner. Also, I want to thank 'w3 schools' for providing such helpful resources to make further progress as a web developer. Hare Krishna!
