# Using Bootstrap Styles

## Overview

Bootstrap is a mobile-first front-end framework designed to help developers build responsive websites that adapt seamlessly across devices, platforms, and screen sizes—without redesigning for each device.

In this module, we focus on **Bootstrap CSS class infixes and modifiers**, which help save development time while maintaining responsive and consistent UI design.

---

## Responsive Design in Bootstrap

### Mobile-First Approach

* Bootstrap is **mobile-first** by default.
* Styles are applied to small screens first, then enhanced for larger screens using breakpoints.

---

## Bootstrap Breakpoints (Class Infixes)

Bootstrap uses **breakpoints** to control how layouts change based on screen size. These breakpoints are applied using **class infixes** in CSS class names.

### Available Breakpoints

| Breakpoint Name   | Screen Width | Abbreviation       |
| ----------------- | ------------ | ------------------ |
| Extra Small       | < 576px      | Default (no infix) |
| Small             | ≥ 576px      | `sm`               |
| Medium            | ≥ 768px      | `md`               |
| Large             | ≥ 992px      | `lg`               |
| Extra Large       | ≥ 1200px     | `xl`               |
| Extra Extra Large | ≥ 1400px     | `xxl`              |

### Key Notes

* **Extra small (XS)** has no infix because it is the default.
* Breakpoint abbreviations are inserted directly into class names.

---

## Using Class Infixes in the Grid System

Bootstrap grid classes use breakpoint infixes to change layouts at specific screen sizes.

### Example

* `col-6` → Applies to all screen sizes
* `col-lg-6` → Applies only on large screens and above

This allows layouts to adapt without writing custom media queries.

---

## Bootstrap Components and Modifiers

Bootstrap provides pre-built UI components with **modifiers** that control appearance, such as color and emphasis.

### What Are Modifiers?

* Modifiers are the suffixes added to component class names
* They change the **context or style** of a component

---

## Alert Component Example

Alerts are used to display messages that require user attention, such as:

* Information
* Warnings
* Errors
* Confirmations

### Alert Structure

* Base class: `alert`
* Contextual class: `alert-{modifier}`
* Role attribute: `role="alert"`

---

## Available Alert Modifiers

| Modifier    | Purpose                |
| ----------- | ---------------------- |
| `primary`   | Default / main message |
| `secondary` | Secondary information  |
| `success`   | Success messages       |
| `info`      | Informational messages |
| `warning`   | Warnings               |
| `danger`    | Errors                 |
| `light`     | Light background       |
| `dark`      | Dark background        |

### Examples

* `alert-primary` → Blue alert
* `alert-danger` → Red alert for errors

The only difference between alert types is the **color used**.

---

## Modifiers in Practice

* To change an alert from blue to red:

  * Replace `primary` with `danger`
* Modifiers make it easy to reuse components with different visual meanings

---

## Key Takeaways

* Bootstrap eliminates the need to redesign for different devices
* **Class infixes** control responsive behavior at breakpoints
* **Modifiers** customize component appearance
* Using infixes and modifiers saves time and reduces custom CSS

---

By mastering Bootstrap infixes and modifiers, you can build flexible, responsive, and visually consistent web applications efficiently.
