# Chapter 8 - Let's Get Classy 🎩

Welcome to Chapter 8 of the "Namaste React" course! In this chapter, we dive into the world of class-based components, exploring their lifecycle methods, creating state variables, and passing props. Let's get started! 🚀

## Table of Contents 📑

- [Introduction](#introduction)
- [Key Topics Covered](#key-topics-covered)
- [Theory](#theory)
- [Practical Examples](#practical-examples)
- [Coding Challenges](#coding-challenges)

## Introduction 📢

In today's session, we focused on understanding class-based components, their lifecycle methods, and what's happening under the hood. It's an exciting journey, especially if you're already familiar with functional components in React.

## Key Topics Covered 🗝️

Here are the key topics we'll explore in this chapter:

| Topic                             | Description                                                |
| --------------------------------- | ---------------------------------------------------------- |
| Create Class-Based Component      | Learning to create class-based components                 |
| Pass Props                        | How to pass props from a parent to a child component       |
| State Variables in Child          | Creating state variables inside child components           |
| Lifecycle Methods in React        | Understanding the lifecycle methods in class-based comps  |
| Console Log Exploration           | Playing with console logs to determine execution sequence |
| Handling Intervals                | Using `clearInterval` to manage intervals in components    |
## Theory 📚

### Nested Routes and Sub-Nested Routes

Nested routing can be further extended to create sub-nested routes, allowing for more complex routing structures.

### Order of Lifecycle Method Calls in Class-Based Components

In class-based components, the order of lifecycle method calls is as follows:

1. `constructor()`
2. `render()`
3. `componentDidMount()`
4. `componentDidUpdate()`
5. `componentWillUnmount()`

These methods play a crucial role in managing the component's lifecycle and behavior.

### Usage of `componentDidMount`

The `componentDidMount()` method is used to execute React code when a component is already placed in the DOM. It's called during the Mounting phase after the component is rendered. It's ideal for tasks like making API calls.

### Usage of `componentWillUnmount`

`componentWillUnmount()` is essential for cleaning up resources when navigating between different routes in a Single Page Application (SPA). Failing to do so can result in performance issues, as resources may continue running in the background.

### Understanding `super(props)` in Constructor

`super(props)` is used to inherit properties and access variables from the parent React class when initializing a component. It's necessary to access this context inside the constructor.

### Async Callback Function in useEffect

`useEffect` expects its callback function to return nothing or a cleanup function. Making the callback function async can return a promise, affecting the cleanup function. To handle asynchronous operations, create a separate async function within the `useEffect` callback.

## Practical Examples 💡

In this chapter, we'll explore practical examples, including:

- Creating class-based components.
- Implementing 2 class-based child components.
- Passing props from a parent to a child.
- Utilizing the constructor.
- Managing state variables inside child components.
- Using `this.setState` for state updates.
- Handling multiple state variables.
- Exploring lifecycle methods with console logs.
- Working with intervals in `componentDidMount`.
- Using `clearInterval` to resolve interval-related issues.

## Coding Challenges 🚧

Get ready for some hands-on coding challenges! In this chapter, we'll:

- Create class-based components.
- Develop 2 class-based child components.
- Practice passing props between components.
- Leverage constructors and state variables.
- Explore the intricacies of lifecycle methods.
- Tackle interval-related issues and resolve them using `clearInterval`.

## Notes 📚

**Class-based Components**

React started with components with class-based components and there was NO functional components. Functional components became popular after the introduction of Hooks.
Class-based Components are:
- less maintainable
- little confusing
- more code
- difficult for new developer to understand
This is the right time to understand class-based components where you already know how React works and developed an app.

**Why class-based components now?**

- It's asked in interviews & already lot of old projects are still using it.

**Nesting Routes [children inside children]:**

```
localhost:1234/                  // parent
localhost:1234/about             // children
localhost:1234/about/profile     // children inside children
const appConfig = createBrowserRouter([
  {
    path: "/",
    element: <AppLayout />,     // Parent
    errorElement: <Error />,
    children: [                 // Children
      {
        path: "/",
        element: <Home />
      },
      {
        path: "/about",
        element: <About />,    
        children: [            // Children inside children
          {
            path: "profile",             // Note: we are not using "/profile"
            element: <ProfileClassComponent1 />
          },
          {
            path: "profile2",            // Note: we are not using "/profile"
            element: <ProfileFunctionalComponent1 />
          }
        ]
      },
      {
        path: "/contact",
        element: <Contact />
      },
      {
        path: "/about-class",
        element: <AboutClassComponent />
      }
    ]
  }
])
```
How to tell React it's a class based component and not a normal class.

using React.Component
```
class ProfileClass extends React.Component {

}
```
Important: without render() method, we can't create a class based component.

```
render () {
  return <h1> This is class component </h1>
}
```
How to pass props from parent to child?

while receiving in this use this.props.name

```
class ProfileClass extends React.Component {
  render() {
    return (
      <h1> This is class component </h1>
      <h3>{this.props.name}</h3>
    )
  }
}
```
How to create state ?

In Functional Component: useState() hook is used to create a state.
In Class Component, this.state is used in constructor method of class.

```
class ProfileClass extends React.Component {
  constructor(props) {
    super(props)
    this.state = {
      stateName: value
    }
  }
  
  render() {
    return <h1> This is class component </h1>
  }
}
```
Why super(props) in constructor ?

refer stackoverflow
constructor initialized the class instance

this.state = {
  stateName : value
}
How to use state ?

In Functional Components, {stateName}
In Class Component, {this.state.stateName}
How to create multiple states ?

In Functional Components:
```
const [state1] = usestate(0);
const [state2] = useState(0)
In Class Component:

this.state = {
  state1 : 0,
  state2 : 0
}
```
How to mutate state ?

In Functional Components, setStateName(newValue)
In Class Component, this.setState({ stateName: newValue })
How to mutate multiple state ?

In Functional Components, setCount1(newValue) setCount2(newvalue)
In Class Component, this.setState({ count1: newValue, count2 : newValue })
React Life Cycle: constructor() is called and then render(), then componentDidMount()

How is API call made

In FC, we use useEffect()
It renders whatever we want with the default state before API call.
After update, it re-renders again.
In CC, we write our API code inside componentDidMount() method
First, the constructor will set the default state,
Then, render(),
Then, componentDidMount() for API call
Question: In which order, the console.log output will be printed for Nested Routes -> (Parent - Child) Or In which order, the constructor(), render() & componentDidMount() will be called for Nested Routes -> (Parent - Child)

Output:

Parent: constructor
Parent: render
Child: constructor
Child: render
Child: componentDidMount
Parent: componentDidMount

In which order, the console.log output will be printed for Nested Routes -> (Parent - Child 1 - Child 2) Or In which order, the constructor(), render() & componentDidMount() will be called for Nested Routes -> (Parent - Child 1 - Child 2)*

Output:

Parent: constructor
Parent: render
child1: constructor
child1: render
child2: constructor
child2: render
child1: componentDidMount
child2: componentDidMount
Parent: componentDidMount
React Lifecycle phases 

When we render a React component, it has 2 phases: Render phase & Commit phase.

Render phase:

In this phase, the constructor() is called.
Then, render() is called.
Commit phase:

In this phase, the DOM is modified.
Then, componentDidMount() is called.
Why async can be used in componentDidMount() but not in useEffect()

refer blog & stackoverflow
Make API call in componentDidMount()
Lifecycle :

child constructor
child render
child componentDidMount
API call
setState()
render
componentDidUpdate
componentWillUnmount
componentDidMount - Called Only once in a component
componentDidUpdate - Called when the state is updated
If there is no state, there will be no componentDidUpdate