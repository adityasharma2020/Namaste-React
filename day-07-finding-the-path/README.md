# Chapter 7 - Finding the Path 🚀

Welcome to Chapter 7 of the "Namaste React" course! In this chapter, we'll explore the exciting world of routing in React and learn how to navigate through different pages of our application. 🌐

## Table of Contents 📑

- [Recap](#recap)
- [Why Routing Matters](#why-routing-matters)
- [Key Topics Covered](#key-topics-covered)
- [Practical Examples](#practical-examples)
- [Coding Challenges](#coding-challenges)

## Recap 🔍

Before diving into routing, let's refresh our memory on some essential concepts from the previous chapter:

- `useEffect()`
- Creating components
- State management best practices

## Why Routing Matters 🛣️

Routing is a fundamental concept in modern web development. In this chapter, we'll discover why it's crucial for creating dynamic and engaging web applications. We'll also explore the concept of Single Page Applications (SPAs). 🏞️

## Key Topics Covered 🗝️

Here are the key topics we'll cover in this chapter:

| Topic                   | Description                                           |
| ----------------------- | ----------------------------------------------------- |
| Adding Images           | How to include images in your React app               |
| Shimmer Effect          | Enhancing user experience with a shimmer effect      |
| `react-router-dom`      | Introduction to the routing library                 |
| `createBrowserRoute`    | Setting up routing in your app                      |
| `RouterProvider`        | Understanding its role in routing                    |
| `<Link>`                | Creating navigation links                            |
| Error Handling          | Gracefully handling routing errors                   |
| Nested Routing          | Implementing nested routes                          |
| Dynamic Routing         | Using dynamic parameters in the path                 |
| Coding Challenges       | Enhancing the Insta Ordering App and more            |

## Practical Examples 💡

### Adding Images 🖼️

You can add images to your React app using various methods:

1. Using a full URL for web images:
   ```jsx
   <img src="https://reactjs.org/logo-og.png" alt="React Image" />


Importing images into your project:

```
import reactLogo from "./reactLogo.png";

export default function App() {
  return <img src={reactLogo} alt="React Logo" />;
}
Organizing images in a dedicated folder:


import reactLogo from "../../assets/images/reactLogo.png";

export default function App() {
  return <img src={reactLogo} alt="React Logo" />;
}
```
console.log(useState()) 🧐
When you log useState(), you'll get an array with two elements: [undefined, function]. The first element represents the initial state (undefined), and the second element is the setState function.

Understanding useEffect Without a Dependency Array 🔄
When there's no dependency array in useEffect, the callback runs every time the component renders.
An empty dependency array runs the callback once during the initial render.
Including conditions in the dependency array runs the callback on the initial render and when the condition changes.
Coding Challenges 🚧
We'll tackle some exciting coding challenges in this chapter:

Adding a shimmer effect for a smoother user interface.
Setting up routing using react-router-dom.
Creating Home, About, and Contact pages with child routes.
Handling routing errors gracefully.
Implementing a dynamic Restaurant page with variable restaurant IDs.
Bonus: Creating a login page using the Formik library.