# 🎨 CSS Full Course - Basic to Advanced with Properties and Examples

Welcome to the **CSS Full Course** README! This document covers CSS concepts from beginner to advanced with clean explanations, syntax, and real code examples.

---

## 🧠 1. What is CSS?

* **CSS** stands for **Cascading Style Sheets**.
* It styles HTML content — layout, colors, fonts, spacing, and more.
* CSS can be written **inline**, **internal**, or **external**.

```html
<!-- External CSS -->
<link rel="stylesheet" href="styles.css">

<!-- Internal CSS -->
<style>
  body { background-color: lightblue; }
</style>

<!-- Inline CSS -->
<h1 style="color: red;">Hello</h1>
```

---

## ✍️ 2. Selectors in CSS

### 🔹 Types of Selectors:

* `*` → Universal Selector
* `element` → Tag Selector
* `.class` → Class Selector
* `#id` → ID Selector
* `element1, element2` → Grouping
* `element1 element2` → Descendant

```css
* { margin: 0; }
h1 { color: blue; }
.box { padding: 10px; }
#header { background: gray; }
div p { font-size: 14px; }
```

---

## 🧠 3. Colors in CSS

* `color`: Text color
* `background-color`: Background
* Supports `hex`, `rgb()`, `hsl()`, `named` colors

```css
body { background-color: #f0f0f0; color: #333; }
```

---

## 🧱 4. Box Model

* **Content → Padding → Border → Margin**
* Properties:

  * `padding`, `margin`, `border`, `width`, `height`

```css
.box {
  margin: 20px;
  padding: 10px;
  border: 2px solid black;
  width: 300px;
}
```

---

## 🪤 5. Text and Font Styling

* `color`, `text-align`, `text-decoration`, `text-transform`
* `font-size`, `font-family`, `font-weight`, `line-height`

```css
p {
  font-family: 'Arial';
  font-size: 18px;
  text-align: justify;
  line-height: 1.6;
}
```

---

## 📆 6. Display and Positioning

### 🔹 Display:

* `block`, `inline`, `inline-block`, `none`, `flex`, `grid`

### 🔹 Position:

* `static`, `relative`, `absolute`, `fixed`, `sticky`

```css
.header {
  position: sticky;
  top: 0;
  background: white;
}
```

---

## 📐 7. Flexbox

* Layout tool for 1D alignment (row/column)

```css
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
```

---

## 🔲 8. Grid Layout

* Layout system for 2D (rows and columns)

```css
.grid {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 20px;
}
```

---

## 🎯 9. Pseudo-classes & Pseudo-elements

```css
a:hover { color: red; }
p::first-line { font-weight: bold; }
```

---

## 🧬 10. Media Queries (Responsive Design)

```css
@media (max-width: 768px) {
  body { background: yellow; }
}
```

---

## 🔄 11. Transitions and Animations

### Transitions:

```css
button {
  transition: background 0.3s ease;
}
```

### Keyframe Animation:

```css
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

div {
  animation: fadeIn 1s ease-in;
}
```

---

## 💡 12. Variables in CSS

```css
:root {
  --main-color: #3498db;
}

h1 {
  color: var(--main-color);
}
```

---

## 🧠 13. Best Practices

* Use class names that describe the role (`.nav`, `.btn-primary`)
* Avoid inline styles for scalability
* Use shorthand properties where possible (`margin: 10px 20px;`)
* Use a reset/normalize stylesheet
* Organize CSS with comments or sections

---

## 💡 14. Project Ideas

* Responsive Landing Page
* Profile Card UI
* Product Grid Layout
* Flexbox-based Navigation Bar
* CSS Animation Loader
* Mobile-first Portfolio Design

---

## 📚 Resources

* [MDN Web Docs - CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
* [W3Schools CSS](https://www.w3schools.com/css/)
* [CSS Tricks](https://css-tricks.com/)
* [Flexbox Froggy](https://flexboxfroggy.com/)
* [Grid Garden](https://cssgridgarden.com/)

---

## ❓ CSS Interview Questions and Answers

### Q1: What is the difference between `class` and `id` in CSS?

**Answer**: `class` can be reused on multiple elements, while `id` must be unique within a page.

### Q2: What is the Box Model in CSS?

**Answer**: The Box Model describes the layout of elements in terms of content, padding, border, and margin.

### Q3: What is the difference between `absolute`, `relative`, and `fixed` positioning?

**Answer**:

* `absolute`: Positioned relative to the nearest positioned ancestor.
* `relative`: Positioned relative to its normal position.
* `fixed`: Positioned relative to the viewport.

### Q4: What are pseudo-classes in CSS?

**Answer**: Pseudo-classes define a special state of an element like `:hover`, `:active`, `:first-child`.

### Q5: What is specificity in CSS?

**Answer**: Specificity determines which rule is applied when multiple rules match the same element. `id` > `class` > `element`.

### Q6: How do media queries help in responsive design?

**Answer**: Media queries allow you to apply different styles based on device size or screen resolution.

---

## 🔮 Important CSS Properties, Values, Usage, and Examples

### 1. `color` – Text Color

```css
p { color: blue; }
```

### 2. `background-color` – Background Fill

```css
div { background-color: lightgray; }
```

### 3. `font-size`, `font-family`, `font-weight`

```css
h1 {
  font-size: 36px;
  font-family: 'Verdana';
  font-weight: bold;
}
```

### 4. `margin`, `padding` – Spacing Outside/Inside Elements

```css
.container {
  margin: 20px;
  padding: 10px;
}
```

### 5. `border` – Border Styling

```css
div {
  border: 2px solid black;
  border-radius: 8px;
}
```

### 6. `width`, `height`

```css
img {
  width: 100px;
  height: auto;
}
```

### 7. `display` – Box Behavior

```css
span { display: inline; }
div { display: block; }
.container { display: flex; }
```

### 8. `position` and `top`, `right`, `bottom`, `left`

```css
.box {
  position: absolute;
  top: 10px;
  left: 20px;
}
```

### 9. `z-index` – Stack Order

```css
div {
  position: relative;
  z-index: 10;
}
```

### 10. `overflow` – Handle Content Overflow

```css
div {
  overflow: auto;
}
```

### 11. `cursor`

```css
a:hover {
  cursor: pointer;
}
```

### 12. `visibility`, `opacity`

```css
.hidden {
  visibility: hidden;
}
.fade {
  opacity: 0.5;
}
```

### 13. `text-align`, `text-transform`, `text-decoration`

```css
p {
  text-align: center;
  text-transform: uppercase;
  text-decoration: underline;
}
```

### 14. `box-shadow`, `text-shadow`

```css
.card {
  box-shadow: 0 4px 8px rgba(0,0,0,0.1);
}
h1 {
  text-shadow: 2px 2px 5px gray;
}
```

### 15. `transition`, `transform`, `animation`

```css
.box {
  transition: transform 0.3s;
}
.box:hover {
  transform: scale(1.1);
}
```

---

**Happy Styling! 💅**
