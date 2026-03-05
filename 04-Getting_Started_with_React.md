# Chapter 4: Getting Started with React

## Adding React to Your Project

### Load React Scripts
```html
<script src="https://unpkg.com/react@18/umd/react.development.js"></script>
<script src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>
```

- **react**: Core React library
- **react-dom**: DOM-specific methods for using React with the DOM

### Using React to Render
```javascript
const app = document.getElementById('app');
const root = ReactDOM.createRoot(app);
root.render(<h1>Develop. Preview. Ship.</h1>);
```

## What is JSX?

JSX is a syntax extension for JavaScript that allows you to write HTML-like code in JavaScript.

**Example**:
```jsx
<h1>Develop. Preview. Ship.</h1>
```

**Important**: Browsers don't understand JSX natively - it needs to be compiled to JavaScript.

## Adding Babel

Babel is a JavaScript compiler that transforms JSX into regular JavaScript.

```html
<script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
<script type="text/jsx">
  const domNode = document.getElementById('app');
  const root = ReactDOM.createRoot(domNode);
  root.render(<h1>Develop. Preview. Ship.</h1>);
</script>
```

Note: Change script type to `type="text/jsx"`

## Declarative vs. Imperative Comparison

**Declarative React**:
```jsx
root.render(<h1>Develop. Preview. Ship.</h1>);
```

**Imperative JavaScript**:
```javascript
const header = document.createElement('h1');
const text = 'Develop. Preview. Ship.';
const headerContent = document.createTextNode(text);
header.appendChild(headerContent);
app.appendChild(header);
```

React reduces repetitive code significantly.

## Essential JavaScript for React

Key JavaScript concepts used in React:
- Functions and Arrow Functions
- Objects
- Arrays and array methods
- Destructuring
- Template literals
- Ternary Operators
- ES Modules and Import/Export Syntax

## Resources
- [UI Trees - React Docs](https://react.dev/learn/understanding-your-ui-as-a-tree)
- [Writing Markup with JSX](https://react.dev/learn/writing-markup-with-jsx)
- [Babel Documentation](https://babeljs.io/)
