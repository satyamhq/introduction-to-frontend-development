# Text and Color in CSS

When designing websites, you will work extensively with **text and colors**. CSS provides many ways to control how text appears and how colors are defined and displayed.

This section explains the most common ways to work with **color** and **text styling** in CSS.

---

## Color in CSS

Colors are used in many CSS properties, such as `color`, `background-color`, `border-color`, and more.

### Example

```css
p {
  color: blue;
}
```

---

## Ways to Define Colors

From **CSS Level 3**, there are **five main ways** to define colors:

1. RGB values
2. RGBA values
3. HSL values
4. Hexadecimal values
5. Predefined color names

---

## RGB Values

RGB stands for **Red, Green, and Blue**. This color model works based on how the human eye perceives color.

* Each value ranges from `0` to `255`
* `0` means no intensity
* `255` means full intensity

### Examples

* Red → `255, 0, 0`
* Black → `0, 0, 0`
* White → `255, 255, 255`

### CSS Usage

```css
p {
  color: rgb(255, 0, 0);
}
```

---

## RGBA Values

RGBA extends RGB by adding an **alpha (A)** channel.

* Alpha controls **opacity**
* Values range from `0` (fully transparent) to `1` (fully opaque)

### CSS Usage

```css
p {
  color: rgba(255, 0, 0, 0.8);
}
```

---

## HSL Values

HSL stands for **Hue, Saturation, and Lightness**.

<img width="3894" height="3441" alt="6W-NFfelTF-vjRX3pXxfHw_71bfe705b84941a1b8f51eea05a848e1_text_color_hue" src="https://github.com/user-attachments/assets/47bacd8b-2425-4270-903e-184063a1fa9c" />


### Hue

![Uploading EoftTRz8S7uH7U0c_Fu7KQ_ba9919ab0ef54d29bb897ce29dcd03e1_text_color_hue2.png…]()


* Represented as degrees on a color wheel (`0`–`360`)
* `0` → red
* `120` → green
* `240` → blue

### Saturation

* Represents color intensity
* `0%` → gray
* `100%` → full color

### Lightness

* Controls brightness
* `0%` → black
* `100%` → white

### CSS Usage

```css
p {
  color: hsl(0, 100%, 50%);
}
```

---

## Hexadecimal Values

Hexadecimal (hex) colors use a **base‑16 number system**.

* Digits range from `0–9` and `A–F`
* Prefixed with `#`
* Represent RGB values in hex format

### Example

* Red (`255, 0, 0`) → `#FF0000`

### CSS Usage

```css
p {
  color: #FF0000;
}
```

Converters are commonly used to switch between RGB and hex values.

---

## Predefined Color Names

Modern browsers support **140 predefined color names**.

Some common examples include:

* black
* white
* gray
* red
* blue
* green
* yellow
* purple
* navy
* teal
* aqua

### Example

```css
p {
  color: red;
}
```

---

## Text Styling in CSS

CSS provides many properties to control how text is displayed.

---

## Text Color

The `color` property sets the color of text.

```css
p {
  color: red;
}
```

---

## Font Family and Font Size

A **font** defines the visual style of text characters.

### Font Family

The `font-family` property specifies which font to use.

```css
p {
  font-family: "Courier New", monospace;
}
```

Multiple fonts are listed as **fallbacks**. If the first font is unavailable, the browser tries the next one.

---

### Font Size

The `font-size` property controls text size.

```css
p {
  font-size: 12px;
}
```

---

## Text Transformation

The `text-transform` property changes text capitalization.

```css
p {
  text-transform: uppercase;
}
```

Common values:

* `uppercase`
* `lowercase`
* `capitalize`
* `none` (default)

---

## Text Decoration

The `text-decoration` property adds visual decoration to text.

### Basic Example

```css
p {
  text-decoration: underline;
}
```

### Advanced Decoration

```css
p {
  text-decoration: underline red solid 5px;
}
```

---

### Individual Text Decoration Properties

```css
p {
  text-decoration-line: underline;
  text-decoration-color: red;
  text-decoration-style: solid;
  text-decoration-thickness: 5px;
}
```

#### Common Values

* Lines: `underline`, `overline`, `line-through`, `none`
* Styles: `solid`, `double`, `dotted`, `dashed`, `wavy`

---

## Key Takeaways

* CSS supports multiple color formats
* RGB, RGBA, HSL, hex, and named colors are widely used
* Text styling includes font, size, color, transformation, and decoration
* Fallback fonts improve compatibility
* Text decoration can be customized in detail

