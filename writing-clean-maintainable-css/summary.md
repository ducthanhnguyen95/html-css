# Clean CSS Summary

This document summarizes best practices for writing clean and maintainable CSS code.

---

## 1. Naming Conventions

- **Follow a naming convention for naming IDs and classes.**  
  The most common naming conventions are:
  - **PascalCase**
  - **camelCase**
  - **kebab-case**

---

## 2. Stylesheet Organization

- **For a small project:**  
  You can write all of your CSS rules in one stylesheet.  
  - **Tip:** Use CSS comments to create logical sections in your stylesheet.

- **For a more complex project:**  
  You need to separate your stylesheet into multiple files and combine them together using build tools such as:
  - **Webpack**
  - **Rollup**
  - **Parcel**

---

## 3. Selector Specificity

- **Avoid over-specific selectors.**  
  Limit nesting to two or, at most, three selectors to keep your styles manageable.

---

## 4. Avoid `!important`

- **Avoid the `!important` keyword as much as possible.**  
  Overusing it can make your CSS hard to override and maintain.

---

## 5. Sorting CSS Properties

- **Sort CSS properties.**  
  Organizing properties in a consistent order (alphabetically or by grouping functionality) makes your code easier to read and maintain.

---

## 6. Style Inheritance

- **Take advantage of style inheritance**  
  and reduce duplication in your styles by leveraging CSS's cascading nature.

---

## 7. CSS Variables (Custom Properties)

- **Use CSS variables, also called custom properties, to keep your code DRY (Don't Repeat Yourself).**
  
- **How to use them:**
  - Declare variables using the `:root` selector, which targets the `<html>` element.
  - Access these variables using the `var()` function.

- **Example:**
  ```css
  :root {
    --primary-color: #3498db;
    --font-size: 16px;
  }

  body {
    color: var(--primary-color);
    font-size: var(--font-size);
  }
