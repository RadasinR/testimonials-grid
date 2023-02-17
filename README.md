# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout for the site depending on their device's screen size

### Screenshot

![](./screenshot.png)


### Links

- Solution URL: [Add solution URL here](https://github.com/RadasinR/testimonials-grid.git)
- Live Site URL: [Add live site URL here](https://testimonials-grid-ashy.vercel.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

### Structure
  Having readeable code is important becuase it will be more read then writen. For code to be readeable and understandable it has to be
  well structured and meanigfull. To achive that i used html elements with semantic meaning and i give meanigfull names to the classes.
### Layout
  Setting the grid layout of the page with html can be done with table elements, but its very hard to read and write, so i used CSS Grid for that.
```html
 <article class="testimonial bg-purple">
      <header class="user">
        <img class="accent" src="/images/image-daniel.jpg" alt="user picture" width="34" height="34">
        <div>
          <p class="user__name">Daniel Clifford</p>
          <p class="verification">Verified Graduate</p>
        </div>
      </header>
      <h1 class="testimonial__title">
        I received a job offer mid-course, and the subjects I learned were current, if not more so,
        in the company I joined. I honestly feel I got every penny’s worth.
      </h1>
      <p class="testimonial__text">

        “ I was an EMT for many years before I joined the bootcamp. I’ve been looking to make a
        transition and have heard some people who had an amazing experience here. I signed up
        for the free intro course and found it incredibly fun! I enrolled shortly thereafter.
        The next 12 weeks was the best - and most grueling - time of my life. Since completing
        the course, I’ve successfully switched careers, working as a Software Engineer at a VR startup. ”
      </p>
    </article>
```
```css
grid {
        grid-template-columns: 1fr 1fr 1fr 1fr;
        padding: 10% 10%;
    }

    .testimonial:first-child {
        grid-column-start: 1;
        grid-column-end: 3;
    }

    .testimonial:nth-child(4) {
        grid-column-start: 2;
        grid-column-end: 4;
    }
    .testimonial:nth-child(5) {
        grid-column: 4;
        grid-row: 1 / 3;
    }
}
```

### Continued development

### Useful resources

- [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout) - how to use css grid.

## Author


- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/Radasin)

