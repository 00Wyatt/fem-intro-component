# Frontend Mentor - Intro component with sign up form solution

This is a solution to the [Intro component with sign up form challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/intro-component-with-signup-form-5cf91bd49edda32581d28fd1). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout for the site depending on their device's screen size
- See hover states for all interactive elements on the page
- Receive an error message when the `form` is submitted if:
  - Any `input` field is empty. The message for this error should say *"[Field Name] cannot be empty"*
  - The email address is not formatted correctly (i.e. a correct email address should have this structure: `name@host.tld`). The message for this error should say *"Looks like this is not an email"*

### Screenshot

![Intro Component with Sign Up Form](./images/screenshot-intro-component-with-sign-up-form.png)

### Links

- Solution URL: [Sign-up Form using Client-side JavaScript Validation](https://www.frontendmentor.io/solutions/signup-form-using-clientside-javascript-validation-cMO8I-udNo)
- Live Site URL: [Frontend Mentor | Intro component with sign up form](https://00wyatt.github.io/fem-intro-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Mobile-first workflow

### What I learned

This was a great exercise for using Javascript to create basic client-side form validation. I hadn't done enough of it before to really know what I was doing, but after the research I did to complete this challenge, I have a better understanding of what's possible and what's necessary.

The Javascript was the main challenge for me, I had to do a bit of reading to understand what to do. If anybody has a suggestion about how to improve, please let me know.

I tried to create seperate reusable functions to make the code as clean as I could. I wanted to compact it down as much as possible, but still make sure it's easy to understand.

I was happy with the function I ended up using for handling and displaying the form errors:

```js
const diplayError = (input, message) => {
    const errorMessage = input.nextElementSibling;
    errorMessage.innerText = message;
    if (message) {
        input.classList.add('show-error');
    } else {
        input.classList.remove('show-error');
    }
}
```

I had to learn from example to write a lot of the Javascript, and then made my own adjustments.

If anyone has feedback, please let me know.

### Continued development

I want to keep working on my Javascript skills, I find it harder than the styling and markup. I want to be competent in all three as soon as possible. I'll look for more Frontend Mentor Challenges involving JS.

### Useful resources

- [Form validation using javascript](https://dev.to/javascriptacademy/form-validation-using-javascript-34je) - This first article, written by Adam Nagy, is what I started learning from for form validation using JS, before I tried using the Constraint Validation API.
- [Form Validation Using JavaScript's Constraint Validation API](https://blog.openreplay.com/form-validation-using-javascript-s-constraint-validation-api) - This was a helpful article by Craig Buckler, that I referred to during this challenge.
- [Constraint validation](https://web.dev/constraintvalidation/) - Another good article on Constaint Validation, by TJ VanToll.

## Author

- Frontend Mentor - [@00Wyatt](https://www.frontendmentor.io/profile/00Wyatt)

## Acknowledgments

I also got a bit of inspiration for the Javascript from @TahoeBoelat's solution - [Sign up intro solution challenge](https://www.frontendmentor.io/solutions/sign-up-intro-solution-challenge-KhP05j3EMj)
This is how I got onto the path of using the Constraint Validation API.