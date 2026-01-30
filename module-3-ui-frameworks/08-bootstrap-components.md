# Bootstrap Components

## Overview

Bootstrap includes a rich collection of **pre-built UI components** that help developers create visually appealing and consistent websites quickly. These components range from alerts and badges to cards and navigation menus.

In this section, Bootstrap components are used to enhance the **Little Lemon** website by adding a new dish and improving the overall layout.

---

## Adding a New Dish

### Dish Details

* Dish name: **Fried Calamari**
* Ingredients: Squid, buttermilk

### Steps

* Add an `h2` heading with the dish name
* List ingredients directly under the heading
* Add an image using the `<img>` tag
* Use the `img-fluid` class to ensure the image scales with its parent column

---

## Highlighting New Items with Badges

Bootstrap provides a **badge component** to highlight small pieces of information.

### Usage

* Add a `<span>` inside the `h2` heading
* Apply the `badge` class
* Add the contextual class `bg-primary` for a blue background
* Display text such as **New** inside the badge

---

## Improving Layout with Cards

The **card component** helps organize content such as images, titles, and text in a clean, structured layout.

### Card Features

* Supports images, titles, subtitles, and body content
* Improves visual consistency

### Responsive Card Layout

* Cards stack vertically on mobile devices: `col-12`
* Cards display side by side on desktop devices: `col-lg-6`

---

## Card Structure

Each dish card includes:

* `card` – main wrapper
* `card-img-top` – dish image
* `card-body` – content container
* `card-title` – dish name
* `card-text` – dish description

This structure improves readability and visual appeal.

---

## Updating the Price Table

* Add a new table row for Fried Calamari
* Use two `td` elements:

  * Dish name
  * Price

### Example

* Fried Calamari – $12

---

## Informing Users with Alerts

Bootstrap alerts are used to show important messages to users.

### Alert Setup

* Add a `div` with the `alert` class
* Use `alert-info` for a blue informational alert
* Add `role="alert"` to define its purpose

### Alert Message

* "Try our new Fried Calamari"

---

## Result

* Menu layout is more structured and visually appealing
* New dish is clearly highlighted
* Customers are informed using alerts
* Website feels more modern and engaging

---

## Key Takeaway

Bootstrap components such as **badges, cards, tables, and alerts** make it easy to enhance both functionality and design. Exploring more Bootstrap components can further improve user experience and engagement.
