# Exp 03 – React Lab Exercise: State in React using useState()
## NAME : Hariharan S
## REG NO: 2305001009
## Aim
To create a React application that demonstrates the use of State using the `useState()` Hook and understand how state changes update the user interface.

## Objectives
- To understand the concept of State in React.
- To create state variables using the `useState()` Hook.
- To update state using state setter functions.
- To handle button click events using `onClick`.
- To understand how changing state causes the component to re-render.
- To implement counter, student name, department, like button, and attendance applications.

## Program

### Step 1: Create a React Project
```bash
npm create vite@latest state-demo
cd state-demo
npm install
npm run dev
```

### Step 2: App.jsx
```jsx
import { useState } from "react";

function App() {
  const [count, setCount] = useState(0);
  const [name, setName] = useState("Hariharan");

  return (
    <div>
      <h1>React State Example</h1>

      <h2>Student Name: {name}</h2>

      <button onClick={() => setName("Priya")}>
        Change Name
      </button>

      <h2>Count: {count}</h2>

      <button onClick={() => setCount(count + 1)}>
        Increase
      </button>

      <button onClick={() => setCount(count - 1)}>
        Decrease
      </button>

      <button onClick={() => setCount(0)}>
        Reset
      </button>
    </div>
  );
}
export default App;
```
## Output
<img width="1920" height="914" alt="Screenshot 2026-10-26 093952" src="https://github.com/user-attachments/assets/dae7c84a-10c3-487c-b022-ac6a6e250496" />

<img width="1920" height="915" alt="Screenshot 2026-10-26 094022" src="https://github.com/user-attachments/assets/3ce45d63-1cae-46cf-9847-b9add91182a0" />


## Result
Thus, a React application was successfully created and executed using the `useState()` Hook to demonstrate state management, button click events, and dynamic user interface updates through counter, student name, department, like button, and attendance activities.
