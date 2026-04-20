# Tool Learning Log

## Tool: **react.dev**

---

### 03/16/26:

* Learned React builds UI using components
* Saw JSX mixes HTML and JavaScript
* Noticed components return markup
* Looked at basic example from docs

```jsx
function App() {
  return <h1>Hello world</h1>;
}
```

* Realized components are just functions
* Learned React uses `className` instead of `class`
* JSX looked confusing at first

---

### 03/17/26:

* Tried reading the "Describing the UI" section
* Learned components can be reused
* Saw nesting components inside each other

```jsx
function Card() {
  return <div>Card</div>;
}

function App() {
  return <Card />;
}
```

* This felt similar to Bootstrap components
* Started understanding how pages are built from pieces

---

### 03/18/26:

* Looked at props section on react.dev
* Learned props pass data to components
* This was confusing at first

```jsx
function Card(props) {
  return <h1>{props.title}</h1>;
}
```

* A-ha moment when I saw values change per component
* React feels like reusable blocks

---


---

### 03/19/26:

* Explored **state** in React
* Learned state allows components to remember data
* Saw `useState` hook example

```jsx
import { useState } from "react";

function Counter() {
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>{count}</p>
      <button onClick={() => setCount(count + 1)}>Increase</button>
    </div>
  );
}
```

* Realized state updates re-render the component
* Excited about dynamic UIs

---

### 03/20/26:

* Looked at **events** in React
* Learned JSX uses `onClick`, `onChange` etc.
* Saw how to handle input forms

```jsx
function NameInput() {
  const [name, setName] = useState("");

  return (
    <input
      value={name}
      onChange={(e) => setName(e.target.value)}
    />
  );
}
```

* Noticed event object `e` carries info
* Felt forms are easier with controlled components

---

### 03/21/26:

* Explored **conditional rendering**
* Learned `if` and ternary operator in JSX

```jsx
function Greeting({ loggedIn }) {
  return <h1>{loggedIn ? "Welcome back!" : "Please log in"}</h1>;
}
```

* Cool to show different content dynamically
* Helps make interactive pages

---

### 03/22/26:

* Looked at **lists and keys**
* Learned `map()` to render multiple items
* Key is required for unique identification

```jsx
function List() {
  const items = ["Apple", "Banana", "Cherry"];
  return (
    <ul>
      {items.map((item, index) => (
        <li key={index}>{item}</li>
      ))}
    </ul>
  );
}
```

* Realized keys prevent rendering bugs
* Lists make data-driven UI simpler

````md
---

### 04/13/26 (Monday)

* Started learning **lifting state up**
* Learned that sometimes multiple components need the same state
* Moved state to a parent component and passed it down via props
* This helped keep data in sync

```jsx
function Parent() {
  const [value, setValue] = useState("");

  return (
    <>
      <Input value={value} onChange={setValue} />
      <Display value={value} />
    </>
  );
}
````

* Realized: state should live in the closest common parent
* This concept felt important but slightly tricky

---

### 04/15/26 (Wednesday)

* Learned about **useEffect**
* It runs side effects after render
* Example: logging or fetching data

```jsx
import { useEffect } from "react";

useEffect(() => {
  console.log("Component rendered");
}, []);
```

* Learned dependency array controls when it runs
* Empty array = run once on mount
* Without array = runs every render
* Still a bit confusing when to use it

---

### 04/17/26 (Friday)

* Explored **fetching data with useEffect**
* Tried calling an API and storing result in state

```jsx
useEffect(() => {
  fetch("https://api.example.com/data")
    .then(res => res.json())
    .then(data => setData(data));
}, []);
```

* Learned about async behavior in React
* Realized UI updates after data loads
* Starting to understand real-world usage

---

### 04/19/26 (Yesterday)

* Reviewed everything learned so far

* Focused on connecting concepts together:

  * props + state + events + effects

* Noticed patterns:

  * state = data
  * props = passing data
  * events = user interaction
  * effects = side actions

* Big realization:
  React is about **data flowing through components**

* Still unsure about:

  * When to split components
  * Best practices for useEffect

---

### Questions
* How do I structure larger apps with many components?
* When should I create custom hooks?
* How do I avoid messy useEffect logic?

---

### Next

* Build a small project (todo app or weather app)
* Practice lifting state and data flow
* Try using useEffect with real APIs

```

---
