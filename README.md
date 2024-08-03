# Introduction to React

React is a popular JavaScript library for building user interfaces, especially single-page applications. It allows developers to create reusable UI components and manage the state of those components efficiently. This article will introduce you to the core concepts of React, including components, state, and props.

## What is React?

React is a JavaScript library developed by Facebook. It is used to build user interfaces by creating reusable components. React follows a declarative approach, making it easier to reason about your application and aim for a predictable and efficient way to update and render your UI.

## Core Concepts

### Components

Components are the building blocks of a React application. A component is a self-contained module that renders some output. You can think of a component as a JavaScript function that returns HTML. Components can be classified into two types:

- **Functional Components:** These are simple JavaScript functions that return JSX (JavaScript XML). They are also known as stateless components.
- **Class Components:** These are ES6 classes that extend from `React.Component` and have a `render` method. They can hold and manage state.

Example of a functional component:

```jsx
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
