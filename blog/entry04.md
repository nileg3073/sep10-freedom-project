````markdown
# Entry 4
##### 03/09/26

## Content

This week, I officially picked **React** as my tool using [react.dev](https://react.dev). Honestly, this turned out to be one of the hardest tools I have worked with so far, easily a **🔥🔥🔥🔥🔥 (5/5 difficulty)**. Even though it was extremely frustrating, I still want to challenge myself and push into new things since I am really interested in **Computer Science**. I know this will help me improve in the long run.

---

## Tinkering

I did a lot of tinkering with React this week. I opened multiple [JSBin](https://jsbin.com) sessions just to test small things I was learning. A lot of the time my code did not work, especially when I tried to connect React with what I already knew about HTML and JavaScript.

### Things I tried:
- Making simple components using functions
- Trying to render elements to the page
- Using `useState` to make something interactive
- Testing different ways to structure my code
- Fixing errors that kept showing up in the console

### Example snippet:
```javascript
import { useState } from "react";

function Counter() {
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
````

This was one of the first things I got working actually. Before this, I was confused about how state actually worked, but doing small tests like this helped me understand it better for me.

---

## Skills

### Debugging

One **skill** I worked on was debugging. React gave me a lot of errors, especially when I made small mistakes. I had to read the error messages and search up what they meant. For example, when my component would not show up, I checked my imports and code structure until I found the issue.

### Problem-Solving

Another **skill** I improved was problem solving. A lot of my JSBin tests failed at first, so I had to figure out what went wrong. I started breaking my code into smaller parts and testing each part, which made it easier to find the problem.

---

## Engineering Design Process (EDP)

Right now I am in the learning and experimenting stage of the **engineering design process**. I am still trying to understand how React works before I fully use it in my project.

### Next Steps:

* Build a small React app that actually works
* Practice using components and state together
* Start adding React into my Freedom Project

---

## Sources

* [react.dev](https://react.dev)
* [jsbin.com](https://jsbin.com)

---

## Reflection

This week was hard but still productive. React confused me a lot at first, but I started to understand some basic ideas by testing things over and over. I am going to keep practicing and slowly use what I learn in my project.

---

[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)
