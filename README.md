# Frontend Mentor - News homepage solution

This is a solution to the [News homepage challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/news-homepage-H6SWTa1MFl). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page
- **Bonus**: Toggle the mobile menu (requires some JavaScript)

### Screenshot

![](./screenshot.jpg)


### Links

- Solution URL: [Add solution URL here](https://github.com/vlpreddy/frontend-mentor-challenge-1)
- Live Site URL: [Add live site URL here](https://vlpreddy.github.io/frontend-mentor-challenge-1/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS preprossessor Saas
- Flexbox
- CSS Grid
- Mobile-first workflow


### What I learned

Using combination of both cssgrid and flxbox, and some resolutions dealing the height issues with less content div. And i did some experiment with CSS transition and input type checkbix to avoid using javascript to build a burger menu.

To see how you can add code snippets, see below:

```html
<input type="checkbox" id="check" hidden  class="checkbox">
<div class="hamburger_icon">
  <label for="check" class="burger">
    <div class="burger-line burger-line-1"></div>
    <div class="burger-line burger-line-2"></div>
    <div class="burger-line burger-line-3"></div>
</label>
</div>
```
```css
 .hamburger_icon{
                    width: 40px;
                    height: 40px;
                    position: absolute;
                    right:0px;
                    top:10px;
                    display:block;
                    z-index: 45;
            
                }

                .burger{
                    display:flex;
                    flex-direction: column;
                    justify-content: space-around;
                    cursor: pointer;
                    height: inherit;
                    transition: transform .5s;
    
                    &-line{
                        width:100%;
                        height:4px;
                        background-color:#000000;
                        transform-origin: right;
                        transition: all .5s .5s;
                    }
                }

                .checkbox:checked ~ nav{
                    right:0;
                }
```


### Continued development

I wan to improve writing mixins for clean clode especially when I am using media queres.


### Useful resources

- [Example resource 1](https://www.udemy.com) - I have lisned few topics in different courses helped me tp upgrade my csss skillset.



## Author

- Website - [Leela Parameswara Reddy](https://www.vlpreddy.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@vlpreddy](https://www.twitter.com/vlpreddy)


## Acknowledgments

