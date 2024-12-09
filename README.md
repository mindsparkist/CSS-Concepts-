# CSS-Concepts
**Understanding * and body Selectors**

In CSS, the `*` and `body` selectors are used to target specific elements in an HTML document, but they differ in their scope and specificity.

**Universal Selector (`*`)**

* **Scope:** Targets all elements in the document.
* **Specificity:** Low specificity.
* **Usage:**
  - Often used to set default styles for all elements, such as:
    ```css
    * {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
    ```
  - Can be used to apply styles to all elements of a particular type, but it's generally not recommended due to its low specificity.

**Body Selector (`body`)**

* **Scope:** Targets the `<body>` element, which contains the main content of the page.
* **Specificity:** Higher specificity than the universal selector.
* **Usage:**
  - Commonly used to set global styles for the entire page, such as:
    ```css
    body {
        font-family: Arial, sans-serif;
        font-size: 16px;
        line-height: 1.5;
        background-color: #f0f0f0;
    }
    ```

**Key Differences:**

| Feature | Universal Selector (`*`) | Body Selector (`body`) |
|---|---|---|
| Scope | All elements | `<body>` element |
| Specificity | Low | Higher |
| Common Usage | Default styles, less specific targeting | Global page styles |

**When to Use Which:**

- **Use the `*` selector** sparingly, primarily for setting default styles or for very specific, targeted styles where specificity isn't a concern.
- **Use the `body` selector** for global page styles that affect the entire content area.

By understanding the differences between the `*` and `body` selectors, you can effectively style your HTML documents and create consistent, visually appealing layouts.

