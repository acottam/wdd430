# Chapter 5: Building UI with Components

## React Core Concepts
1. Components
2. Props
3. State

## What are Components?

Components are self-contained, reusable building blocks of UI. Think of them as LEGO bricks that can be combined to form larger structures.

**Benefits**:
- Modular and maintainable code
- Reusable across the application
- Easy to update without affecting other parts

## Creating Components

### Component Rules
1. Components are **functions** that return UI elements
2. Component names must be **capitalized**
3. Use components like HTML tags with angle brackets `<Component />`

### Example
```jsx
function Header() {
  return <h1>Develop. Preview. Ship.</h1>;
}

const root = ReactDOM.createRoot(app);
root.render(<Header />);
```

## Nesting Components

Components can be nested inside each other:

```jsx
function Header() {
  return <h1>Develop. Preview. Ship.</h1>;
}

function HomePage() {
  return (
    <div>
      <Header />
    </div>
  );
}

const root = ReactDOM.createRoot(app);
root.render(<HomePage />);
```

## Component Trees

Applications are structured as component trees:
- Top-level component (e.g., `HomePage`)
- Child components (e.g., `Header`, `Article`, `Footer`)
- Nested children (e.g., `Logo`, `Title`, `Navigation` inside `Header`)

This modular format allows component reuse throughout the app.

## Resources
- [Your First Component - React Docs](https://react.dev/learn/your-first-component)
- [Importing and Exporting Components](https://react.dev/learn/importing-and-exporting-components)
