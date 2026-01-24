# Introduction to HTML, CSS, and JavaScript

## Introduction

The web pages you visit every day are built using three core technologies:
- **HTML**
- **CSS**
- **JavaScript**

Together, these technologies allow developers to create web pages and interactive web applications. This document explains how they work together through two simple examples: a digital clock and a video player.

---

## The Three Core Web Technologies

### HTML (HyperText Markup Language)

HTML is responsible for **structuring content** on a web page.

It defines:
- Text
- Headings
- Buttons
- Images
- Videos

HTML describes *what* content appears on the page.

---

### CSS (Cascading Style Sheets)

CSS controls the **visual appearance** of a web page.

It defines:
- Layout and positioning
- Colors and backgrounds
- Fonts and sizes
- Spacing and alignment

CSS describes *how* the content looks.

---

### JavaScript

JavaScript adds **logic and interactivity** to a web page.

It is used to:
- Update content dynamically
- Respond to user actions
- Control behavior and application logic

JavaScript defines *how the page behaves*.

---

## Example 1: Digital Clock

The first example demonstrates how HTML, CSS, and JavaScript work together to create a **digital clock**.

### HTML File: `clock.html`

- Defines elements for hours, minutes, and seconds
- Displays placeholder values (e.g., `00:00:00`)

Without CSS or JavaScript, the clock appears as plain text with no styling or behavior.

---

### CSS File: `styles.css`

- Styles the clock layout
- Sets font size, color, background, and positioning

The browser retrieves and processes the CSS file to visually format the clock.

---

### JavaScript File: `clock.js`

- Updates the time every second
- Dynamically changes the hour, minute, and second values

JavaScript makes the clock **functional and dynamic**.

---

### Result

With all three files linked together:
- HTML provides structure
- CSS provides style
- JavaScript updates the time continuously

The digital clock works as expected.

---

## Example 2: Interactive Video Player

The second example demonstrates **user interaction** using JavaScript.

---

### HTML File

- Defines the video element
- Defines a Play/Pause button

HTML describes the content visible on the page.

---

### CSS File

- Styles the video player and button
- Controls layout and appearance

The browser applies CSS styling after retrieving the file.

---

### JavaScript File: `videoplayer.js`

The JavaScript code performs the following actions:

1. Registers a click event listener on the button
2. Checks whether the video is currently playing or paused
3. Plays the video and changes the button icon when clicked
4. Pauses the video and updates the button icon when clicked again

---

### Result

- The video is stopped by default
- Clicking **Play** starts the video and updates the icon
- Clicking again pauses the video and restores the play icon

This creates a fully interactive video player.

---

## How HTML, CSS, and JavaScript Work Together

In both examples:
- The **HTML file** references the CSS and JavaScript files
- The **CSS file** styles the application
- The **JavaScript file** controls logic and interactivity

Each technology has a clear responsibility, and together they form complete web applications.

---

## Summary

- HTML structures the content
- CSS styles the content
- JavaScript controls behavior and interaction
- All three are required for modern web development
- Linking these files together enables dynamic and interactive websites

Understanding how HTML, CSS, and JavaScript work together is a fundamental step in becoming a web developer.
