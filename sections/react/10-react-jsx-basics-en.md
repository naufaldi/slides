# React & JSX Basics

## Online editors

recommendation: https://codesandbox.io/s

others:

- Glitch: https://glitch.com/edit/#!/remix/starter-react-template
- CodePen: https://reactjs.org/redirect-to-codepen/hello-world

## Defining a component as a function

```jsx
import React from 'react';

const App = () => {
  return <div>Hello, World!</div>;
};

export default App;
```

## Defining a component as a class

```jsx
import React, { Component } from 'react';

class App extends Component {
  render() {
    return <div>Hello, World!</div>;
  }
}

export default App;
```

## Component definition

In order to distinguish them from ordinary tags, components start with a capital letter

## JSX: JS + XML

JSX = Template language of React

- **<** switches from JS to XML/HTML
- **{** switches back to JS

## JSX: JS + XML

```jsx
<div>A year has {365 * 24} hours</div>
```

## JSX: Simple tasks

- Show the current date
- Show either "heads" or "tails" inside a div

## JSX: Properties

we can also change from XML to JS in properties:

```jsx
<a href={'https://en.wikipedia.org/wiki/' + articleName}>
  some article
</a>
```

Note there are no quote characters around the value of _href_

## JSX: events

```jsx
const hello = () => {
  console.log('hello world');
  // ...
};
```

```jsx
<button onClick={hello}>Say Hello</button>
```

list of browser events:
https://www.w3schools.com/jsref/dom_obj_event.asp