# Frontend Mentor - Ricky's 'Testimonials Grid Section' Solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7).

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

I was very confident going into this project, thanks to Dr. Angela, Developer and Lead Instructor. Also, thanks to Codepips for providing a super helpful game called "CSS Grid Garden." Both of these resources led to my success in completing this project. 

Leading up to this CSS Grid project, I planned my execution ahead of time by looking at the example designs provided. I didn't download the Figma file, so I eyeballed the overall size. 

The main rule that I used within the CSS Grid is the 

grid-template-columns and grid-template-rows for my .card-grid

..And...

grid-area, grid-column, and grid-row for the 
.grid-items. 

Overall, the execution was better than I anticipated, but I think I could have done a better job sizing the paragraphs and headers and being clearer about group naming my tags for easier targeting. 

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size

### Screenshot

<img src="./design/my desktop testimonial cards.png"/>
<img src="./design/testimonial card 1050 mq.png"/>
<img src="./design/testimonial card 780 mq.png"/>
<img src="./design/testimonial card 700 mq.png"/>
<img src="./design/testimonial card 375 mq.png"/>


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

HTML:

My process started by creating my containers and all the boxes: 

```html
<main class="container">
 <article class="card-grid">
 <section class="grid-items daniel">
 </section>
 </article>
</main>
```
...within the section, I set up my cards:
```html
 <img class="img" src="" alt="">
 <header>
 <h4></h4>
 <p></p>
 </header>
 <div class="testimony-container">
 <h2 class="opening-statement"></h2>
 <p class="comment"></p>
 </div>
```
...my name setup was after all the names to make it easier to recall and to know exactly what position they're in. 

===

After all the details were added within the five cards, I proceeded to add all its features--

My CSS Grid styling began with:
```css
.card-grid {
 max-width: 1050px;
 display: grid;
 grid-template-rows: 1fr 1fr 1fr 1fr;
 grid-template-columns: 1fr 1fr 1fr 1fr;
 gap: 20px;
 margin-top: 150px; 
```
...this set up was east to implement since all I used were rows and columns spans:
```css
.daniel {
 background-image: url(./images/bg-pattern-quotation.svg);
 background-repeat: no-repeat;
 background-position: 82% -2%;
 background-color: hsl(263, 55%, 52%);
 color: hsl(0, 0%, 100%);
 grid-column: span 2;
 padding: 30px;
}


.kira {
 background-color: hsl(0, 0%, 100%);
 color: hsl(217, 19%, 35%);;
 grid-row: span 2;
 padding: 36px;
}


.patrick {
 background-color: hsl(219, 29%, 14%);
 color: hsl(0, 0%, 81%);
 grid-column: span 2;
 padding: 36px;
 box-shadow: 10px 50px 40px hsl(217, 16%, 72%);
}

```
...I didn't need to add a specific placement to 
.jeanette and .jonathan, because these sizing was smaller and all the other items took up all the spaces. So they technically positioned themselves into the avaliable slots. 

After my positioning, I added four media queries:

--1080px
--780px
--700px
--375px

...if you take a closer look at the 780px and the 700px. What I intended in the transitioning here was to give the .kira card more space since it was becoming too vertical (reading this would be a hassle). To fix this, I just switched the placement of the two smallest cards (.jonathan and .jeanette) to the outside, giving the .kira card the left horizontal space. 

### Built with

- Semantic HTML5 markup
- Flexbox
- CSS Grid
- Desktop-first workflow

### What I learned

I learned a little bit more about media queries combined with CSS Grid. I have never actually worked that much with media queries, but using a lot more, I can see the benefits.

I've also used the background-image: url(); I haven't use this as much, but the 'Order Summary' project was my first time in a long time, so using it again in this project helped me understand it better

### Continued development

Going to continue working on my CSS Grid and Flexbox, mainly focusing my attention to responsive design.

### Useful resources


## Author

--Website: (https://www.rarroyoharo.com)<a href="https://www.rarroyoharo.com" target="_blank">rarroyoharo.com</a> 
--Frontend Mentor - [@RiickyRiick]<a href="https://www.frontendmentor.io/profile/RiickyRiick" target="_blank">@RiickyRiick</a> 


## Acknowledgments

<a href="https://www.udemy.com/course/the-complete-web-development-bootcamp/
" target="_blank">Dr. Angela's Complete Web Developing Bootcamp/a> 

<a href="https://www.udemy.com/course/the-complete-web-development-bootcamp/?couponCode=ST7MT290425G3#instructor-1" target="_blank">Dr. Angela's Profile</a>


