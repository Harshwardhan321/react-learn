# react-learn 😀

Learning react and building projects

### To build websites - React Library + react-dom

### To build Apps - React Library + react-native

## Create React App

Basic way to create react app - "npx create-react-app" (Utility/software to create react app)
Note - It takes much time to install the packages. So, there is another way to install which we will dicuss later.
npx - Node package Executer

## Getting Started with vite ✌️

Vite: It is a build tool that aims to provide a faster and leaner development experience for modern web projects.

Utility: npm create vite@latest

## Custom React 🛃

**Custom Rendering Functions**:Custom rendering functions are reusable blocks of code that allow us to generate and insert HTML elements into the DOM dynamically. They're particularly useful in frameworks like React, where we often need to render components based on data or user interactions.

**Manipulating DOM Elements:** When we manipulate DOM elements, we're essentially interacting with the structure of the webpage directly using JavaScript. We can create new elements, modify their attributes or content, and insert them into the document. This process allows us to dynamically update the webpage without needing to reload the entire page.

**React-like Element Structure:** In a React-like element structure, we typically have three main properties: type, props, and children. The type property specifies the type of HTML element we want to render, such as 'div' or 'a'. The props property contains additional attributes we want to assign to the element, like 'href' or 'target'. Finally, the children property holds any nested elements or text content that should be included inside the element.

**Looping through Object Properties:** When we loop through object properties, we're iterating over each key-value pair in an object and performing some action based on those properties. In JavaScript, we can use techniques like for...in loops to iterate over an object's properties. This allows us to dynamically handle properties without needing to know them beforehand.

**Handling Props and Children:** Handling props and children is essential in React components. Props represent the data that a component receives from its parent, and children are the components or elements nested within it. We need to properly handle these props and children to ensure that our components render correctly and behave as expected.

**React Component Lifecycle:** In React, components go through a lifecycle of events from initialization to destruction. For example, componentDidMount is called after a component is rendered for the first time, while componentWillUnmount is called just before a component is removed from the DOM. Understanding these lifecycle methods allows us to perform actions at specific points in a component's lifespan, such as fetching data or cleaning up resources.

**JavaScript DOM Manipulation:** "JavaScript DOM manipulation involves using JavaScript to interact with the Document Object Model, which represents the structure of the webpage. We can create, modify, or remove DOM elements, change their attributes, styles, or content, and respond to user interactions. This allows us to create dynamic and interactive web experiences.

## Hooks 🪝

In React, hooks are functions that enable functional components to access React features such as state, lifecycle methods, context, and more. Hooks were introduced in React 16.8 to provide a way to use state and other React features without writing a class. They allow developers to reuse stateful logic across components without changing the component hierarchy.

**useState**: Allows functional components to manage local state.

**useEffect**: Enables performing side effects in functional components, such as data fetching, subscriptions, or manually changing the DOM.

**useContext**: Provides access to the nearest Context object within a functional component.

**useReducer**: An alternative to useState. It accepts a reducer function with the current state and an action to compute a new state.

**useCallback**: Returns a memoized callback function that only changes if one of the dependencies has changed.

**useMemo**: Returns a memoized value. It is similar to useCallback, but it memoizes any value (not just functions).

**useRef**: Returns a mutable ref object whose .current property is initialized to the passed argument (initialValue). The returned object will persist for the full lifetime of the component.

**useImperativeHandle**: Customizes the instance value that is exposed when using ref.

**useLayoutEffect**: Similar to useEffect, but it fires synchronously after all DOM mutations. It is useful for measurements or DOM mutations that need to happen synchronously.

**useDebugValue**: Used to display a label for custom hooks in React DevTools.

### React Fibre 🪛

Source Article : [React Fibre](https://github.com/acdlite/react-fiber-architecture)

**React Fiber** is a reimplementation of React's core algorithm aimed at improving performance and enabling new features such as animation, layout, and gestures. It introduces incremental rendering, allowing rendering work to be split into smaller chunks and spread across multiple frames.

**Key features of React Fiber include**:

**Incremental Rendering**: Splitting rendering work into smaller units and spreading it over multiple frames.
**Pause, Abort, or Reuse Work**: Ability to pause, abort, or reuse rendering work as new updates come in.
**Priority Assignment**: Assigning priority to different types of rendering updates to ensure smoother user experience.
**New Concurrency Primitives**: Introducing new concurrency primitives to handle rendering work more efficiently.

**Key Concepts**:

**Reconciliation**: The algorithm used by React to determine which parts of the UI need to be updated.
**Scheduling**: The process of determining when rendering work should be performed and assigning priority to different types of work.
**Fibers**: Lower-level abstractions representing units of rendering work in React Fiber. Fibers track component instances and their rendering output.