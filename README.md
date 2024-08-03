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
Example of a class component:


class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
State
State is an object that determines how a component renders and behaves. It is managed within the component (similar to variables declared within a function). When the state changes, the component re-renders.

Example of using state in a class component:


class Clock extends React.Component {
  constructor(props) {
    super(props);
    this.state = { date: new Date() };
  }

  componentDidMount() {
    this.timerID = setInterval(() => this.tick(), 1000);
  }

  componentWillUnmount() {
    clearInterval(this.timerID);
  }

  tick() {
    this.setState({
      date: new Date()
    });
  }

  render() {
    return (
      <div>
        <h1>Hello, world!</h1>
        <h2>It is {this.state.date.toLocaleTimeString()}.</h2>
      </div>
    );
  }
}
Props
Props (short for properties) are read-only attributes passed from a parent component to a child component. They allow you to pass data and event handlers down the component tree.

Example of using props in a functional component:


function Greeting(props) {
  return <h1>Hello, {props.name}</h1>;
}

function App() {
  return <Greeting name="Alice" />;
}
Conclusion
React is a powerful library for building dynamic user interfaces. By understanding the core concepts of components, state, and props, you can start creating complex applications with reusable and maintainable code. As you dive deeper into React, you'll discover more advanced features and patterns that will help you build robust and scalable applications.


Depois de adicionar o conteúdo, desça até a seção "Commit new file".

Adicione uma mensagem de commit, como "Add Introduction to React article".

Certifique-se de que a opção "Commit directly to the main branch" esteja selecionada.

Clique em "Commit new file".

4. Adicionar o Link ao Seu README Principal
Navegue até o repositório onde você deseja adicionar o link para este artigo no seu README principal.

Clique em "README.md" para editar o arquivo.

Adicione a seção de artigos mais recente com o link para o novo artigo:



## 📝 Latest Articles

| Article                       | Description                                                                                      |
|-------------------------------|--------------------------------------------------------------------------------------------------|
| 📄 [Introduction to React](https://github.com/jardelva96/introduction-to-react) | An introductory article on React, covering its core concepts, components, state, and props.      |
Adicione uma mensagem de commit, como "Add link to Introduction to React article".

