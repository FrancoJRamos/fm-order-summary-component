# Frontend Mentor - Order summary card solution

This is a solution to the [Order summary card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- See hover states for interactive elements

### Screenshot

![](./screenshot.jpg)

Add a screenshot of your solution. The easiest way to do this is to use Firefox to view your project, right-click the page and select "Take a Screenshot". You can choose either a full-height screenshot or a cropped one based on how long the page is. If it's very long, it might be best to crop it.

Alternatively, you can use a tool like [FireShot](https://getfireshot.com/) to take the screenshot. FireShot has a free option, so you don't need to purchase it. 

Then crop/optimize/edit your image however you like, add it to your project, and update the file path in the image above.

**Note: Delete this note and the paragraphs above when you add your screenshot. If you prefer not to add a screenshot, feel free to remove this entire section.**

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://francojramos.github.io/fm-order-summary-component/)

## My process

Day 1 07/13/22
  •Implemented Semantic HTML Structuring

  Notes for consideration: 
    The main changes between screen views is the background image and the size of the box.

Day 2 07/25/22
  Worked on: 
  •formating Semantic HTML Structures - editing spacing and color
  •Media Queries

  Notes for consideration:
    •Media Queries have been implemented and are cropped once the browser width reaches ~1200px but is not smooth

    •When formatting the 'plan-summary' div use grid format and seperate the elements into 3 different divs: 1 for the icon, 1 for the annual plan & price text and 1 for the change icon

    **REMINDER** the order of this 'plan-summary' element will not change, but the width of its cells could

    •Revisit the Media Queries rules - should the mobile view extend until 1440px? then enter desktop?

Day 3 07/26/22
  Worked on:
  •getting the page to look on model with the drafts given via spacing and matching font weights
  •Implementing a grid structure for the 'plan-summary' div

  Notes for Consideration:
    •Still haven't revisited the Media Query
    •Still need to play with the background image

Day 4 08/04/22
  Worked on:
  •improving how media queries are implemented to give a consistent view between mobile, tablet and desktop
  •Implementing hover actions on interactive elements that create feedback for the user
  •Improved the display of the background-image

  Notes for Consideration
    •At the end of the project, here a some things that I was constantly reading the documentation of to make sure I was using correctly:
      •background-size and its values
      •the definition of a vh unit
      •border-radius and its values
      •display:grid, its values and how their are used between the parent container and its child elements
    •At the end of the project, here are some new pieces of code that I picked up on
      •vh (value)
      •:root (selector)
      •defining variables for color (rules)


### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow
- [React](https://reactjs.org/) - JS library
- [Next.js](https://nextjs.org/) - React framework
- [Styled Components](https://styled-components.com/) - For styles

**Note: These are just examples. Delete this note and replace the list above with your own choices**

### What I learned

Use this section to recap over some of your major learnings while working through this project. Writing these out and providing code samples of areas you want to highlight is a great way to reinforce your own knowledge.

W.I.L. #1
  Dealing with matching border radius' between images and their divs
On previous attempts, I've tried finding a way to use css object-fit and background-fit rules to try and crop an image so that it doens't exceed its parent containers. But when a border radius is implemented the img shoots past the border of its parent div - therefore, by implementing the border-top-xx-radius rules I can match the border-radius between an image and its parent container
```html
<section class="order-card">
  <div class="image-header">
      <img src="images/illustration-hero.svg" alt="Illustration">
  </div>
</section>
```
```css
.order-card
{
    border-radius:25px;
}
.image-header img
{
    border-top-left-radius: 25px;
    border-top-right-radius: 25px;
}
```

If you want more help with writing markdown, we'd recommend checking out [The Markdown Guide](https://www.markdownguide.org/) to learn more.

**Note: Delete this note and the content within this section and replace with your own learnings.**

### Continued development

Use this section to outline areas that you want to continue focusing on in future projects. These could be concepts you're still not completely comfortable with or techniques you found useful that you want to refine and perfect.

**Note: Delete this note and the content within this section and replace with your own plans for continued development.**

### Useful resources

- [Setting footer at bottom](https://dev.to/nehalahmadkhan/how-to-make-footer-stick-to-bottom-of-web-page-3i14) - Looked for a simple method to set the footer to the bottom and the resource was straight to the point, I had even used some of its formatting in my own solution to organizing the elements and it fit in great.
- [Example resource 2](https://www.example.com) - This is an amazing article which helped me finally understand XYZ. I'd recommend it to anyone still learning this concept.

**Note: Delete this note and replace the list above with resources that helped you during the challenge. These could come in handy for anyone viewing your solution or for yourself when you look back on this project in the future.**

## Author

- Website - [Add your name here](https://www.your-site.com)
- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/yourusername)
- Twitter - [@yourusername](https://www.twitter.com/yourusername)

**Note: Delete this note and add/remove/edit lines above based on what links you'd like to share.**

## Acknowledgments

This is where you can give a hat tip to anyone who helped you out on this project. Perhaps you worked in a team or got some inspiration from someone else's solution. This is the perfect place to give them some credit.

**Note: Delete this note and edit this section's content as necessary. If you completed this challenge by yourself, feel free to delete this section entirely.**
