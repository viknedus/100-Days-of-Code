# 100 days of code, day 6

## Using the State Hook

### Increment change in count

```jsx
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

### Continuous multiple calls and renders

```jsx
import React, { useState } from "react";
import "./style.css";

export default function App() {
  const [username, setUsername] = useState("");
  const [password, setPassword] = useState("");

  const printValues = (e) => {
    e.preventDefault();
    console.log(username, password);
  };

  return (
    <div className="container">
      <h1>This is a useState() Hook Example</h1>

      <h2>Multiple continuous calls and render</h2>
      <form onSubmit={printValues}>
        <label>
          Username:
          <input
            value={username}
            onChange={(event) => setUsername(event.target.value)}
            name="username"
            type="text"
          />
        </label>
        <br />
        <label>
          Password:
          <input
            value={password}
            onChange={(event) => setPassword(event.target.value)}
            name="password"
            type="password"
          />
        </label>
        <br />
      </form>
      <p>
        Username: {username} <br /> Password: {password}
      </p>
    </div>
  );
}
```

---

## Documentation

[The useState() Hook in React](https://reactjs.org/docs/hooks-state.html), [Examples](https://daveceddia.com/usestate-hook-examples/)

## Stackblitz

[Code on Stackblitz](https://stackblitz.com/edit/react-5k5akb)
