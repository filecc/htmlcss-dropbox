# Boolean Academy - Dropbox Landing Page
This is a solution to the exercice of - Classe #92 - 13 Febbraio 2023.


## Table of contents

- [Overview](#overview)
  - [The exercice](#the-exercice)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)


## Overview

### The exercice

Students should be able to:

- View the optimal layout for the website using CSS Flexbox and Position (Absolute and Relative)

### Screenshot
Below is how the page should looks like

![Page](./screenshot.png)


### Links

- Solution URL: [https://github.com/filecc/htmlcss-dropbox](https://github.com/filecc/htmlcss-dropbox)
- Live Site URL: [https://filecc.github.io/htmlcss-dropbox/](https://filecc.github.io/htmlcss-dropbox/)

## My process

### What I learned
CSS for anchor tag in navbar with background on hover

```css
.topnav a {
    transition: all linear .3s;
    float: left;
    display: block;
    text-align: center;
    padding: 14px 16px;
    border-bottom: 3px solid transparent;
}
.topnav a:hover {
    background-color: var(--primary);
    color: white;
}
```

custom checkmark

```css
.checkmark {
    position: absolute;
    top: 0;
    left: 0;
    height: 24px;
    width: 24px;
    background-color: #eeeeee;
    border-radius: 50%;
}
input:checked~.checkmark {
    background-color: var(--primary);
}
input:checked~.checkmark:after {
    display: block;
}
.checkmark:after {
    content: "";
    position: absolute;
    display: none;
    top: 5px;
    left: 5px;
    padding: 7px;
    border-radius: 50%;
    background: white;
}
```
Thank to @GiuseppeIndomenico for this idea: just set a box shadow inset white with 50% transparency on hover, instaed of manually set every different color for every square. 

```css
:is(.designit, .asu, .uf, .topps, .center, .wbr, .lonley, .hearst, .clear):hover{
    box-shadow: inset 0 0 0 15px  #ffffff74;
}
```

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox



