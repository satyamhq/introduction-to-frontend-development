# Working with Libraries

Imagine you want to cook a dish you’ve never tried before. You could experiment with ingredients and cooking times, or you could simply follow a recipe. In a similar way, as a developer, you can build everything from scratch—or you can use **libraries** created by other developers.

Libraries help you build websites faster by providing reusable code for common features.

---

## What Are Libraries?

Libraries are collections of prewritten code that expose **APIs** you can use in your application. Your code interacts with these APIs to add functionality such as layouts, buttons, animations, or interactive behavior.

Because your application relies on this external code, libraries are often referred to as **dependencies**.

---

## What Are Dependencies?

A **dependency** is code that your application depends on to work correctly.

If you do not include required libraries:

* Your application cannot call the APIs it needs
* Features may fail or not load at all

On the front end, dependencies are usually included by referencing **CSS** and **JavaScript** files in your HTML.

---

## Including a CSS Library

One popular UI library is **Bootstrap**, which provides prebuilt styles and components.

To include a CSS library, add a `<link>` tag inside the `<head>` element.

### Example: Adding a CSS Library

```html
<head>
  <link rel="stylesheet" href="bootstrap.css">
</head>
```

* `rel="stylesheet"` tells the browser this is a CSS file
* `href` specifies the location of the library

---

## Including a JavaScript Library

Some libraries also provide JavaScript files that enable interactive features such as:

* Dropdown menus
* Tooltips
* Modals

JavaScript libraries are included using the `<script>` tag, usually near the end of the `<body>` element.

### Example: Adding a JavaScript Library

```html
<body>
  <script src="bootstrap.js"></script>
</body>
```

The `src` attribute specifies the location of the JavaScript file.

---

## Using a Library Feature

Once the library is included, you can start using its features.

### Example: Bootstrap Button

```html
<button type="button" class="btn btn-primary">
  Click this button
</button>
```

This creates a styled button using Bootstrap’s built-in classes.

---

## Dependency Trees

Sometimes a library depends on **other libraries**. This creates a **dependency tree**.

A project can have:

* Dozens or hundreds of dependencies
* Multiple layers of dependencies

Managing these manually would be time-consuming and error-prone.

---

## Package Managers

A **package manager** automates the process of:

* Downloading dependencies
* Installing correct versions
* Managing dependency trees

Dependencies are often referred to as **packages**.

The most common package manager for front-end development is **npm (Node Package Manager)**.

Package managers ensure:

* Everyone uses the same dependency versions
* Dependencies are installed consistently
* Dependency conflicts are avoided

---

## Bundlers

Once dependencies are installed, adding every file manually to your HTML would be inefficient.

This is where **bundlers** are used.

A **bundler**:

* Combines multiple dependency files into one (or a few) files
* Improves performance
* Simplifies HTML setup

Popular bundling tools include:

* Webpack
* Gulp

Large applications may split dependencies into multiple bundles for better loading performance 

---

## Key Takeaways

* Libraries provide reusable functionality
* Applications depend on libraries to work correctly
* Dependencies must be included in HTML files
* CSS uses `<link>`, JavaScript uses `<script>`
* Dependency trees can be complex
* Package managers automate dependency handling
* Bundlers combine dependencies into optimized files

Using libraries allows developers to build faster, more reliable, and more feature-rich websites 
