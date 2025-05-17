# 🌐 HTML Full Course - Basic to Advanced with Tags, Properties, and Examples

Welcome to the **HTML Full Course**! This GitHub README provides a complete, topic-wise breakdown of HTML from basic to advanced concepts with tag descriptions, attributes, and usage examples.

---

## 🧠 1. What is HTML?

* HTML stands for Hyper Text Markup Language
* HTML is the standard markup language for creating Web pages
* HTML describes the structure of a Web page
* HTML consists of a series of elements
* HTML elements tell the browser how to display the content
* HTML elements label pieces of content such as "this is a heading", "this is a paragraph", "this is a link", etc.

---

## 🧱 2. HTML Basic Structure

```html
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```

### 🔖 Tags Used

* The <!DOCTYPE html> declaration defines that this document is an HTML5 document
* The <html> element is the root element of an HTML page
* The <head> element contains meta information about the HTML page
* The <title> element specifies a title for the HTML page (which is shown in the browser's title bar or in the page's tab)
* The <body> element defines the document's body, and is a container for all the visible contents, such as headings, paragraphs, images, hyperlinks, tables, lists, etc.
* The <h1> element defines a large heading
* The <p> element defines a paragraph

---

## ✍️ 3. Text Formatting Tags

```html
<h1>Heading 1</h1>
<p>This is a paragraph.</p>
<b>Bold</b>
<i>Italic</i>
<u>Underline</u>
<mark>Highlighted</mark>
<sup>Superscript</sup>
<sub>Subscript</sub>
<small>Small text</small>
```

### 🔧 Use:

For formatting and styling textual content.

---

## 🔖 4. HTML Elements & Attributes

**HTML Element = Opening Tag + Content + Closing Tag**

### 🌍 Global Attributes

* `id`: Unique identifier
* `class`: For CSS/JS styling
* `style`: Inline CSS
* `title`: Tooltip
* `hidden`: Hides element
* `lang`: Language of content

```html
<div id="box" class="container" style="color: red;">Hello</div>
```

---

## 🔗 5. Links and Anchors

```html
<a href="https://example.com" target="_blank" title="Go to Example">Visit Site</a>
```

### 🔧 Attributes:

* `href`: URL
* `target`: `_blank`, `_self`
* `title`: Tooltip on hover

Anchor Link:

```html
<a href="#section1">Jump to Section 1</a>
```

---

## 🖼️ 6. Images

```html
<img src="image.jpg" alt="Description" width="300" height="200">
```

### 🔧 Attributes:

* `src`: Image file path
* `alt`: Alternate text
* `width`/`height`: Size

---

## 📋 7. Lists

### Ordered List:

```html
<ol>
  <li>Item 1</li>
  <li>Item 2</li>
</ol>
```

### Unordered List:

```html
<ul>
  <li>Item A</li>
  <li>Item B</li>
</ul>
```

### Description List:

```html
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language</dd>
</dl>
```

---

## 📊 8. Tables

```html
<table border="1">
  <tr>
    <th>Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Alice</td>
    <td>25</td>
  </tr>
</table>
```

### 🔖 Tags:

* `<table>`, `<tr>`, `<td>`, `<th>`
* `<caption>`, `<thead>`, `<tbody>`, `<tfoot>`

---

## 📝 9. Forms

```html
<form action="submit.php" method="POST">
  <label>Name: <input type="text" name="username"></label>
  <input type="submit" value="Submit">
</form>
```

### 🔖 Tags:

* `<form>`, `<input>`, `<label>`, `<textarea>`, `<select>`, `<option>`, `<button>`

---

## 🔤 10. Input Types and Attributes

### Input Types:

* `text`, `email`, `password`, `number`
* `checkbox`, `radio`, `file`, `date`, `range`, `color`

### Common Attributes:

* `placeholder`, `required`, `readonly`, `disabled`, `min`, `max`, `step`

```html
<input type="email" placeholder="Enter email" required>
```

---

## 🧩 11. Semantic HTML Tags

```html
<header>Header Content</header>
<nav>Navigation</nav>
<main>Main Content</main>
<article>Article Content</article>
<section>Section Content</section>
<footer>Footer Info</footer>
```

### 📌 Use:

Improves SEO and accessibility.

---

## 🎵 12. Audio and Video

```html
<audio controls>
  <source src="audio.mp3" type="audio/mpeg">
</audio>

<video controls width="400">
  <source src="video.mp4" type="video/mp4">
</video>
```

---

## 🧭 13. IFrames

```html
<iframe src="https://example.com" width="600" height="400" frameborder="0" allowfullscreen></iframe>
```

---

## 🔍 14. Meta Tags

```html
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="HTML course">
```

---

## &️⃣ 15. HTML Entities

```html
&copy;, &nbsp;, &lt;, &gt;, &amp;, &quot;, &apos;
```

### 📌 Use:

Displays special/reserved characters.

---

## 📦 16. Block vs Inline Elements

### Block:

* `<div>`, `<p>`, `<section>`, `<article>`, `<table>`, `<form>`

### Inline:

* `<span>`, `<a>`, `<img>`, `<b>`, `<i>`, `<input>`

---

## ⚙️ 17. HTML5 APIs (Overview)

### 🔍 Geolocation API

Used to get the user's geographical location.

```javascript
navigator.geolocation.getCurrentPosition(function(position) {
  console.log("Latitude: " + position.coords.latitude);
});
```

### 💾 Web Storage API

Used to store data in the browser.

#### `localStorage`

* Stores data with **no expiration**.
* Data persists even after browser is closed.

```javascript
localStorage.setItem("username", "John");
console.log(localStorage.getItem("username"));
```

#### `sessionStorage`

* Stores data only for the **session**.
* Data is cleared when tab is closed.

```javascript
sessionStorage.setItem("token", "abc123");
console.log(sessionStorage.getItem("token"));
```

### 🎨 Canvas API

Used to draw graphics directly in the browser.

```html
<canvas id="myCanvas" width="200" height="100"></canvas>
<script>
  const canvas = document.getElementById("myCanvas");
  const ctx = canvas.getContext("2d");
  ctx.fillStyle = "blue";
  ctx.fillRect(20, 20, 150, 50);
</script>
```

### 🧲 Drag and Drop API

Used to implement drag-and-drop functionality.

```html
<div id="dragMe" draggable="true">Drag me</div>
```

```javascript
document.getElementById("dragMe").addEventListener("dragstart", function(event) {
  event.dataTransfer.setData("text/plain", "Dragged Content");
});
```

---

## 🧠 18. Best Practices

* Use semantic elements
* Validate code with validators
* Add `alt` text for images
* Separate structure (HTML), style (CSS), logic (JS)
* Use indentation and comments

---

## 💡 19. Project Ideas

* Personal Portfolio
* Resume Webpage
* Contact Form
* Product Landing Page
* Blog Layout
* Image Gallery

---

## 📚 Resources

* [MDN Web Docs - HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
* [W3Schools HTML](https://www.w3schools.com/html/)
* [HTML Reference](https://htmlreference.io/)


