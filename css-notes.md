# CSS Notes

CSS (Cascading Style Sheets) is used to style and design HTML web pages.

It controls the appearance, layout, spacing, colors, fonts, and responsiveness of a webpage.

## 📌 Why is CSS Used?

CSS helps to:

* Add colors and backgrounds
* Change fonts and text styles
* Control spacing and sizing
* Create layouts
* Add borders and shadows
* Make websites responsive
* Improve the overall appearance of web pages

## 🧩 Ways to Add CSS

### 1. Inline CSS

CSS is written directly inside an HTML element.

```html
<p style="color: blue;">Hello World</p>
```

### 2. Internal CSS

CSS is written inside a `<style>` tag in the HTML document.

```html
<style>
    p {
        color: blue;
    }
</style>
```

### 3. External CSS

CSS is written in a separate `.css` file and linked with HTML.

```html
<link rel="stylesheet" href="style.css">
```

External CSS is commonly used for larger projects.

## 🎨 Common CSS Properties

| Property           | Purpose                  |
| ------------------ | ------------------------ |
| `color`            | Changes text color       |
| `background-color` | Changes background color |
| `font-size`        | Changes text size        |
| `font-family`      | Changes font             |
| `margin`           | Adds outer spacing       |
| `padding`          | Adds inner spacing       |
| `border`           | Adds a border            |
| `width`            | Sets element width       |
| `height`           | Sets element height      |
| `text-align`       | Aligns text              |

## 📦 CSS Box Model

Every HTML element can be understood using the CSS box model.

```text
Content
   ↓
Padding
   ↓
Border
   ↓
Margin
```

* **Content:** Actual text or element
* **Padding:** Space inside the element
* **Border:** Boundary around the element
* **Margin:** Space outside the element

## 📐 CSS Grid

CSS Grid is used to create layouts using rows and columns.

Example:

```css
.container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 10px;
}
```

## ✨ Pseudo-classes

Pseudo-classes define a special state of an element.

Example:

```css
button:hover {
    background-color: black;
    color: white;
}
```

Here, the style is applied when the mouse pointer is over the button.

## 📱 Responsive Design

Responsive design allows a webpage to adapt to different screen sizes such as:

* Mobile phones
* Tablets
* Laptops
* Desktop computers

A common technique is using media queries.

```css
@media (max-width: 600px) {
    body {
        font-size: 14px;
    }
}
```

## 🎯 Learning Goals

* Understand CSS syntax
* Learn common CSS properties
* Understand the box model
* Create layouts using CSS Grid
* Practice responsive design
* Improve webpage styling

---

**Author:** Naziya Gouri
**Course:** BCA
