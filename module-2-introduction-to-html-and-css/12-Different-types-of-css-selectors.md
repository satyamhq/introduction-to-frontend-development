# Different Types of CSS Selectors

When styling a web page, CSS provides many types of **selectors**. These selectors allow developers to be as **broad or as specific as needed** when choosing which HTML elements a rule should apply to.

This section covers some of the **most commonly used CSS selectors**.

---

## Element Selectors

The **element selector** selects HTML elements based on their **tag name**.

### Example

**HTML**

```html
<p>Once upon a time...</p>
<p>In a hidden land...</p>
```

**CSS**

```css
p {
  color: blue;
}
```

This rule applies to **all `<p>` elements** on the page.

---

## ID Selectors

The **ID selector** selects a single, unique element using its `id` attribute.

* IDs must be **unique** within a webpage
* ID selectors are prefixed with `#`

### Example

**HTML**

```html
<span id="latest">New!</span>
```

**CSS**

```css
#latest {
  background-color: purple;
}
```

This rule applies only to the element with the ID `latest`.

---

## Class Selectors

The **class selector** selects all elements that share the same class name.

* Multiple elements can have the same class
* Class selectors are prefixed with `.`

### Example

**HTML**

```html
<a class="navigation">Go Back</a>
<p class="navigation">Go Forward</p>
```

**CSS**

```css
.navigation {
  margin: 2px;
}
```

This rule applies to **all elements with the `navigation` class**.

---

## Element with Class Selector

You can create more **specific selectors** by combining an element selector with a class or ID selector.

### Example

**HTML**

```html
<p class="introduction">Welcome to the site</p>
```

**CSS**

```css
p.introduction {
  margin: 2px;
}
```

This rule applies only to `<p>` elements that have the `introduction` class.

---

## Descendant Selectors

**Descendant selectors** select elements that are contained within another element, at **any depth level**.

### Example Structure

**HTML**

```html
<div id="blog">
  <h1>Latest News</h1>
  <div>
    <h1>Today's Weather</h1>
    <p>The weather will be sunny</p>
  </div>
  <p>Subscribe for more news</p>
</div>
<div>
  <h1>Archives</h1>
</div>
```

**CSS**

```css
#blog h1 {
  color: blue;
}
```

This rule selects **all `<h1>` elements inside the element with ID `blog`**, but not the `Archives` heading.

### Multiple Descendants

```css
#blog div h1 {
  color: blue;
}
```

This selects `<h1>` elements that are descendants of `<div>` elements inside `#blog`.

---

## Child Selectors

The **child selector** is more specific than a descendant selector.

* It selects only **direct children**
* Uses the `>` combinator

### Example

**HTML**

```html
<div id="blog">
  <h1>Latest News</h1>
  <div>
    <h1>Today's Weather</h1>
    <p>The weather will be sunny</p>
  </div>
  <p>Subscribe for more news</p>
</div>
```

**CSS**

```css
#blog > h1 {
  color: blue;
}
```

This rule applies only to the **direct child `<h1>`** (`Latest News`) and not to nested headings.

---

## `:hover` Pseudo-Class

A **pseudo-class** selects elements based on their **state**.

The `:hover` pseudo-class applies styles when the mouse pointer hovers over an element.

### Example

```css
a:hover {
  color: orange;
}
```

This changes the color of a link when it is hovered over.

---

## Other Selectors

CSS provides many additional selectors, including:

* Attribute selectors
* Pseudo-elements
* Sibling selectors
* Universal selector (`*`)

You can combine selectors to create powerful and precise styling rules.

---

## Key Takeaways

* Selectors determine which elements a CSS rule applies to
* Element selectors target all elements of a type
* ID selectors target one unique element
* Class selectors target multiple elements
* Descendant selectors target nested elements
* Child selectors target direct children only
* Pseudo-classes enable interactive styling

Mastering selectors allows you to style webpages efficiently and precisely 🎯
