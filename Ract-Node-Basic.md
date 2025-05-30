# 📘 React.js & Node.js Full Course - Basic to Advanced with Concepts and Examples

Welcome to the **React.js & Node.js Full Course** README! This guide covers all essential and advanced concepts with clean examples, usage explanations, and best practices.

---

## ⚛️ React.js Concepts

### 🧠 1. What is React?
* A JavaScript library for building **user interfaces**.
* Developed and maintained by **Meta (Facebook)**.
* Uses a component-based architecture and virtual DOM.

```bash
npx create-react-app my-app
cd my-app
npm start
```

---

### 🧩 2. JSX (JavaScript XML)
* Syntax extension to JavaScript used with React.
* Looks like HTML, but compiles to `React.createElement()`.

```jsx
const element = <h1>Hello, JSX!</h1>;
```

---

### 🧱 3. Components
* Functional and Class-based components.
* Functional components use Hooks.

```jsx
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
```

---

### 🔄 4. Props and State
* **Props**: Read-only, passed from parent to child.
* **State**: Managed within the component.

```jsx
const [count, setCount] = useState(0);
```

---

### 🔁 5. Lifecycle Methods / useEffect
* `useEffect` mimics lifecycle methods like `componentDidMount`, `componentDidUpdate`, and `componentWillUnmount`.

```jsx
useEffect(() => {
  console.log('Component mounted');
}, []);
```

---

### 🧠 6. Handling Events
```jsx
<button onClick={() => alert('Clicked!')}>Click Me</button>
```

---

### 📦 7. Conditional Rendering
```jsx
{isLoggedIn ? <Logout /> : <Login />}
```

---

### 📚 8. Lists and Keys
```jsx
{items.map(item => <li key={item.id}>{item.name}</li>)}
```

---

### 🧪 9. Forms Handling
```jsx
<input value={name} onChange={(e) => setName(e.target.value)} />
```

---

### 🌐 10. React Router
```bash
npm install react-router-dom
```
```jsx
<BrowserRouter>
  <Routes>
    <Route path="/home" element={<Home />} />
  </Routes>
</BrowserRouter>
```

---

### 📦 11. useContext & useReducer
```jsx
const ThemeContext = createContext();
const theme = useContext(ThemeContext);
```

---

### 🧩 12. Custom Hooks
```jsx
function useCounter(initial) {
  const [count, setCount] = useState(initial);
  return [count, () => setCount(count + 1)];
}
```

---

### 💅 13. Styling in React
* CSS, inline styles, CSS Modules, Styled-Components.

---

### ⚙️ 14. React Performance Optimization
* `React.memo`, `useMemo`, `useCallback`, Lazy Loading.

---

## 🚀 Node.js Concepts

### 🧠 1. What is Node.js?
* A JavaScript runtime built on Chrome's V8 engine.
* Allows running JS code on the server.

```bash
node index.js
```

---

### 📦 2. Modules
```js
const fs = require('fs');
```
* Built-in, custom, and third-party modules (npm).

---

### 🔃 3. Asynchronous Programming
* Callbacks, Promises, Async/Await

```js
fs.readFile('file.txt', (err, data) => {
  if (err) throw err;
  console.log(data);
});
```

---

### 🌐 4. Creating HTTP Server
```js
const http = require('http');
const server = http.createServer((req, res) => {
  res.end('Hello World');
});
server.listen(3000);
```

---

### 🧩 5. Express.js Basics
```bash
npm install express
```
```js
const express = require('express');
const app = express();
app.get('/', (req, res) => res.send('Home'));
app.listen(3000);
```

---

### 🗃️ 6. Middleware
```js
app.use(express.json());
```

---

### 📦 7. REST API with Express
```js
app.get('/api/users', (req, res) => res.json(users));
```

---

### 🧬 8. CRUD Operations
* Create (POST), Read (GET), Update (PUT), Delete (DELETE)

---

### 💾 9. MongoDB & Mongoose
```bash
npm install mongoose
```
```js
mongoose.connect('mongodb://localhost:27017/mydb');
```

---

### 🔐 10. Authentication (JWT, bcrypt)
```bash
npm install jsonwebtoken bcrypt
```

---

### ⚙️ 11. Error Handling
```js
app.use((err, req, res, next) => {
  res.status(500).send('Something broke!');
});
```

---

## 🧪 Project Ideas
* Blog App (MERN)
* To-Do List
* E-commerce Site
* Chat App with Socket.io
* Authentication System

---

## 🌟 Resources
* [React Docs](https://reactjs.org/docs/getting-started.html)
* [Node.js Docs](https://nodejs.org/en/docs)
* [Express Docs](https://expressjs.com/)
* [MongoDB Docs](https://www.mongodb.com/docs/)

---

**Happy Full Stack Coding! 🚀**
