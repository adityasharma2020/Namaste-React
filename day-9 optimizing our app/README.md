# Day 9 - Optimizing our App 🚀

Welcome to Day 9 of your course! In this episode, we'll dive into optimizing our app. We'll explore the use of custom hooks, lazy loading, and suspense to make our app more efficient and user-friendly. Let's get started! 🌟

## Table of Contents 📑

- [Topics Covered](#topics-covered)
- [Notes](#notes)
- [Theory](#theory)
- [Coding](#coding)
- [Quick Code Reference](#quick-code-reference)
- [References](#references)

## Topics Covered 🗝️

Today, we'll cover the following topics:

| Topic                                  | Description                                      |
| -------------------------------------- | ------------------------------------------------ |
| Custom Hooks                           | Understanding what custom hooks are and why they are useful. |
| Lazy Loading                           | Implementing lazy loading for components.       |
| Suspense                               | Exploring suspense and its role in rendering components. |
| Code Splitting                         | Understanding code splitting and its advantages and disadvantages. |
| When and Why to use `lazy()` and `suspense`? | Learning when and why to use lazy loading and suspense. |

## Notes 📚

### Theory

**When and why do we need `lazy()`?**

React.lazy() is used to dynamically import a component when it is first rendered, instead of importing at the beginning when the file loads. This is called Code Splitting/ On-demand loading. It improves performance by only loading components when they are needed.

**What is `suspense`?**

Suspense allows us to show fallback content (e.g., loading indicator) while waiting for lazy-loaded components to load or when a component is not yet rendered. It is similar to a catch block and can be used to improve the user experience during loading.

**Why we got this `error`: A component was suspended while responding to `synchronous input`. How does `suspense` fix this error?**

This error occurs when a promise for a lazy component is not yet resolved, and React expects a Suspense boundary to show a fallback. Suspense allows React to handle this situation gracefully by showing the old UI until the new UI is ready.

**Advantages and Disadvantages of using the code splitting pattern:**

| Advantages                                | Disadvantages                                 |
| ----------------------------------------- | -------------------------------------------- |
| Reduces page load time by bundling large code into smaller bundles. | Increases load time for dynamically loaded components. |
| Loads only the components that the user needs initially. | Generates many HTTP requests for dynamic loading. |
| Improves user experience with suspense fallback/loading indicators. | Requires additional code for showing the loading UI. |

**When do we need `suspense`?**

Suspense is useful when components are waiting to render, such as React.lazy components getting dynamically loaded before rendering. It is currently mainly used for dynamic component loading but may support other use cases in the future.

### Coding

In today's coding session, you'll get hands-on experience with the following:

- Creating custom hooks.
- Trying out lazy loading and suspense.
- Writing clean and optimized code for your project.

## Quick Code Reference 📝

- [Custom Hooks](utils/useRestaurantMenu.js)
- [Lazy Loading Example](App.js)
- [References](References)

## References 📖

- [React Custom Hooks](https://reactjs.org/docs/hooks-custom.html)
- [React.lazy](https://reactjs.org/docs/code-splitting.html#reactlazy)
- [Akshay Saini - Code Link](https://github.com/akshaysaini96/react-food-delivery-app)

Happy coding! 🚀✨
