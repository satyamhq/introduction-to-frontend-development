# Getting Started with Bootstrap

## Overview

Bootstrap is a front-end framework that provides pre-written CSS and JavaScript components to help build responsive websites faster than creating everything from scratch. It simplifies layout design, styling, and responsiveness using a grid system and reusable UI components.

---

## Why Use Bootstrap?

* Saves development time
* Provides a responsive grid system
* Includes ready-made CSS and JavaScript components
* Ensures consistent design across browsers and devices

---

## Basic Bootstrap Page Structure

### 1. Container

* The **container** is the first required element in a Bootstrap layout.
* It wraps the content and enables the grid system.
* Implemented using a `<div>` with the `container` class.

### 2. Row

* Rows are placed inside containers.
* Created using a `<div>` with the `row` class.
* Rows hold columns and help align content horizontally.

### 3. Columns

* Columns are created using the `col` class.
* In this example:

  * One column is used for **menu items**
  * One column is used for **prices**

---

## Adding Content to Columns

### Menu Column

#### Headings

* `H1` tag: Column title ("Our Menu")
* `H2` tag: Dish name (e.g., Falafel, Pasta Salad)

#### Dish Details

* Use a `<p>` tag to list ingredients

**Example Ingredients:**

* Falafel: Chickpeas, herbs, spices
* Pasta Salad: Lettuce, vegetables, mozzarella

#### Images

* Use the `<img>` tag with the `src` attribute to link images
* Apply the `img-fluid` class

**Benefits of `img-fluid`:**

* Automatically scales images to fit the parent column width
* No need to manually set image dimensions

---

## Adding Multiple Dishes

* Repeat the structure:

  * `H2` for dish name
  * `<p>` for ingredients
  * `<img>` for the dish image

---

## Creating a Price Table

### Table Setup

* Use the `<table>` tag
* Apply the Bootstrap `table` class for styling

### Table Structure

* `<tr>`: Table row (one per dish)
* `<td>`: Table data cells

  * First cell: Dish name
  * Second cell: Price

**Example:**

* Falafel – $12
* Pasta Salad – $10

---

## Previewing the Webpage

* Save the file:

  * Windows/Linux: `Ctrl + S`
  * macOS: `Command + S`
* Use Live Preview to view changes instantly

---

## Result

* Menu items displayed in columns
* Images scale correctly
* Price table styled automatically using Bootstrap

---

## Key Takeaway

By using Bootstrap containers, rows, columns, responsive images, and tables, you can quickly build a clean and responsive webpage with minimal custom CSS.
