# 📘 JavaScript Full Course - Basic to Advanced with Concepts and Examples

Welcome to the **JavaScript Full Course** README! This guide covers all essential and advanced JavaScript concepts with clean examples, usage explanations, and best practices.

---

## 🧠 1. What is JavaScript?

* JavaScript is a **lightweight**, **interpreted**, or **just-in-time compiled** programming language.
* It is most well-known as the scripting language for Web pages, enabling **dynamic content**.

```html
<script>
  alert('Hello, JavaScript!');
</script>
```

---

## 📦 2. Variables and Data Types

### 🧾 Variable Declarations:

* `var` – Function scoped (Avoid using)
* `let` – Block scoped (Preferred)
* `const` – Block scoped, constant value

### 📚 Data Types:

* Primitive: `string`, `number`, `boolean`, `null`, `undefined`, `symbol`, `bigint`
* Non-Primitive: `object`, `array`, `function`

```js
let name = "John";
const age = 25;
let isStudent = true;
```

---

## ✍️ 3. Operators

* Arithmetic: `+`, `-`, `*`, `/`, `%`, `**`
* Assignment: `=`, `+=`, `-=`, etc.
* Comparison: `==`, `===`, `!=`, `<`, `>`
* Logical: `&&`, `||`, `!`
* Ternary: `condition ? expr1 : expr2`

---

## 🔄 4. Control Flow

### 📜 Conditional Statements

```js
if (score > 50) {
  console.log("Pass");
} else {
  console.log("Fail");
}
```

### 🔁 Loops

```js
for (let i = 0; i < 5; i++) {
  console.log(i);
}

while (condition) { }
do { } while (condition);
```

---

## 🎯 5. Functions

* Function Declaration
* Function Expression
* Arrow Functions

```js
function greet(name) {
  return `Hello ${name}`;
}

const add = (a, b) => a + b;
```

---

## 🧱 6. Arrays

```js
const fruits = ["apple", "banana"];
fruits.push("orange");
fruits.pop();
fruits.forEach(f => console.log(f));
```

---

## 🗃️ 7. Objects

```js
const person = {
  name: "Alice",
  age: 30,
  greet() {
    console.log("Hi, I'm " + this.name);
  }
};
person.greet();
```

---

## 🔁 8. Higher Order Functions

* `map`, `filter`, `reduce`

```js
const nums = [1, 2, 3];
const squared = nums.map(n => n * n);
```

---

## 🌐 9. DOM Manipulation

```html
<button onclick="changeText()">Click Me</button>
<p id="demo">Hello</p>
<script>
  function changeText() {
    document.getElementById("demo").innerHTML = "Text changed!";
  }
</script>
```

---

## 📲 10. Events

```js
document.querySelector("button").addEventListener("click", () => {
  alert("Button clicked");
});
```

---

## 🌐 11. Fetch API (AJAX)

```js
fetch('https://jsonplaceholder.typicode.com/posts')
  .then(response => response.json())
  .then(data => console.log(data));
```

---

## ⏳ 12. Async/Await

```js
async function getData() {
  const res = await fetch(url);
  const data = await res.json();
  console.log(data);
}
```

---

## 🧪 13. Error Handling

```js
try {
  // risky code
} catch (error) {
  console.log(error);
} finally {
  console.log("Always runs");
}
```

---

## 🧬 14. ES6+ Features

* Template Literals: `Hello ${name}`
* Destructuring: `const {name, age} = person;`
* Spread/Rest: `[...arr]`, `(...args)`
* Default Parameters: `function(a = 10) {}`
* Optional Chaining: `obj?.prop`
* Nullish Coalescing: `a ?? "default"`

---

## 📚 15. JavaScript Interview Questions

### Q1: What is hoisting?

**A:** JavaScript moves declarations to the top before execution.

### Q2: Difference between `==` and `===`?

**A:** `==` checks value only; `===` checks value and type.

### Q3: What is a closure?

**A:** A closure is a function that remembers its outer variables even after the outer function is done executing.

### Q4: What are arrow functions?

**A:** Arrow functions are a shorthand syntax for writing functions and they don't bind `this`.

### Q5: What is the difference between `null` and `undefined`?

**A:** `null` is assigned by developer to mean empty; `undefined` means not assigned.

---

## 🔧 Project Ideas

* To-Do List App
* Calculator
* Weather App (using API)
* Quiz Game
* Form Validation
* Stopwatch/Timer

---

## 🌟 Resources

* [MDN JavaScript Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
* [W3Schools JS](https://www.w3schools.com/js/)
* [JavaScript.info](https://javascript.info/)
* [ES6 Features](https://github.com/lukehoban/es6features)

---

**Happy Coding! 🚀**
