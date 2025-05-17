# 🌐 HTML Full Course - Basic to Advanced with Tags, Properties, and Examples

Welcome to the **HTML Full Course**! This GitHub README provides a complete, topic-wise breakdown of HTML from basic to advanced concepts with tag descriptions, attributes, and usage examples.

---

## 🧠 1. What is HTML?

- HTML stands for Hyper Text Markup Language
- HTML is the standard markup language for creating Web pages
- HTML describes the structure of a Web page
- HTML consists of a series of elements
- HTML elements tell the browser how to display the content
- HTML elements label pieces of content such as "this is a heading", "this is a paragraph", "this is a link", etc.

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

- `<!DOCTYPE html>`: Defines that this document is an HTML5 document
- `<html>`: Root element of an HTML page
- `<head>`: Contains meta information about the HTML page
- `<title>`: Specifies a title for the HTML page
- `<body>`: Container for all visible contents
- `<h1>`: Defines a large heading
- `<p>`: Defines a paragraph

---

## 📑 3. Structural & Semantic Tags

| Tag         | Description                        |
| ----------- | ---------------------------------- |
| `<html>`    | Root element                       |
| `<head>`    | Container for metadata             |
| `<title>`   | Title of the document              |
| `<body>`    | Main content container             |
| `<header>`  | Introductory content or navigation |
| `<nav>`     | Navigation links                   |
| `<main>`    | Main content area                  |
| `<section>` | Thematic grouping of content       |
| `<article>` | Self-contained content block       |
| `<aside>`   | Tangential content (sidebars)      |
| `<footer>`  | Footer content                     |
| `<div>`     | Generic container                  |
| `<span>`    | Inline container                   |

---

## ✍️ 4. Text Formatting Tags

```html
<p>This is a <strong>bold</strong> and <em>emphasized</em> text.</p>
```

| Tag        | Description                        |
| ---------- | ---------------------------------- |
| `<p>`      | Paragraph tag                      |
| `<br>`     | Line break                         |
| `<hr>`     | Horizontal rule                    |
| `<b>`      | Bold text (non-semantic)           |
| `<strong>` | Bold text (semantic: important)    |
| `<i>`      | Italic text (non-semantic)         |
| `<em>`     | Emphasized text (semantic)         |
| `<u>`      | Underlined text                    |
| `<mark>`   | Highlighted text                   |
| `<small>`  | Smaller text                       |
| `<sub>`    | Subscript text                     |
| `<sup>`    | Superscript text                   |
| `<ins>`    | Inserted text                      |
| `<del>`    | Deleted text                       |

---

## 🔖 5. HTML Elements & Global Attributes

### HTML Element Structure:

**Opening Tag + Content + Closing Tag**

### 🌍 Common Global Attributes:

- `id`, `class`, `style`, `title`, `hidden`, `lang`

```html
<div id="box" class="container" style="color: red;">Hello</div>
```

---

## 🔗 6. Links and Anchors

```html
<a href="https://example.com" target="_blank" title="Go to Example">Visit Site</a>
```

- `href`: URL
- `target`: `_blank`, `_self`
- `title`: Tooltip text

Anchor link:

```html
<a href="#section1">Jump to Section 1</a>
```

---

## 🖼️ 7. Images

```html
<img src="image.jpg" alt="Description" width="300" height="200">
```

- `src`: Image source path
- `alt`: Alternate text
- `width`, `height`: Size attributes

---

## 📋 8. Lists

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

### List Tags Table

| Tag    | Description                |
| ------ | -------------------------- |
| `<ul>` | Unordered list             |
| `<ol>` | Ordered list               |
| `<li>` | List item                  |
| `<dl>` | Description list           |
| `<dt>` | Term in a description list |
| `<dd>` | Description of the term    |

---

## 📊 9. Tables

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

### Table Tags

| Tag          | Description               |
| ------------ | ------------------------- |
| `<table>`    | Table container           |
| `<tr>`       | Table row                 |
| `<td>`       | Table data cell           |
| `<th>`       | Table header cell         |
| `<thead>`    | Header section            |
| `<tbody>`    | Body section              |
| `<tfoot>`    | Footer section            |
| `<caption>`  | Table title               |
| `<colgroup>` | Group table columns       |
| `<col>`      | Column formatting         |

---

## 📝 10. Forms

```html
<form action="submit.php" method="POST">
  <label>Name: <input type="text" name="username"></label>
  <input type="submit" value="Submit">
</form>
```

### Tags Used:

- `<form>`, `<input>`, `<label>`, `<textarea>`, `<select>`, `<option>`, `<button>`

---

## 🔤 11. Input Types and Attributes

### Common Types:

- `text`, `email`, `password`, `number`, `checkbox`, `radio`, `file`, `date`, `range`, `color`

### Common Attributes:

- `placeholder`, `required`, `readonly`, `disabled`, `min`, `max`, `step`

```html
<input type="email" placeholder="Enter email" required>
```

---

## 🔘 12. Form Tags Reference

| Tag          | Description                     |
| ------------ | ------------------------------- |
| `<form>`     | Form container                  |
| `<input>`    | Input field                     |
| `<textarea>` | Multiline input                 |
| `<label>`    | Label for input                 |
| `<button>`   | Button                          |
| `<select>`   | Dropdown list                   |
| `<option>`   | Option in dropdown              |
| `<optgroup>` | Grouping dropdown options       |
| `<fieldset>` | Group related fields            |
| `<legend>`   | Caption for `<fieldset>`        |
| `<datalist>` | Suggestion list for input       |
| `<output>`   | Output from a calculation       |

---

## 🎵 13. Audio and Video

```html
<audio controls>
  <source src="audio.mp3" type="audio/mpeg">
</audio>

<video controls width="400">
  <source src="video.mp4" type="video/mp4">
</video>
```

---

## 📷 14. Media Tags

| Tag        | Description                                     |
| ---------- | ----------------------------------------------- |
| `<img>`    | Embed image                                     |
| `<audio>`  | Embed audio                                     |
| `<video>`  | Embed video                                     |
| `<source>` | Media source                                    |
| `<track>`  | Subtitles for media                             |
| `<iframe>` | Embed external content                          |
| `<embed>`  | Embed application                               |
| `<object>` | Embed external resource                         |

---

## 🧭 15. IFrames

```html
<iframe src="https://example.com" width="600" height="400" frameborder="0" allowfullscreen></iframe>
```

---

## 🔍 16. Meta Tags

```html
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="HTML course">
```

---

## &️⃣ 17. HTML Entities

```html
&copy;, &nbsp;, &lt;, &gt;, &amp;, &quot;, &apos;
```

---

## 📦 18. Block vs Inline Elements

### Block Elements:

- `<div>`, `<p>`, `<section>`, `<article>`, `<table>`, `<form>`

### Inline Elements:

- `<span>`, `<a>`, `<img>`, `<b>`, `<i>`, `<input>`

---

## ⚙️ 19. HTML5 APIs Overview

### 🌍 Geolocation API

```javascript
navigator.geolocation.getCurrentPosition(function(position) {
  console.log("Latitude: " + position.coords.latitude);
});
```

### 💾 Web Storage API

```javascript
localStorage.setItem("username", "John");
console.log(localStorage.getItem("username"));
```
