# React Foundations Progress Tracker

## Week 1: Chapters 1-7

- [x] Chapter 1: About React and Next.js
- [x] Chapter 2: Rendering User Interfaces (UI)
- [x] Chapter 3: Updating UI with JavaScript
- [x] Chapter 4: Getting Started with React
- [x] Chapter 5: Building UI with Components
- [x] Chapter 6: Displaying Data with Props
- [x] Chapter 7: Adding Interactivity with State

## Week 2: Remaining Chapters

- [ ] Chapter 8: (To be completed next week)
- [ ] Chapter 9: (To be completed next week)
- [ ] Additional chapters as assigned

## GitHub Repository

**Repository URL**: https://github.com/acottam/wdd430/ 

## Notes

Use this space to track key learnings, questions, or challenges:

---

### Chapter 1 Notes:
- React is a library (tools), Next.js is a framework (structure + tools)
- Modern web apps need to consider: UI, routing, data fetching, rendering, integrations, infrastructure, performance, scalability, and developer experience
- Next.js handles common requirements like routing, data fetching, and caching

---

### Chapter 2 Notes:
- DOM = Document Object Model (object representation of HTML)
- DOM has a tree-like structure with parent-child relationships
- Acts as a bridge between code and UI
- Can be manipulated with JavaScript to update UI dynamically

---

### Chapter 3 Notes:
- Imperative programming = HOW to do something (step-by-step)
- Declarative programming = WHAT you want (describe outcome)
- Vanilla JavaScript DOM manipulation is verbose and challenging at scale
- React is declarative - you describe what you want, React handles the DOM updates

---

### Chapter 4 Notes:
- JSX = HTML-like syntax in JavaScript
- Babel compiles JSX to regular JavaScript
- React significantly reduces code compared to vanilla JavaScript
- Essential JS concepts: functions, arrow functions, objects, arrays, destructuring, template literals, ternary operators, ES modules

---

### Chapter 5 Notes:
- Components are functions that return UI elements
- Component names must be capitalized
- Components can be nested to create component trees
- Modular structure makes code maintainable and reusable

---

### Chapter 6 Notes:
- Props pass data from parent to child (one-way data flow)
- Props are read-only (immutable)
- Use curly braces {} to embed JavaScript in JSX
- Use array.map() to render lists
- Always include unique key prop for list items

---

### Chapter 7 Notes:
- State = data that changes over time in a component
- useState() hook manages state: const [value, setValue] = useState(initialValue)
- Event names are camelCase (onClick, onChange, onSubmit)
- State is mutable and triggers re-renders when updated
- State logic stays in the component where it was created, but can be passed as props to children

---
