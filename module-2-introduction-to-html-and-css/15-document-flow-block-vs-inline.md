# Document Flow: Block vs Inline Elements

By now, you know how CSS styles individual HTML elements. But how does the browser decide **where elements appear on the screen**?

The browser’s default method of positioning elements is called **document flow**.

---

## What Is Document Flow?

**Document flow** is the normal way a browser lays out HTML elements on a page.

By default, nearly all HTML elements fall into one of two categories:

* **Block-level elements**
* **Inline elements**

Understanding the difference between these two is essential for building clean layouts.

---

## Block-Level Elements

A **block-level element**:

* Occupies the **full width** of its parent container
* Takes up the **height of its content**
* Always starts on a **new line**
* Forces elements before and after it onto new lines

Multiple block-level elements stack vertically, like a stack of boxes.

### Common Block Elements

* `<div>`
* `<form>`
* `<h1>` to `<h6>`
* `<p>`

---

## Inline Elements

An **inline element**:

* Only occupies the **width and height of its content**
* Does **not** start on a new line
* Flows within surrounding text

Multiple inline elements can appear on the same line.

### Common Inline Elements

* `<a>` (anchor)
* `<img>`
* `<input>`
* `<label>`
* `<b>` (bold)
* `<i>` (italic)
* `<em>`
* `<span>`

---

## Example: `div` vs `span`

Consider the following HTML:

```html
<div>
  <span>Lorem ipsum dolor sit amet.</span>
  <span>Consectetur adipiscing elit.</span>
  <span>Sed do eiusmod tempor.</span>
</div>
```

Since `<span>` elements are inline, all text appears in a continuous flow on one line.

---

## Changing an Inline Element to a Block Element

If the middle sentence is changed from a `<span>` to a `<div>`:

```html
<div>
  <span>Lorem ipsum dolor sit amet.</span>
  <div>Consectetur adipiscing elit.</div>
  <span>Sed do eiusmod tempor.</span>
</div>
```

Because `<div>` is a block-level element:

* It moves to a new line
* The following inline content also shifts to a new line

---

## Changing Display Behavior with CSS

CSS allows you to change how elements behave using the `display` property.

---

## Example: Converting a Block Element to Inline

### HTML

```html
<div id="middle">Consectetur adipiscing elit.</div>
```

### CSS

```css
#middle {
  display: inline;
}
```

This changes the `<div>` from a block-level element to an inline element.

---

## Changing Back to Block

```css
#middle {
  display: block;
}
```

This restores the element’s original block behavior.

---

## Key Points About `display`

* `display: block` → element starts on a new line
* `display: inline` → element flows within text
* The `display` property controls layout behavior

Other display values exist and can further change layout behavior.

---

## Key Takeaways

* Document flow is how browsers position elements by default
* Block elements start on new lines and take full width
* Inline elements flow within surrounding content
* `div` is block-level, `span` is inline by default
* CSS `display` property can change element behavior

