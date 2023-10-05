
# Lecture Notes: 04 - Coding in React 👨‍💻

## Overview 📚
We embarked on a journey to develop a config-driven UI for a food ordering platform. Throughout this lecture, we explored React fundamentals, delved into the concept of the Virtual DOM, understood the importance of Props and Keys, and explored the world of Config Driven UI. This knowledge is essential for aspiring frontend developers, backend developers, software engineers, and full-stack engineers. Let's dive into the topics covered:

## Table of Contents 📋
- [React Basics](#react-basics)
- [Virtual DOM](#virtual-dom)
- [Reconciliation](#reconciliation)
- [React Fiber](#react-fiber)
- [Why Do We Need Keys in React?](#why-do-we-need-keys-in-react)
- [Props in React](#props-in-react)
- [Config Driven UI](#config-driven-ui)
- [JavaScript: Map() vs forEach()](#javascript-map-vs-foreach)
- [JavaScript: Optional Chaining (?.)](#javascript-optional-chaining)

## React Basics 🚀
<details>
  <summary>Is `JSX` mandatory for React? 🤔</summary>
  No, JSX is not mandatory. It's syntactic sugar for calling `React.createElement()`. Plain JavaScript can also be used.
</details>

<details>
  <summary>Is `ES6` mandatory for React? 🤔</summary>
  ES6 is not mandatory but highly recommended. Modern React projects often use ES6 features.
</details>

<details>
  <summary>`{TitleComponent}` vs `{< TitleComponent/>}` vs `{< TitleComponent>}` in `JSX` 🤯</summary>
  <table>
    <tr>
      <th>Expression</th>
      <th>Description</th>
    </tr>
    <tr>
      <td>{TitleComponent}</td>
      <td>Represents TitleComponent as a JavaScript expression or variable.</td>
    </tr>
    <tr>
      <td>{TitleComponent()}</td>
      <td>Renders TitleComponent by calling it as a function.</td>
    </tr>
    <tr>
      <td>{< TitleComponent/>}</td>
      <td>Renders TitleComponent using Self Closing Tag.</td>
    </tr>
    <tr>
      <td>{< TitleComponent></ TitleComponent>}</td>
      <td>Renders TitleComponent using Normal Tag.</td>
    </tr>
  </table>
</details>

<details>
  <summary>How can I write comments in JSX? 📝</summary>
  In JSX, comments are written similar to JavaScript. Use `{/* */}` for multi-line comments.
</details>

<details>
  <summary>What is `< React.Fragment>` and `<>`? 🧩</summary>
  `<></>` is a shorthand for `<React.Fragment></React.Fragment>`. It groups children without adding extra DOM nodes.
</details>

## Virtual DOM 🌐
<details>
  <summary>What is `Virtual DOM` in React? 🌟</summary>
  Virtual DOM is a lightweight abstraction of the real DOM. It improves React's performance through efficient updates.
</details>

<details>
  <summary>Difference between `Virtual DOM` and `Real DOM`? 🔄</summary>
  <table>
    <tr>
      <th>Feature</th>
      <th>Virtual DOM</th>
      <th>Real DOM</th>
    </tr>
    <tr>
      <td>DOM Manipulation</td>
      <td>Efficient</td>
      <td>Slower</td>
    </tr>
    <tr>
      <td>Memory Usage</td>
      <td>Low</td>
      <td>High</td>
    </tr>
    <tr>
      <td>Direct HTML Update</td>
      <td>No</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td>Updates</td>
      <td>Fast</td>
      <td>Slower</td>
    </tr>
  </table>
</details>

<details>
  <summary>What is `Reconciliation` in React? 🔄</summary>
  Reconciliation is the process of comparing and updating the Real DOM efficiently in React.
</details>

<details>
  <summary>What is `React Fiber`? 🌐</summary>
  React Fiber is the new reconciliation engine in React 16. It allows for features like incremental rendering.
</details>

<details>
  <summary>Why do we need `keys` in React? 🔑</summary>
  Keys are used to identify changed, updated, or deleted items in lists, ensuring efficient updates.
</details>

<details>
  <summary>Can we use `index as keys` in React? ⚠️</summary>
  Yes, but it's not recommended as it can cause issues with component state and performance.
</details>

## Props in React 🎁
<details>
  <summary>What is `props` in React? 🎁</summary>
  Props (properties) are arguments passed into React components, enabling data flow between parent and child components.
</details>

<details>
  <summary>Ways to pass and receive `props` in React 📤 📥</summary>
  <table>
    <tr>
      <th>Passing Props to Component</th>
      <th>Receiving Props in Another Component</th>
    </tr>
    <tr>
      <td>{`<Profile name="Harshi" age={28} />`}</td>
      <td>{`const Profile = (props) => { let name = props.name; let age = props.age; }`}</td>
    </tr>
    <tr>
      <td>{`<Profile name="Harshi" age={28} />`}</td>
      <td>{`const Profile = ({name, age}) => { }`}</td>
    </tr>
    <tr>
      <td>{`<Profile {...props} />`}</td>
      <td>{`const Profile = ({name, age}) => { }`}</td>
    </tr>
  </table>
</details>

## Config Driven UI ⚙️
<details>
  <summary>What is `Config Driven UI`? ⚙️</summary>
  Config-driven UI is a pattern where the UI is rendered based on configuration parameters from the server.
</details>

## JavaScript: Map() vs forEach() 🔄
<details>
  <summary>JavaScript: Map() vs forEach() 🔄</summary>
  <table>
    <tr>
      <th>Method</th>
      <th>Description</th>
    </tr>
    <tr>
      <td>map()</td>
      <td>Returns a new array, ideal for transforming data.</td>
    </tr>
    <tr>
      <td>forEach()</td>
      <td>Does not return a new array,

 used for looping.</td>
    </tr>
  </table>
</details>

## JavaScript: Optional Chaining (?.) 🛡️
<details>
  <summary>JavaScript: Optional Chaining (?.) 🛡️</summary>
  Optional chaining (`?.`) safely accesses nested object properties. It short-circuits to undefined if properties are undefined or null.
</details>

Certainly! Here's the continuation of your README file to include the code implementation part of building a Food Ordering App using React:

---

## Code Implementation 🚀

In this section, we will walk through the code implementation for building a Food Ordering App step by step.

### Step 1: Recap on Chapter-03

We start by recapping some key concepts from Chapter-03, including functional components and React elements.

### Step 2: Creating the Food Ordering App - Food Villa

We create a Food Ordering App called "Food Villa" in this session.

### Step 3: Writing Comments in JSX

We discuss how to write comments in JSX, similar to JavaScript, using `{/* */}`.

### Step 4: ES6, JSX, TypeScript in React

We emphasize that while ES6, JSX, and TypeScript are not mandatory for working in React, they are highly recommended for modern React projects.

### Step 5: Create Low-Level Design - Create App Layout

We define the structure of our Food Ordering App's layout, including the header, body, and footer components.

```jsx
// Header
- logo (Title)
- nav items (right side)
- cart

// Body
- search bar
- restaurantList
- restaurantCard
  - image
  - Name
  - Rating
  - Cuisine

// Footer
```

### Step 6: Create HeaderComponent

We create the HeaderComponent, which includes the TitleComponent with a logo image and navigation items.

### Step 7: JSX and React.Fragment

We discuss JSX and the use of React.Fragment (`<></>`) to group children without adding extra DOM nodes.

### Step 8: Config Driven UI

We introduce the concept of Config Driven UI, which allows for different UI layouts for different users based on backend-driven configuration.

### Step 9: Optional Chaining (?.)

We explain Optional Chaining (`?.`) in JavaScript, which safely accesses nested object properties.

### Step 10: Props (Properties)

We delve into Props, which are attributes passed through the component tag, enabling data flow between parent and child components.

### Step 11: Virtual DOM and React Reconciliation

We highlight the importance of Virtual DOM in React and how it facilitates React Reconciliation, which efficiently updates the DOM.

### Step 12: React Fiber

We briefly mention React Fiber, the reconciliation engine in React 16 that enables features like incremental rendering.

### Code Examples

Now, let's dive into the code examples for different scenarios of rendering restaurant cards.

#### Case 1: Using Hard Coded Data (without Props)

```jsx
const restaurantData = {
  imageId: "bdcd233971b7c81bf77e1fa4471280eb",
  name: "KFC",
  cuisines: ["Burger", "Biryani", "American"],
  approxDeliveryTime: "45"
}

const RestaurantCard = () => {
  return (
    <div className="restaurant-card">
      <img src={"https://res.cloudinary.com/swiggy/image/upload/fl_lossy,f_auto,q_auto,w_508,h_320,c_fill/" + restaurantData?.imageId} alt="restaurant image" />
      <h2>{restaurantData?.name}</h2>
      <h3>{restaurantData?.cuisines.join(", ")}</h3>
      <h4>{restaurantData?.approxDeliveryTime} minutes</h4>
    </div>
  )
}
```

#### Case 2: Passing Sample Data (Object) through Props

```jsx
const restaurantData = {
  imageId: "bdcd233971b7c81bf77e1fa4471280eb",
  name: "KFC",
  cuisines: ["Burger", "Biryani", "American"],
  approxDeliveryTime: "45"
}

const RestaurantCard = (props) => {
  return (
    <div className="restaurant-card">
      <img src={"https://res.cloudinary.com/swiggy/image/upload/fl_lossy,f_auto,q_auto,w_508,h_320,c_fill/" + props.restaurant?.imageId} alt="restaurant image" />
      <h2>{props.restaurant?.name}</h2>
      <h3>{props.restaurant?.cuisines.join(", ")}</h3>
      <h4>{props.restaurant?.approxDeliveryTime} minutes</h4>
    </div>
  )
}
```

#### Case 3: Passing Sample Data (Array) through Props

```jsx
const restaurantDataArray = [
  {
    imageId: "bdcd233971b7c81bf77e1fa4471280eb",
    name: "KFC",
    cuisines: ["Burger", "Biryani", "American"],
    approxDeliveryTime: "45"
  },
  {
    imageId: "bdcd233971b7c81bf77e1fa4471280eb",
    name: "Burger king",
    cuisines: ["Burger", "American"],
    approxDeliveryTime: "15"
  }
]

const RestaurantCard = (props) => {
  return (
    <div className="restaurant-card">
      <img src={"https://res.cloudinary.com/swiggy/image/upload/fl_lossy,f_auto,q_auto,w_508,h_320,c_fill/" + props.restaurant?.imageId} alt="restaurant image" />
      <h2>{props.restaurant?.name}</h2>
      <h3>{props.restaurant?.cuisines.join(", ")}</h3>
      <h4>{props.restaurant?.approxDeliveryTime} minutes</h4>
    </div>
  )
}
```

#### Case 4: Passing Sample Data (Array) through Props [Object Destructuring]

```jsx
const restaurantDataArray = [
  {
    imageId: "bdcd233971b7c81bf77e1fa4471280eb",
    name: "KFC",
    cuisines: ["Burger", "Biryani", "American"],
    approxDeliveryTime: "45"
  },
  {
    imageId: "bdcd233971b7c81bf77e1fa4471280eb",
    name: "Burger king",
    cuisines: ["Burger", "American"],
    approxDeliveryTime: "15"
  }
]

const RestaurantCard = ({ restaurant }) => {
  const { imageId, name, cuisines, approxDeliveryTime } = restaurant;
  return (
    <div className="restaurant-card">
      <img src={"https://res.cloudinary.com/swiggy/image/upload/fl_lossy,f_auto,q_auto,w_508,h_320,c_fill/" + imageId} alt="restaurant image" />
      <h2>{name}</h2>
      <h3>{cuisines.join(", ")}</h3>
      <h4>{approxDeliveryTime} minutes</h4>
    </div>
  )
}
```

#### Case 5: Passing Sample Data (Array) through Props [Object Destructuring on the Fly & Passing Individual Props]

```jsx
const restaurantDataArray = [
  {
    imageId: "bdcd233971b7c81bf77e1fa4471280eb",
    name: "KFC",
    cuisines: ["Burger", "Biryani", "American"],
    approxDeliveryTime: "45"
  },


  {
    imageId: "bdcd233971b7c81bf77e1fa4471280eb",
    name: "Burger king",
    cuisines: ["Burger", "American"],
    approxDeliveryTime: "15"
  }
]

const RestaurantCard = ({ restaurant }) => {
  const { imageId, name, cuisines, approxDeliveryTime } = restaurant;
  return (
    <div className="restaurant-card">
      <img src={"https://res.cloudinary.com/swiggy/image/upload/fl_lossy,f_auto,q_auto,w_508,h_320,c_fill/" + imageId} alt="restaurant image" />
      <h2>{name}</h2>
      <h3>{cuisines.join(", ")}</h3>
      <h4>{approxDeliveryTime} minutes</h4>
    </div>
  )
}
```

#### Case 6: Passing Sample Data (Array) through Props [Using Map() + Spread Operator + Destructuring]

```jsx
const restaurantDataArray = [
  {
    imageId: "bdcd233971b7c81bf77e1fa4471280eb",
    name: "KFC",
    cuisines: ["Burger", "Biryani", "American"],
    approxDeliveryTime: "45"
  },
  {
    imageId: "bdcd233971b7c81bf77e1fa4471280eb",
    name: "Burger king",
    cuisines: ["Burger", "American"],
    approxDeliveryTime: "15"
  }
]

const RestaurantCard = ({ restaurant }) => {
  const { imageId, name, cuisines, approxDeliveryTime } = restaurant;
  return (
    <div className="restaurant-card">
      <img src={"https://res.cloudinary.com/swiggy/image/upload/fl_lossy,f_auto,q_auto,w_508,h_320,c_fill/" + imageId} alt="restaurant image" />
      <h2>{name}</h2>
      <h3>{cuisines.join(", ")}</h3>
      <h4>{approxDeliveryTime} minutes</h4>
    </div>
  )
}
```

### Conclusion

In this README, we've covered the essential steps and code examples for building a Food Ordering App in React. Feel free to refer to these code snippets as you work on your project. Happy coding! 🍔🍕🍟🍣🌮🍱

---

This README file provides a comprehensive guide to building a Food Ordering App in React. Feel free to use it as a reference for your lecture or share it with your audience. If you have any questions or need further clarification, please don't hesitate to ask. Good luck with your lecture and happy coding! 🚀📚👨‍💻


Feel free to use this README file as a reference for your lecture . Happy coding! 🚀📚👨‍💻