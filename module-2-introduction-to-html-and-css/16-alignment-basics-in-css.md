# Alignment Basics in CSS

Alignment plays a key role in making websites readable and visually balanced. In this section, you’ll learn how to align **text** and **HTML elements** using CSS.

We’ll focus on **horizontal alignment** first. Vertical alignment is more complex and will be explored later.

---

## Text Alignment

Aligning text inside an HTML element is straightforward using the `text-align` property.

### Example

```css
p {
  text-align: center;
}
```

This rule centers the text inside all `<p>` elements.

### Common `text-align` Values

* `left` – default for left-to-right languages (like English)
* `right` – default for right-to-left languages (like Arabic)
* `center`
* `justify`

The **justify** value spreads text so that each line has the same width.

---

## HTML Element Alignment

Aligning HTML elements is more complex than aligning text. It depends on:

* The **box model**
* The **document flow**
* Whether the element is **block-level** or **inline**

---

## Center Aligning a Block-Level Element

To center an element horizontally:

1. Set a width
2. Set left and right margins to `auto`

### HTML Structure

```html
<div class="parent">
  <div class="child"></div>
</div>
```

### CSS

```css
.parent {
  border: 4px solid red;
}

.child {
  width: 50%;
  padding: 20px;
  border: 4px solid green;
  margin: auto;
}
```

---

## Result

The **child element is centered horizontally** inside the parent element.

<img width="313" height="36" alt="ElKjOOdnT2GSozjnZy9hJw_0670f63ae6e548a28dfa041b7983bfe1_css_center_div" src="https://github.com/user-attachments/assets/b4992294-5d83-49d4-9227-7f834959736f" />

## Center Aligning an Inline Element (Images)

Inline elements (such as `<img>`) cannot be centered using `margin: auto` unless they are converted into block-level elements.

### HTML

```html
<div class="parent">
  <img src="photo.png" class="child">
</div>
```

### CSS

```css
.child {
  display: block;
  width: 50%;
  margin: auto;
}
```


---

## Precise Center Alignment

To control vertical spacing while centering horizontally, set only left and right margins to `auto`.

```css
.child {
  display: block;
  width: 50%;
  margin-left: auto;
  margin-right: auto;
}
```

---

## Left and Right Alignment of Elements

The two most common ways to align elements left or right are:

* `float`
* `position`

For now, we’ll focus on **float**.

---

## Floating Elements

The `float` property positions an element relative to the surrounding text. Text wraps around the floated element.

### Example: Right-Aligned Image

**HTML**

```html
<div class="parent">
  <img src="photo.png" class="child">
  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur eu odio eget leo auctor porta sit amet sit amet justo. Donec fermentum quam in diam volutpat, at lacinia diam placerat. Aenean quis feugiat sem.
</div>
```

**CSS**

```css
.child {
  float: right;
}
```

<img width="710" height="371" alt="02" src="https://github.com/user-attachments/assets/61b64ee7-e179-438a-b73a-c1667b5a4e3c" />

---

## Key Takeaways

* `text-align` is used for aligning text
* HTML element alignment depends on box model and document flow
* Block-level elements can be centered using `margin: auto`
* Inline elements must be converted to block-level to be centered
* `float` allows left and right alignment with text wrapping
