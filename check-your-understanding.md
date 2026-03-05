# Check Your Understanding - JavaScript to React

## Questions and Answers

### What is the DOM?
The Document Object Model (DOM) is a programming interface for web documents. It represents the page structure as a tree of objects that can be manipulated with JavaScript. Each HTML element becomes a node in this tree, allowing developers to dynamically update content, structure, and styles.

### What is the difference between Imperative vs Declarative Programming?
**Imperative Programming**: You describe HOW to do something step-by-step.
- Example: Step-by-step instructions on how to make a pizza (mix dough, knead for 10 minutes, spread sauce, add toppings, bake at 450°F for 15 minutes)

**Declarative Programming**: You describe WHAT you want, not how to achieve it.
- Example: Just ordering a pizza (you specify what you want, someone else handles the details)

In React, you declare what the UI should look like based on the current state, and React handles the DOM updates.

### What is JSX – the syntax extension for JavaScript?
JSX (JavaScript XML) is a syntax extension that allows you to write HTML-like code directly in JavaScript. It makes React components more readable by combining markup and logic in the same file.

Example:
```jsx
const element = <h1>Hello, world!</h1>;
```

JSX gets compiled to regular JavaScript function calls that create React elements.

### What is the Babel interpreter?
Babel is a JavaScript compiler (transpiler) that converts modern JavaScript and JSX into backwards-compatible JavaScript that browsers can understand. It transforms JSX syntax into `React.createElement()` calls and converts newer JavaScript features into older syntax for broader browser support.

### What is the difference between props and state?
**Props (Properties)**:
- Data passed FROM parent TO child components
- Read-only (immutable) - cannot be modified by the receiving component
- Used to configure components and pass data down the component tree

**State**:
- Data managed WITHIN a component
- Mutable - can be updated using setState or useState
- When state changes, the component re-renders
- Used for data that changes over time (user input, toggles, counters, etc.)
