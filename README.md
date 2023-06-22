# Make It Real - NAME OF THE PROJECT

This is a solution to the HTML-1 project of the Make It Real course.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)


## Overview

### The challenge

#### Users should be able to:

Build a responsive 404 page and make it look as much like the design as possible.
You can use any tool you like to help you complete the challenge. So, if you have something you'd like to practice, feel free to give it a try.
Your users should be able to:

See the optimal design according to the screen size of their device.

### Screenshot

Desktop
![Desktop](./screenshots/Screen%20Shot%202023-06-20%20at%208.53.15%20PM.png)

Mobile
![Mobile 1](./screenshots/Screen%20Shot%202023-06-20%20at%208.56.37%20PM.png)
![Mobile 2](./screenshots/Screen%20Shot%202023-06-20%20at%208.55.48%20PM.png)


## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first design strategy

### What I learned

1. I've learned how to layout UIs using flexbox, it's an easy way to set element in the expected place.

```html
<div class="container">
  <h1>This is a centered title</h1>
</div>
```
```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

```html
<main class="container">
  <section class="image-container">
    <img src="img/scarecrow.png" alt="Scarecrow" aria-label="Page Not Found Image" />
  </section>
  <section class="message-container">
    <h2 class="not-found-subtitle">
      I have bad news for you
    </h2>
    <p class="not-found-message">
      The page you are looking for might be removed or is temporarily unavailable
    </p>
    <a class="back-to-home__button" href="#">BACK TO HOMEPAGE</a>
  </section>
</main>
```
```css
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
```

2. I've learned Responsive Design, it lets us apply styles to elements on specific resolutions and using the Mobile First strategy make it easier this process.

```html
<main class="container">
  <section class="image-container">
    <img src="img/scarecrow.png" alt="Scarecrow" aria-label="Page Not Found Image" />
  </section>
  <section class="message-container">
    <h2 class="not-found-subtitle">
      I have bad news for you
    </h2>
    <p class="not-found-message">
      The page you are looking for might be removed or is temporarily unavailable
    </p>
    <a class="back-to-home__button" href="#">BACK TO HOMEPAGE</a>
  </section>
</main>
```
```css
.container {
  display: flex;
  flex-direction: column;
  align-items: center;
}

/** Desktop **/
@media (min-width: 768px) {
  .container {
    flex-direction: row;
    justify-content: center;
  }
}
```


### Continued development

There are some concept that I would like to learn and to know deeper such as:

- BEM (Naming convention)
- Specificity
- Flexbox
- CSS Grid
- Semantic HTML

### Useful resources

- [CSS Flexbox Course](https://app.ed.team/cursos/flexbox-grid/) - This is a good Flexbox and CSS Grid course.
- [Flexbox Froggy](https://flexboxfroggy.com/#es) - This is a fun game that let you practice Flexbox.

## Author

- LinkedIn - [Andry Peña](https://www.linkedin.com/in/andrystylist/)
- Twitter - [@andrystylist](https://www.twitter.com/andrystylist)


## Acknowledgments

I haven't tried to only solve the challenge but apply best practices and techniques that make your code more readable and maintainable through the time.