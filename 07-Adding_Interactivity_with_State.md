# Chapter 7: Adding Interactivity with State

## Event Handling

### Listening to Events
React uses camelCase event names:
```jsx
<button onClick={handleClick}>Like</button>
```

Common events:
- `onClick` - button clicks
- `onChange` - input field changes
- `onSubmit` - form submissions

### Handling Events
```jsx
function HomePage() {
  function handleClick() {
    console.log("increment like count");
  }

  return (
    <div>
      <button onClick={handleClick}>Like</button>
    </div>
  );
}
```

## State and Hooks

**State**: Information in your UI that changes over time, usually triggered by user interaction.

**Hooks**: Functions that add additional logic (like state) to components.

## Using useState()

The `useState()` hook manages state in React components.

### Syntax
```jsx
const [stateValue, setStateValue] = React.useState(initialValue);
```

### Example: Like Button
```jsx
function HomePage() {
  const [likes, setLikes] = React.useState(0);

  function handleClick() {
    setLikes(likes + 1);
  }

  return (
    <div>
      <button onClick={handleClick}>Likes ({likes})</button>
    </div>
  );
}
```

### useState() Breakdown
- **First item**: State value (e.g., `likes`)
- **Second item**: Update function (e.g., `setLikes`)
- **Argument**: Initial value (e.g., `0`)

## Props vs. State

**Props**:
- Passed from parent to child
- Read-only (immutable)
- Used to configure components

**State**:
- Managed within a component
- Mutable (can be updated)
- Triggers re-render when changed
- Logic for updating state stays in the component where it was created

## Key Principle
State can be passed to child components as props, but the logic for updating state should remain in the component where state was initially created.

## Resources
- [State: A Component's Memory](https://react.dev/learn/state-a-components-memory)
- [Meet Your First Hook](https://react.dev/learn/state-a-components-memory#meet-your-first-hook)
- [Responding to Events](https://react.dev/learn/responding-to-events)
- [Adding Interactivity](https://react.dev/learn/adding-interactivity)
- [Managing State](https://react.dev/learn/managing-state)
