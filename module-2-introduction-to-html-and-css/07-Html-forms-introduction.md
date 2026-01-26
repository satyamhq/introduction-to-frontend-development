# What Are Forms in HTML?

Today, you can order almost anything online—from food to electronics. One of the key features that makes this possible is **HTML forms**. Without forms, users would not be able to:

* Log in to websites
* Enter credit card details
* Submit contact information
* Search or filter content

Forms are used every day across the web, far beyond e‑commerce.

In this lesson, you will learn how HTML forms work and explore common **input types** used to collect user data.

---

## How HTML Forms Work

When a user enters data into a form and submits it, the form sends an **HTTP request** containing that data to a server.

HTML forms are defined using the `<form>` tag.

### The `<form>` Tag

```html
<form>
</form>
```

Forms support important attributes that control how data is sent.

---

## The `action` Attribute

The `action` attribute specifies **where** the form data should be sent.

```html
<form action="/submit">
</form>
```

* It defines a URL or path
* If omitted, the form submits to the **current page**

---

## The `method` Attribute

The `method` attribute specifies **how** the data is sent.

There are two main HTTP methods used by forms:

* **GET** – retrieves information from the server
* **POST** – sends data to the server

```html
<form method="post">
</form>
```

> You will explore form submission and HTTP methods in more detail in a later course.

---

## Input Fields

Form fields are created using the `<input>` tag.

* `<input>` is a **self-closing tag**
* Different input types collect different kinds of data

---

## Text Input

Used for single-line text such as a username.

```html
<label>Username</label>
<input type="text">
```

---

## Password Input

Used for passwords. Characters entered are **masked**.

```html
<label>Password</label>
<input type="password">
```

---

## Submit Button

The submit button sends the form data to the server.

```html
<input type="submit" value="Submit">
```

When clicked, the browser sends an HTTP request using the specified method.

---

## Complete Basic Form Example

```html
<form method="post">
  <label>Username</label><br>
  <input type="text"><br><br>

  <label>Password</label><br>
  <input type="password"><br><br>

  <input type="submit" value="Login">
</form>
```

---

## Checkboxes

Checkboxes allow users to select **multiple options**.

```html
<input type="checkbox" name="food" value="pizza"> Pizza
<input type="checkbox" name="food" value="pasta"> Pasta
```

Each checkbox can be checked or unchecked independently.

---

## Radio Buttons

Radio buttons allow users to select **only one option** from a group.

```html
<input type="radio" name="size" value="small"> Small
<input type="radio" name="size" value="large"> Large
```

Selecting one radio button unchecks the others in the same group.

---

## Other Common Input Types

HTML provides many additional input types, including:

* `number`
* `email`
* `file`

```html
<input type="email">
<input type="number">
<input type="file">
```

---

## Text Area (`<textarea>`)

For **multi-line text input**, use the `<textarea>` tag instead of `<input>`.

```html
<textarea rows="4" cols="30"></textarea>
```

---

## Drop-Down Lists (`<select>`)

Drop-down lists allow users to choose one option from a list.

```html
<select>
  <option>Option 1</option>
  <option>Option 2</option>
  <option>Option 3</option>
</select>
```

---

## Key Takeaways

* HTML forms collect user input
* `<form>` defines a form
* `action` specifies where data is sent
* `method` specifies how data is sent
* `<input>` supports many input types
* `<textarea>` is used for multi-line text
* `<select>` and `<option>` create drop-down lists

Next time you shop online, take a moment to notice how many form elements you interact with. You now have the knowledge to choose the right input types and build user-friendly forms yourself 🚀
