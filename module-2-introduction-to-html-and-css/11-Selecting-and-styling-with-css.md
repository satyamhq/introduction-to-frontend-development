# Selecting and Styling with CSS

Think about a physical building—its structure, interior, exterior, and decorations. In a similar way:

* **HTML** is the frame and structure of a website
* **CSS** is the paint, wallpaper, fixtures, artwork, and overall look and feel

In simple terms, **CSS tells the web browser how to display HTML elements on the screen**.

---

## What Is CSS?

CSS stands for **Cascading Style Sheets**. It is used to control:

* Colors
* Fonts
* Layout
* Spacing
* Overall visual appearance

---

## The Structure of a CSS Rule

A CSS rule is made up of **five key parts**:

1. Selector
2. Declaration block
3. Property
4. Value
5. Semicolon

---

## Declaration Block

A **declaration block** starts with an opening curly brace `{` and ends with a closing curly brace `}`.

Inside the declaration block are one or more **style declarations**.

```css
h1 {
  color: gray;
}
```

---

## Selectors

The **selector** defines **which HTML element or elements** the CSS rule applies to.

### HTML Type Selector

This selector targets all elements of a specific type.

```css
h1 {
  color: gray;
}
```

* `h1` → selector
* `color` → property
* `gray` → value

This rule changes the text color of **all `<h1>` elements**.

---

## Properties and Values

Each declaration inside a block consists of:

* A **property** (what you want to change)
* A **value** (what you want to change it to)

Example:

```css
h1 {
  color: blue;
  background-color: gray;
}
```

This results in:

* Blue text
* Gray background

for all `<h1>` elements.

---

## Creating and Linking a CSS File

To apply CSS to an HTML file, you must link a stylesheet.

### Step 1: Create Files

* `index.html`
* `style.css`

### Step 2: Link the CSS File

Add the `<link>` tag inside the `<head>` section of your HTML file.

```html
<link rel="stylesheet" href="style.css">
```

* `rel` specifies the relationship (stylesheet)
* `href` specifies the file name

---

## Applying CSS Rules

### Example: Styling All `<h1>` Elements

```css
h1 {
  color: purple;
}
```

This applies the style to **every `<h1>` on the page**.

---

## Styling a Single Element with an ID

To style only one element, use an **ID selector**.

### HTML

```html
<h1 id="header-one">Chapter One</h1>
```

### CSS

```css
#header-one {
  color: green;
}
```

* `#` indicates an ID selector
* This rule applies only to the element with that ID

---

## CSS Specificity and Precedence

You may notice that the ID rule overrides the type selector.

This happens because of **CSS specificity**:

* More specific selectors take precedence
* ID selectors are more specific than type selectors

In this case:

* `#header-one` overrides `h1`

The browser always applies the **most precise rule**.

---

## Live Preview Tip (VS Code)

You can speed up your workflow by using the **Live Preview** extension in Visual Studio Code.

### How It Helps

* View changes instantly
* No need to refresh the browser
* Faster feedback while styling

Once installed:

* Right-click the HTML file
* Select **Live Preview: Show Preview**

---

## Recap

* CSS controls how HTML elements look
* A CSS rule includes a selector and declaration block
* Declarations are property–value pairs
* Type selectors style all elements of a type
* ID selectors style a single element
* Specificity determines which rule is applied

