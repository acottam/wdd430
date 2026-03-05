# Chapter 3: Updating UI with JavaScript

## Building with Vanilla JavaScript

### Basic DOM Manipulation Example
```javascript
// Select element by ID
const app = document.getElementById('app');

// Create new element
const header = document.createElement('h1');

// Create text content
const text = 'Develop. Preview. Ship.';
const headerContent = document.createTextNode(text);

// Append text to element
header.appendChild(headerContent);

// Add element to DOM
app.appendChild(header);
```

## HTML vs. DOM

**HTML**: Represents initial page content (source code)
**DOM**: Represents updated page content (modified by JavaScript)

The DOM can be different from the HTML source because JavaScript dynamically updates it.

## Imperative vs. Declarative Programming

### Imperative Programming
- Describes **HOW** to do something step-by-step
- Example: Step-by-step pizza recipe (mix dough, knead, spread sauce, add toppings, bake)
- Verbose and requires detailed instructions

### Declarative Programming
- Describes **WHAT** you want, not how to achieve it
- Example: Ordering a pizza (specify what you want, someone else handles details)
- Faster development, less code

## Why React?

Updating the DOM with vanilla JavaScript is powerful but verbose. As applications grow, imperative approaches become challenging to maintain.

React is a **declarative UI library** - you tell React what you want, and React figures out how to update the DOM.

## Resources
- [Manipulating Documents - MDN](https://developer.mozilla.org/docs/Learn/JavaScript/Client-side_web_APIs/Manipulating_documents)
- [HTML vs. the DOM](https://developer.chrome.com/docs/devtools/dom/#appendix)
- [Declarative UI - React Docs](https://react.dev/learn/reacting-to-input-with-state#how-declarative-ui-compares-to-imperative)
