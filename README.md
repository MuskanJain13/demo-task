
## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge
Users should be able to:

- View the optimal layout for the app depending on their device's screen size
- See hover states for all interactive elements on the page
- Generate a new piece of advice by clicking the dice icon

### Screenshot

![](https://github.com/MuskanJain13/demo-task/blob/main/Screenshot-1%20Demo%20Task.png)
![](https://github.com/MuskanJain13/demo-task/blob/main/Screenshot-2%20Demo%20Task%20Hover.png)
![](https://github.com/MuskanJain13/demo-task/blob/main/Screenshot-3%20Demo%20Task%20Mobile.png)

### Links

- Solution URL: [https://github.com/MuskanJain13/demo-task](https://github.com/MuskanJain13/demo-task)
- Live Site URL: [https://demo-task.vercel.app/](https://demo-task.vercel.app/)

## My process

So, I started with studying the design which I got in the challenge. Then I figured out how the structure would be created, i.e., how many divisions would be there, and what will come first. Then I started creating the outer structure and followed by the inner structure. Then, added sample styles to it, to see how close it was getting. Then I took each element in the design and started working on it precisely to get more precise results, and once an element was completed, I switched to the next one. Then, I started working on the API part to fetch data and display it. Once, it was completed I started with adding the final styles to the whole project. And this is how, I came more closer to the desired result.

### Built with

- HTML5
- CSS3
- Flexbox
- JavaScript

### What I learned

Some new things which I learned through this project are fetching data from API using "JavaScript". And shadow in the particular way as used here. And I struggled in placing elements in center with respect to each other. So, somehow after some hit and trials and figured it out.

```html
<div class="center">
    <div id="dice-shape" class="center" onclick="display()">
        <img src="assets/icon-dice.svg" alt="dice">
    </div>
</div>
```
```css
#dice-shape:hover{
    box-shadow: 0px 0px 30px 2px hsl(150, 100%, 66%);
}
```
```js
console.log(data.slip.advice);
var advice = data.slip.advice;
var id = data.slip.id;
// Changing the advice text in HTML div
document.getElementById('advice-body').innerHTML = '&ldquo;'+advice+'&rdquo;';
document.getElementById('advice-title').innerHTML = 'ADVICE #'+id;
```

### Few Useful resources

- [Example resource 1](https://www.geeksforgeeks.org/how-to-use-the-javascript-fetch-api-to-get-data/?ref=lbp) - This helped me for fetching the data from API using JavaScript. Previously, I have worked with PHP while working web projects, so I didn't knew how to fetch the data using JavaScript. So, with the help of this resource, I got a base for how to use JavaScript and I tried to apply their steps in my project, to complete the purpose. After few hit and tries and I understood the use of that code, and implemented the same in this project.

- [Example resource 2](https://www.w3schools.com/howto/howto_js_media_queries.asp) - This resource helped me understand using media queries with JavaScript.

## Author

- LinkedIn - [Muskan Jain](https://www.linkedin.com/in/muskan-jain13/)

## Acknowledgments

I took references from Internet wherever I felt to, at places, for knowing a trick for centering a HTML div or whenever I was stuck in the code, and to exploring the new concepts, which were necessary to complete this project.
