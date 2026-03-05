# Chapter 6: Displaying Data with Props

## What are Props?

Props (properties) are pieces of information passed to React components, similar to HTML attributes. They allow components to be dynamic and reusable.

**Key Concept**: Data flows **down** the component tree (one-way data flow) from parent to child.

## Using Props

### Passing Props
```jsx
function HomePage() {
  return (
    <div>
      <Header title="React" />
    </div>
  );
}
```

### Receiving Props
```jsx
function Header(props) {
  console.log(props); // { title: "React" }
  return <h1>{props.title}</h1>;
}
```

### Object Destructuring
```jsx
function Header({ title }) {
  return <h1>{title}</h1>;
}
```

## Using Variables in JSX

Use **curly braces** `{}` to embed JavaScript expressions in JSX:

### Examples
```jsx
// Object property
function Header(props) {
  return <h1>{props.title}</h1>;
}

// Template literal
function Header({ title }) {
  return <h1>{`Cool ${title}`}</h1>;
}

// Function return value
function createTitle(title) {
  return title ? title : 'Default title';
}

function Header({ title }) {
  return <h1>{createTitle(title)}</h1>;
}

// Ternary operator
function Header({ title }) {
  return <h1>{title ? title : 'Default Title'}</h1>;
}
```

## Iterating Through Lists

Use `array.map()` to render lists:

```jsx
function HomePage() {
  const names = ['Ada Lovelace', 'Grace Hopper', 'Margaret Hamilton'];

  return (
    <div>
      <Header title="Develop. Preview. Ship." />
      <ul>
        {names.map((name) => (
          <li key={name}>{name}</li>
        ))}
      </ul>
    </div>
  );
}
```

**Important**: Always include a `key` prop with a unique value for list items. This helps React identify which items have changed.

## Resources
- [Passing Props to a Component](https://react.dev/learn/passing-props-to-a-component)
- [Rendering Lists](https://react.dev/learn/rendering-lists)
- [Conditional Rendering](https://react.dev/learn/conditional-rendering)
