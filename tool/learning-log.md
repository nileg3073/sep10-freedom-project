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

### Questions

* When should I use React instead of HTML
* How React connects to CSS

---

### Next

* Try building a small React component
* Practice props more
