# Using HTML to Work with Data in Tables

The **Little Lemon** website is coming along nicely, but one important piece of information is still missing — **prices**. A clean and effective way to display structured information like prices is by using an **HTML table**.

Tables allow content to be organized into **rows and columns**, similar to spreadsheet software. Websites commonly use tables to display:

* Price lists
* Event schedules
* Product sizes
* Technical specifications

In this lesson, you will learn how to create and style a basic HTML table.

---

## What Is an HTML Table?

An HTML table is used to display data in a structured format using:

* **Rows** (`<tr>`)
* **Data cells** (`<td>`)
* **Header cells** (`<th>`)

---

## Creating a Table

We will add a price table to the bottom of the `index.html` file.

### Step 1: Add the `<table>` Tag

Inside the `<body>` element, below the existing content, add a `<table>` tag.

---

## Adding Table Rows and Data

Each row in a table is created using the `<tr>` tag. Table data is added using `<td>` tags.

### Example: Menu Prices Table

```html
<table>
  <tr>
    <td>Falafel</td>
    <td>$10</td>
  </tr>
  <tr>
    <td>Pasta Salad</td>
    <td>$12</td>
  </tr>
</table>
```

Save the file and open it in the browser. The prices will appear, but the table will not yet look like a traditional table.

---

## Adding Table Headers

To make the table clearer, you can add **column headings** using the `<th>` (table header) tag.

### Updated Table with Headers

```html
<table>
  <tr>
    <th>Dish</th>
    <th>Price</th>
  </tr>
  <tr>
    <td>Falafel</td>
    <td>$10</td>
  </tr>
  <tr>
    <td>Pasta Salad</td>
    <td>$12</td>
  </tr>
</table>
```

Now the information is much clearer, with labels for each column.

---

## Styling the Table (Preview)

By default, HTML tables do not have borders. To make the table easier to read, we can add a small amount of CSS.

> You will learn proper CSS styling techniques later. This is just a quick preview.

### Adding a Border with CSS

```html
<style>
  table, th, td {
    border: 1px solid black;
  }
</style>
```

Save the file and refresh the browser. The table will now display visible borders around all cells.

---

## Complete Example

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Little Lemon Menu</title>
    <style>
      table, th, td {
        border: 1px solid black;
      }
    </style>
  </head>
  <body>
    <h1>Our Menu</h1>

    <table>
      <tr>
        <th>Dish</th>
        <th>Price</th>
      </tr>
      <tr>
        <td>Falafel</td>
        <td>$10</td>
      </tr>
      <tr>
        <td>Pasta Salad</td>
        <td>$12</td>
      </tr>
    </table>
  </body>
</html>
```

---

## Key Takeaways

* Tables organize data into rows and columns
* `<table>` defines the table
* `<tr>` creates a table row
* `<td>` defines table data cells
* `<th>` defines table headers
* CSS can be used to improve table appearance

Congratulations 🎉 You now know how to add tables to HTML files. Tables are widely used, and you’ll be using them a lot as you build more advanced websites.
