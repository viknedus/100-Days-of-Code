# 100 days of code, day 7

## The Effect Hook

### Increment in count render

```jsx
import React, { useState, useEffect } from "react";
import "./style.css";

export default function App() {
  const [count, setCount] = useState(0);

  // Similar to componentDidMount and componentDidUpdate:
  useEffect(() => {
    // update the document title using the browser API
    document.title = `you clicked ${count} times`;
  });
  return (
    <div>
      <title>jd</title>
      <h1>The Effect Hook!</h1>

      <h2>increment count render</h2>
      <button onClick={() => setCount(count + 1)}>Click to increase</button>
      <p>you clicked {count} times</p>
    </div>
  );
}
```

---

## Documentation

[The useEffect() Hook in React](https://reactjs.org/docs/hooks-effect.html)

## Stackblitz

[Code on Stackblitz](https://stackblitz.com/edit/react-hbqpc7)
