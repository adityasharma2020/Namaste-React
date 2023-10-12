# Chapter 11 - Data is the New Oil

🛢️ In Chapter 11, "Data is the New Oil," we ventured into the data layer of our application. Data is the lifeblood of our software, akin to oil, and should be harnessed wisely because it powers the engine and comes at a cost. This chapter revolved around understanding what data means in the context of React and how to pass it through the various layers of our application.

## Key Learnings

### Data in React

1. **UI Layer vs. Data Layer**: We delved into the distinction between the UI layer and the data layer. The UI layer focuses on the visual aspects, while the data layer deals with the underlying information that fuels the application.

2. **Revised State vs. Props**: We revisited the concepts of state and props in React, understanding their roles and how they impact component behavior.

3. **Prop Drilling**: Prop drilling was explained as the process of passing data through interconnected components to reach the one that requires it. This often leads to complex, lengthy, and error-prone code.

4. **Lifting State Up**: "Lifting state up" was introduced as a technique to manage and share state or data between components efficiently. This method involves passing data from child components to their parent or siblings.

### Context and State Management

1. **Accordion Creation**: We explored the creation of accordions, a UI element used for showing or hiding content. We learned both a less desirable coding approach and a good coding approach for implementing accordions.

2. **React Development Tools - Chrome Extension**: We discussed the React Developer Tools, a Chrome extension that aids in debugging. It offers insights into components, profiling, and state management using various state management solutions like React Context, Redux Store, NGRX, MobX, and Flux.

3. **React Context**: React Context was introduced as a solution for global state management. We explored its key components, including creating context, using context with hooks (useContext), and using context in class-based components (using `<ContextName.Consumer>`). Context was shown to provide a central repository for data that can be accessed throughout the application.

### Debugging Data

1. **Displaying Context Name**: During debugging, we discussed how to display the name of a context in the browser console using `ContextName.displayName = "Name"` in the context provider. This helps in identifying and distinguishing different contexts.

## Additional Notes

### Prop Drilling

- **What is Prop Drilling?**: Prop drilling is the process of passing data from one component through a series of interconnected components to reach the component that requires it. It often results in lengthy and complex code.

- **Drawbacks of Prop Drilling**: Prop drilling leads to code that is hard to maintain, increases the chances of errors, and makes refactoring a challenge.

### Lifting State Up

- **When to Use Lifting State Up?**: Lifting state up is a technique used when data needs to be passed from a child component to its parent or its siblings. It ensures that there's a single source of truth maintained by the parent.

- **Example**: Lifting state up can be employed to pass data from a child to a parent or from a child to its siblings. For example, in an application, marked favorite restaurant card data can be passed from a child to the Body component.

### Context Provider and Consumer

- **React Context**: The React Context API offers a way to pass data through multiple levels of components without manually forwarding the data at each level. It serves as a form of global state management.

- **Three Steps of Working with Context**:
  1. Create the Context using `createContext()` and export it from a file.
  2. Provide Context by wrapping the required components with a context provider.
  3. Use the Context by importing the `useContext` hook and the created context, creating a variable to store and utilize this context.

### Default Value in Context

- **Default Value**: When we don't provide a value to the context provider, the default value is not passed as the value to components. React throws an error in such cases.

- **Usage**: If no value needs to be passed, you must mention `value={undefined}` in the provider. The default value is used only when a component does not have a matching provider above it in the component tree.

🚀 Understanding data management is essential for building robust and efficient applications. With knowledge of prop drilling, lifting state up, and React Context, you'll be well-equipped to manage data effectively and provide a seamless user experience in your applications.

