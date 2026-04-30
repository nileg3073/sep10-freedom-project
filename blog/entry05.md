````markdown
# Entry 5
##### 03/23/26

## Content

At this point, I am still working with **React** using [react.dev](https://react.dev), but now I am starting to actually understand what I am doing a little more finally. Before, I was mostly confused and just testing random things, but now I can see how components, props, and state all connect. It is still not easy, but it feels more manageable than before.

---

## Tinkering

This week I spent more time actually building small working pieces instead of just testing random code though. But, I still used [JSBin](https://jsbin.com) & I focused more on making things connect together.

### Things I tried:
- Passing data between components using props
- Using `useState` in different components
- Creating buttons that update the screen
- Organizing my code better so it is easier to read
- Fixing repeated errors faster than before

### Example snippet (props):
```javascript
function User(props) {
  return <p>User: {props.name}</p>;
}

function App() {
  return (
    <div>
      <User name="Alex" />
      <User name="Jordan" />
    </div>
  );
}
````

This helped me understand how props pass information, learning this was hard though.

### Example snippet (state + event):

```javascript
import { useState } from "react";

function LikeButton() {
  const [likes, setLikes] = useState(0);

  return (
    <div>
      <p>Likes: {likes}</p>
      <button onClick={() => setLikes(likes + 1)}>
        Like
      </button>
    </div>
  );
}
```

This helped me understand how state updates when you interact with something. Which is extremely helpful when coding with react.

---

## Skills

### Organization

One **skill** I started developing is organizing my code. Before, my code was messy and hard to follow. Now I try to separate components and keep things cleaner so I can understand it better.

### Understanding Concepts

Another **skill** I improved is understanding concepts better. Things like props and state were confusing before, but now I can see how they actually work in my code when I test them.

---

## Engineering Design Process (EDP)

Right now I am moving from the experimenting stage into the building stage of the **engineering design process**. I am starting to finally take what I learned and use it to actually build parts of my project.

### Next Steps:

* Start putting together a basic version of my project
* Use multiple components in one app
* Keep improving how I manage state and props

---

## Sources

* [react.dev](https://react.dev)
* [jsbin.com](https://jsbin.com)

---

## Reflection

This week felt more productive than before. I am still struggling sometimes unforunately, but I can tell I am improving slowly. Things that really confused me before are starting to make a little more sense. I just need to keep practicing and building more.

---

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)

```
```
