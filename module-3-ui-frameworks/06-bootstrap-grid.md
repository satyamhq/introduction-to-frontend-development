# Responsive Layout with Bootstrap Grid

## Introduction

Responsive web design depends on two key concepts:

* Responsive grids
* Responsive breakpoints

Bootstrap provides both through its built-in **grid system**, making it easier to design layouts that adapt across devices.

---

## Bootstrap Grid System

* Uses a **12-column layout**
* Can be **fluid** or **fixed**
* Built using three core elements:

  * Container
  * Rows
  * Columns

---

## Container

* The **container** is the root of the Bootstrap grid system
* Every grid layout starts with a container
* Responsibilities:

  * Adds padding
  * Aligns content
  * Adjusts width based on current breakpoint

---

## Rows and Columns

* Rows are placed inside containers
* Columns are placed inside rows
* Content lives inside columns

If no column size is specified:

* Bootstrap automatically divides space equally
* Two columns default to **6 + 6**

---

## Controlling Column Size

You can control how much space a column occupies by adding a **numeric suffix**.

### Example

* Menu column: `col-8`
* Price column: `col-4`

Total column width must equal **12**

---

## Responsive Layouts Using Breakpoints

Bootstrap allows different layouts per device using breakpoint-specific classes.

### Mobile vs Desktop Layout

#### Mobile Devices

* Columns take full width
* Use: `col-12`
* Content stacks vertically

#### Desktop Devices

* Columns displayed side by side
* Use: `col-lg-6`

---

## Column Wrapping

* Columns automatically wrap when total exceeds 12
* This behavior enables stacking without extra CSS

---

## Testing Responsiveness

* Save the file:

  * Windows/Linux: `Ctrl + S`
  * macOS: `Command + S`

* Open Developer Tools:

  * Press `F12`

* Enable **Device Mode** (mobile/tablet icon)

* Simulate different devices

---

## Result

* Desktop view: columns appear side by side
* Mobile view: content stacks vertically

---

## Benefits of Bootstrap Grid

* No need to redesign layouts for each device
* Automatic responsiveness via CSS rules
* Faster development workflow
* Suitable for most web development projects

---

## Key Takeaway

Bootstrap’s grid system provides a powerful, flexible, and mobile-first solution for building responsive layouts using containers, rows, columns, and breakpoints.
