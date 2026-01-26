# Adding Images to a Webpage with HTML

A picture is worth a thousand words. A website without images often provides a poor user experience—especially websites about food 🍽️. The **Little Lemon** website can certainly benefit from adding some images.

In this lesson, you will learn how to add images to an HTML document using the **image (`<img>`) tag**, resize images, and improve accessibility with alternative text.

---

## The Image (`<img>`) Tag

Images are **not embedded directly** into HTML files. Instead, HTML uses the `<img>` tag to **link to image files**. The browser then displays those images on the webpage.

The `<img>` tag:

* Is a **self-closing tag**
* Creates a placeholder for the image
* Requires attributes to work correctly

---

## Image Files in the Project

In this example, the project folder contains two image files:

* `falafel.jpeg`
* `salad.jpeg`

---

## Adding Images to HTML

To add an image, use the `<img>` tag with the `src` (source) attribute.

### Example

```html
<img src="falafel.jpeg">
<img src="salad.jpeg">
```

Save the file and open it in the browser. The images will appear, but they may be **too large**.

---

## Resizing Images Using HTML

You can control image size by adding the `width` and `height` attributes.

### Example

```html
<img src="falafel.jpeg" width="240" height="135">
<img src="salad.jpeg" width="240" height="135">
```

* `width` is measured in pixels
* `height` is measured in pixels

After saving and refreshing the browser, the images will appear smaller and better sized.

---

## Adding Alternative Text (`alt` Attribute)

The **`alt` (alternative text)** attribute provides a text description of an image.

### Why `alt` Text Is Important

* Improves **accessibility** for screen readers
* Helps users who cannot see images
* Improves **search engine optimization (SEO)**

The `alt` text is **not displayed visually** on the webpage.

---

## Image with Alt Text Example

```html
<img src="falafel.jpeg" width="240" height="135" alt="A falafel">
<img src="salad.jpeg" width="240" height="135" alt="A pasta salad">
```

Screen readers use the `alt` attribute to describe images to users with visual impairments.

---

## Complete Example

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Little Lemon Menu</title>
  </head>
  <body>
    <h1>Our Menu</h1>

    <img src="falafel.jpeg" width="240" height="135" alt="A falafel">
    <img src="salad.jpeg" width="240" height="135" alt="A pasta salad">
  </body>
</html>
```

---

## Key Takeaways

* Images are added using the `<img>` tag
* Images are linked, not embedded
* The `src` attribute specifies the image file
* `width` and `height` control image size
* The `alt` attribute improves accessibility and SEO

Your **Little Lemon** website is now more colorful and accessible for everyone 🌍. Have fun adding images to your web pages 🎨
