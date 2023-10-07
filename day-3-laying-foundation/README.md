# Laying the Foundation

In this session, we revisited previous topics and addressed any doubts raised in previous sessions. We explored Babel/Polyfills and their usage, wrote scripts for starting and building the app, and learned how to install npm packages. Additionally, we delved into the concepts of JSX, React.createElement(), and Components in depth.

## Topics Covered

- JSX
- React.createElement vs JSX
- Benefits of JSX
- Behind the Scenes of JSX
- Babel & Parcel's Role in JSX
- Components
- Functional Components
- Composing Components

## Theory

### What is JSX?

JSX stands for JavaScript XML. It's not just a string or an HTML tag; it's a syntactic sugar for the React object. JSX allows you to write HTML-like syntax inside JavaScript code to create React elements. This approach emphasizes the separation of concerns (SoC) based on loosely coupled units called 'Components,' which combine both markup and logic.

### How JSX Works

Browsers don't understand JSX, so a transpiler/compiler like Babel is needed to convert it into browser-understandable JavaScript code. Here's the flow:

JSX -> React.createElement() -> React element -> Object rendered in the DOM

### Benefits of JSX

- Easy to maintain
- Secure
- Easy to debug

### Superpowers of JSX

Using JSX, you can write markup inside JavaScript, allowing you to write logic and markup in a single .jsx file, making it easy to maintain and debug.

### JSX Expressions

You can use JSX expressions to set markup-like syntax in a variable, creating a React element (object). JSX supports all JavaScript expressions wrapped in {}.

### Attributes in JSX

In JSX, you can pass all HTML attributes inside the JSX tag, with attributes following the CamelCase convention. Custom attributes can also be created.

### Props in JSX

Props (properties) in JSX allow you to pass attribute values to a React element, making it easy to handle dynamic data.

### Role of the `type` Attribute in Script Tags

The `type` attribute in a script tag defines the type of script to run inside your app. It can have various values, such as `text/javascript`, `module`, `importmap`, `text/ecmascript`, `text/babel`, and `text/typescript`. The choice depends on the script's purpose and the browser's compatibility.

### JSX Elements vs Components

The difference between `{TitleComponent}`, `{<TitleComponent/>}`, and `{<TitleComponent></TitleComponent>}` in JSX:

- `{TitleComponent}`: Describes `TitleComponent` as a JavaScript expression or variable.
- `{<TitleComponent/>}`: Represents a component returning JSX.
- `{<TitleComponent></TitleComponent>}`: Equivalent to the previous when `TitleComponent` has no child components. Opening and closing tags are used for components with children.

## Coding Examples

- Creating a Nested Header Element using `React.createElement()`.
- Creating the same element using JSX.
- Creating a functional component with JSX.
- Passing attributes into JSX tags.
- Component composition (adding a component inside another).

## Laying the Foundation

- Initializing a Git repository with `git init`.
- Adding scripts in `package.json` to start and build the app.
- Using `npx` to run scripts.
- Adding Babel and configuring it to remove `console.log`.
- Understanding the role of keys in props.
- Clarifying that JSX is not HTML into JavaScript; it's HTML-like syntax.
- Explaining how Babel works with JSX.
- Discussing JSX expressions, React elements, and components.
- Different ways to write functional components.
- Rendering React elements vs. React components.
- Using React elements inside React components.
- Exploring component composition.


