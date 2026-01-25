# Linking HTML Documents

By now, you should know how to build a **basic webpage**, but how do you build a **website**?

A website is made up of **multiple web pages linked together**. To connect these pages, HTML uses the **anchor (`<a>`) tag**, which creates hyperlinks (commonly called links).

In this lesson, you will learn how to link different HTML pages together by creating a second page for the **Little Lemon** restaurant.

---

## What Is the Anchor (`<a>`) Tag?

The anchor tag is used to create hyperlinks that allow users to navigate between web pages.

* Links connect multiple HTML files
* Clicking a link loads another page in the browser

Basic syntax:

```html
<a href="filename.html">Link Text</a>
```

---

## Creating a Second Webpage

We will create a second webpage that displays the restaurant’s location.

### Steps to Create the File

1. In **Visual Studio Code**, right-click in the **Explorer** panel
2. Select **New File**
3. Name the file:

```text
location.html
```

---

## Adding Content to `location.html`

Use the same basic HTML structure as `index.html`, then add new content.

### Example Code

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Little Lemon Location</title>
  </head>
  <body>
    <h1>Our Location</h1>
    <p>123 Rome Road, Main District, Capital City</p>
  </body>
</html>
```

Save the file:

* **Windows**: `Ctrl + S`
* **Mac**: `Command + S`

---

## Linking Pages Using the Anchor Tag

Now that the location page is created, we will add a link to it from `index.html`.

### Adding a Link in `index.html`

Below the last paragraph, add an anchor (`<a>`) tag with the `href` attribute.

```html
<a href="location.html">Our Location</a>
```

* `href` stands for **Hypertext Reference**
* `location.html` is the file being linked
* `Our Location` is the clickable text shown on the webpage

---

## Testing the Link in a Browser

1. Save `index.html`
2. Right-click the file
3. Select **Reveal in File Explorer** (Windows) or **Reveal in Finder** (Mac)
4. Double-click `index.html`

The text **Our Location** will appear in blue, indicating a clickable link.

### Result

* Clicking the link opens `location.html`
* The browser navigates to the restaurant address page

Success 🎉

---

## Key Takeaways

* Websites consist of multiple linked HTML pages
* The `<a>` tag is used to create links
* The `href` attribute specifies the file to link to
* Link text appears clickable in the browser
* Linking pages allows you to build complete websites

Keep practicing by adding more pages and links. Best of luck 🚀
