# Frontend Mentor - Mortgage repayment calculator solution

This is a solution to the [Mortgage repayment calculator challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/mortgage-repayment-calculator-Galx1LXK73). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

### The challenge

Users should be able to:

- Input mortgage information and see monthly repayment and total repayment amounts after submitting the form
- See form validation messages if any field is incomplete
- Complete the form only using their keyboard
- View the optimal layout for the interface depending on their device's screen size
- See hover and focus states for all interactive elements on the page

### Screenshot

Desktop:
![Desktop initial state](/Desktop-init-state.png)

![Desktop error state](/Desktop-error-state.png)

![Desktop completed calculation](/Desktop-completed-state.png)

Tablet:

![Tablet initial state](/Tablet-init-state.png)

Mobile:

![Mobile initial state](/Mobile-init-state.png)

### Links

-   [Live Site URL](https://mrtg-calculator-ianwilk20.netlify.app/design/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow


### What I learned

Early on I was faced with the problem of how to format the monthly payment or total repayment so that it would have commas where they are commonly put in monetary amounts. I knew there were functions to do this like .toLocaleString() or a .replace() regex expression could be used, but I guess I wanted a bit of a challenge. So I broke apart the problem into it's most fundamental parts, tried lots of things that didn't work and eventually led me to learn how to format any monetary amount.

I was having trouble figuring out how to group the two radio buttons so that when one is selected the other one cannot be selected. I came across the fieldset element which allows for the grouping of input elements, and in the case of radio buttons it makes it so only one option is selectable at a time.

Another learning, concerning the "Clear All" button, was that the onclick would call the clearInputs function which called the reset function on the form. It would reset the form's inputs, but it would trigger the form's submit event listener. This stumped me for a while until I learned that my Clear All button was likely being treated as a submit button for the form. I fixed this by specifying the button to have a ```type="button"```.

### Continued development

This challenge taught me some basic concepts about HTML/JS forms. I look forward to learning more in this area since forms are everywhere and I've only scratched the surface.

### Useful resources

- [HTML <fieldset> tag](https://www.w3schools.com/tags/tag_fieldset.asp) - This helped me for understand how to use fieldsets for form input elements.
- [Mortage Formulas](https://www.businessinsider.com/personal-finance/mortgages/mortgage-calculator) - I used the formula from this website to figure out how to calculate mortgage repayments and interest.

## Author

-   GitHub - [ianwilk20](https://github.com/ianwilk20)