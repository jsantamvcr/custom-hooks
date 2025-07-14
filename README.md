# 🧩 Custom React Hooks

This repository contains a collection of **reusable custom React hooks** designed to simplify common tasks in React applications.

## 📁 Contents

- `useCounter.js`: Manages a counter with increment, decrement, and reset functionality.
- `useFetch.js`: Performs HTTP requests and handles loading and error states.
- `useForm.js`: Manages form state and input changes.
- `useTodo.js`: Provides utilities to manage a todo list (add, delete, toggle complete).

## 🚀 Usage

You can copy any of the hooks and use them directly in your React projects.

### Example usage with `useCounter`

```js
import useCounter from './useCounter';

function CounterComponent() {
  const { counter, increment, decrement, reset } = useCounter();

  return (
    <div>
      <h2>{counter}</h2>
      <button onClick={increment}>+1</button>
      <button onClick={decrement}>-1</button>
      <button onClick={reset}>Reset</button>
    </div>
  );
}
