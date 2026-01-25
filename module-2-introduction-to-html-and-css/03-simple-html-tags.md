# HTML Text Formatting, Lists, Divs, and Comments

This lesson explains how HTML handles **text formatting**, **lists**, **division containers**, and **comments**, with clear examples and browser behavior.

---

## Line Breaks (`<br>`)

HTML ignores line breaks and extra spaces inside a paragraph by default. To force a new line, you must use the `<br>` tag.

* `<br>` is a **self-closing tag**
* It does **not** require a closing tag

### Example

```html
<p>
  This paragraph<br>
  contains a lot of lines<br>
  and they are displayed.
</p>
```

### Displayed in the Browser

This paragraph
contains a lot of lines
and they are displayed.

---

## Strong (`<strong>`)

The `<strong>` tag is used to indicate that a piece of text is **important**. Screen readers emphasize this text for accessibility.

### Example

```html
<p>
  No matter how much the dog barks: <strong>don't feed him chocolate</strong>.
</p>
```

### Displayed in the Browser

No matter how much the dog barks: **don't feed him chocolate**.

---

## Bold (`<b>`)

The `<b>` tag is used to **draw attention visually**, but it does **not** add importance or meaning.

### Example

```html
<p>
  The primary colors are <b>red</b>, <b>yellow</b>, and <b>blue</b>.
</p>
```

### Displayed in the Browser

The primary colors are **red**, **yellow**, and **blue**.

### When to Use `<b>`

```html
<p>
  The three core technologies of the Internet are <b>HTML</b>, <b>CSS</b>, and <b>JavaScript</b>.
</p>
```

Use `<b>` for emphasis **without meaning or importance**.

---

## Emphasis (`<em>`)

The `<em>` tag adds **emphasis** to text and conveys meaning. Screen readers will stress emphasized words.

### Example

```html
<p>
  Wake up <em>now</em>!
</p>
```

### Displayed in the Browser

Wake up *now*!

---

## Italics (`<i>`)

The `<i>` tag is used to offset text, such as:

* Technical terms
* Book titles
* Thoughts
* Foreign words

### Example

```html
<p>
  The term <i>HTML</i> stands for HyperText Markup Language.
</p>
```

### Displayed in the Browser

The term *HTML* stands for HyperText Markup Language.

---

## Emphasis vs Italics

Both `<em>` and `<i>` look similar by default, but they have **different meanings**.

### Emphasis Example

```html
<p>
  I <em>really</em> want ice cream.
</p>
```

Emphasis stresses the importance of the word.

### Italics Example

```html
<p>
  My favourite book is <i>Dracula</i>.
</p>
```

Italics are used for titles or offset text. Screen readers **do not announce italics differently**.

---

## Lists in HTML

HTML supports two main types of lists.

---

### Unordered List (`<ul>`)

Used when order does not matter.

```html
<ul>
  <li>Tea</li>
  <li>Sugar</li>
  <li>Milk</li>
</ul>
```

### Displayed in the Browser

* Tea
* Sugar
* Milk

---

### Ordered List (`<ol>`)

Used when order is important.

```html
<ol>
  <li>Rocky</li>
  <li>Rocky II</li>
  <li>Rocky III</li>
</ol>
```

### Displayed in the Browser

1. Rocky
2. Rocky II
3. Rocky III

---

## Div (`<div>`) Tag

The `<div>` tag defines a **generic container** used to group content. It has **no visual effect** unless styled with CSS.

### Basic Example

```html
<div>
  <p>This is a paragraph inside a div</p>
</div>
```

---

### Nested Div Example

```html
<div>
  <div>
    <p>This is a paragraph inside a div that’s inside another div</p>
  </div>
</div>
```

Div elements can be nested inside other elements.

---

## Styling Divs with CSS (Preview)

The following CSS adds a border and spacing to all div elements.

> You will learn CSS in detail in later lessons.

```html
<style>
  div {
    border: 1px solid black;
    padding: 2px;
  }
</style>

<div>
  <div>
    <p>This is a paragraph inside stylized divs</p>
  </div>
</div>
```

---

## HTML Comments

Comments are used to leave notes for developers. They are **not displayed** in the browser.

### Example

```html
<!-- This is a comment -->

<p>This paragraph is visible</p>
<!-- This paragraph is hidden -->
```

---

## Key Takeaways

* `<br>` forces a line break
* `<strong>` indicates importance
* `<b>` is for visual emphasis only
* `<em>` adds semantic emphasis
* `<i>` offsets text like titles or terms
* Lists can be ordered or unordered
* `<div>` is a generic container
* Comments are ignored by the browser
