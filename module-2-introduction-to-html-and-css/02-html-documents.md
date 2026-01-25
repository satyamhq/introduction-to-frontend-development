# HTML Documents – Basic Structure and Example

In this lesson, we explore the **blueprint of an HTML document** by creating a simple webpage for a restaurant called **Little Lemon**.

One great thing about HTML documents is that they **do not need the internet** to be viewed. You can save an HTML file on your computer and open it directly in a web browser—just like enjoying takeaway food at home 🍽️.

By the end of this lesson, you will be able to:

* Identify the structure of an HTML document
* Create a basic webpage using common HTML elements

---

## Creating an HTML File

Follow these steps to create your first HTML file:

1. Open **Visual Studio Code**
2. Right-click in the **Explorer** panel
3. Select **New File**
4. Name the file:

```text
index.html
```

---

## Standard HTML Document Structure

Before adding content, every HTML document should follow a standard structure. This structure helps browsers correctly read and display the webpage.

### Key Parts of an HTML Document

* **DOCTYPE declaration**
  Tells the browser that the document is an HTML document

* **`<html>` element**
  The root element that wraps the entire page

* **`<head>` element**
  Contains metadata (information not shown on the page)

* **`<body>` element**
  Contains all visible content

---

## Basic HTML Skeleton

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Little Lemon</title>
  </head>
  <body>
  </body>
</html>
```

---

## The `<head>` Section

The `<head>` element contains **metadata**, which is not directly visible on the webpage.

### Common Uses of `<head>`

* Page title (shown in the browser tab)
* Meta tags (description, keywords)
* Links to CSS files

### Example

```html
<head>
  <title>Little Lemon</title>
</head>
```

---

## The `<body>` Section

The `<body>` element contains everything the user can see on the webpage, including:

* Headings
* Paragraphs
* Images
* Videos

---

## Adding Page Content

### Main Heading

```html
<h1>Our Menu</h1>
```

### Menu Items (Subheadings)

```html
<h2>Falafel</h2>
<h2>Pasta Salad</h2>
```

### Adding Descriptions with Paragraphs

```html
<p>Chickpea, herbs, and spices</p>
<p>Lettuce, vegetables, and mozzarella</p>
```

---

## Complete Example: Little Lemon Menu Page

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Little Lemon</title>
  </head>
  <body>
    <h1>Our Menu</h1>

    <h2>Falafel</h2>
    <p>Chickpea, herbs, and spices</p>

    <h2>Pasta Salad</h2>
    <p>Lettuce, vegetables, and mozzarella</p>
  </body>
</html>
```

---

## Viewing the HTML File in a Browser

1. Save the file

   * **Windows**: `Ctrl + S`
   * **Mac**: `Command + S`

2. Right-click `index.html`

3. Select **Reveal in File Explorer / Finder**

4. Double-click the file

The page will open in your default web browser 🎉

---

## Key Takeaways

* HTML files can be viewed locally without a server
* Every HTML document follows a standard structure
* `<head>` is used for metadata, `<body>` is used for content
* Headings and paragraphs are core building blocks of a webpage
* Practice by editing the file and refreshing the browser
