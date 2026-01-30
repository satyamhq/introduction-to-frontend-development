# Component Hierarchy in React

## Overview

Planning an application as a collection of components can feel challenging at first. However, with practice, structuring applications using a **component hierarchy** becomes natural and highly effective.

React makes it easy to build user interfaces quickly by organizing the UI into reusable, nested components.

---

## Root Component

* Every React application has at least one component
* This is known as the **root component** or **App component**
* All other components are added inside it

The result is a **tree structure** of components that make up the application.

---

## Understanding Component Hierarchy

Components are organized in **parent–child relationships**:

* Parent components contain child components
* Child components can be reused multiple times
* Updates to data can add, remove, or update components dynamically

---

## Example: Shopping List Application

### Component Structure

* **App** (root component)

  * **NewItemBar**
  * **ShoppingList**

    * **ShoppingItem** (reused for each item)

### How It Works

* `NewItemBar` allows users to add new items
* `ShoppingList` displays all items
* Each item is rendered using the same `ShoppingItem` component
* Removing an item deletes its corresponding `ShoppingItem` component

This demonstrates component reuse and dynamic updates.

---

## Example: Blog Website

### High-Level Structure

* **App**

  * **Navbar**
  * **Page**

---

### Navbar Component

Contains:

* Blog title
* Navigation links
* Search component

---

### Page Component

Contains:

* **MainFeature** component
* **SmallFeature** component
* **SmallFeature** component (reused)

---

## Reusable Components

* `MainFeature` displays a highlighted blog post
* `SmallFeature` displays a blog summary with a thumbnail
* The same `SmallFeature` component is reused with different properties

This reuse of components reduces duplicated code and improves maintainability.

---

## Benefits of Component Hierarchy

* Clear structure and organization
* Reusable UI pieces
* Easier maintenance and updates
* Scalable application design

---

## Key Takeaways

* React applications are built as a tree of components
* The App component sits at the root
* Components can be reused with different data
* Planning component hierarchy improves efficiency and clarity

With practice, designing component hierarchies becomes an intuitive and powerful way to build React applications.
