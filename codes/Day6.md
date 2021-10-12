# 100 days of code, day 6

## Using the State Hook

```javascript
import React, { useState } from "react";

export default function App() {
  const [count, setCount] = useState(0);

  return (
    <div className="container">
      <h1>This is a useState() Hook Example</h1>
      <button onClick={() => setCount(count + 1)}>Click Me</button>
      <p>You clicked {count} times</p>
    </div>
  );
}
```

---

## Documentation

[The useState() Hook in React](https://reactjs.org/docs/hooks-state.html)

## Starkblitz

[Code on Starkblitz](https://stackblitz.com/edit/react-5k5akb)
