# Lecture 2 - Igniting Our App 🚀

Welcome to Lecture 2 of the "Namaste React" course! In this lecture, we'll dive into creating a production-ready React app from scratch without using create-react-app. We'll explore the concept of bundlers, with a focus on Parcel, and understand how they contribute significantly to optimizing, improving performance, and speeding up our applications.

## Topics Covered

In this lecture, we covered the following topics:

| Topic                | Description                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| Bundlers             | Introduction to bundlers, setting up Parcel, and more.                      |
| Theory               | Theoretical concepts like `npm`, Parcel, and package management.             |
| Superpowers of Parcel| A look at the powerful features of Parcel.                                   |
| Git and File Management| Exploring `.gitignore`, `package.json`, and `package-lock.json`.           |
| `node_modules` Directory| Understanding its purpose and why it should not be pushed to Git.         |
| The `dist` Folder    | Insights into the `dist` folder and its role.                               |
| Browserslist         | Configuring browser support for your frontend app.                           |
| Other Bundlers       | A brief overview of alternative bundlers.                                    |
| Script Types in HTML | Understanding script types and their usage.                                |
| Script Tag Attributes| Explanation of script tag attributes.                                       |
| Hidden Lockfiles     | Details about hidden lockfiles in `node_modules`.                           |
| Coding               | Hands-on coding tasks for setting up your app with Parcel and more.         |

## 📋 Git and File Management

- Understanding the purpose of `.gitignore` and what to include and exclude.
- The difference between `package.json` and `package-lock.json` files.
- The importance of not modifying `package-lock.json`.

## 📦 `node_modules` Directory

- Explanation of the `node_modules` directory and why it should not be pushed to version control (Git).

## 🗂️ The `dist` Folder

- Insights into the `dist` folder, which contains the minimized production code of the application.

## 🌐 Browserslist

- Explanation of Browserslist and how it helps specify browser support for a frontend app.

## 🚀 Other Bundlers

- Brief overview of other bundlers like Webpack, Vite, Rollup, and Gulp.

## 📜 Script Types in HTML

- Understanding script types in HTML, including `type` attributes and their significance.

## 📑 Script Tag Attributes

- Explanation of attributes in the script tag and their meanings, such as `src`, `async`, `defer`, `type`, `integrity`, `crossorigin`, and `charset`.

## 🔒 Hidden Lockfiles

- Information about hidden lockfiles in the `node_modules` directory and how they optimize the processing of dependencies.

## 💻 Coding

In the coding part of this lecture, we performed the following tasks:

- Initialized npm within your project repository.
- Installed React and React-DOM as dependencies.
- Removed CDN links for React.
- Installed Parcel as a development dependency.
- Set up your app using Parcel.
- Added scripts for "start" and "build" using Parcel commands.
- Created a .gitignore file.
- Specified Browserslist for browser support.
- Built a production version of your code using Parcel build.

## 📚 Summary

```markdown
markdownCopy code
# Igniting React App 🔥

## In the Last Class

In our previous class, we created a basic React app using a CDN. Today, we'll take a significant step forward and learn how to create a production-ready React app from scratch without relying on create-react-app.

## The Role of Bundlers

To ignite our app, we need a Bundler, such as Vite, Parcel, or Webpack. In the context of create-react-app, Webpack is the bundler of choice. A bundler is essentially a package or module of JavaScript code that helps organize and optimize our code.

## Package Management with npm

To include packages in our code, we rely on a Package Manager like npm or Yarn. Here are some essential npm commands:

```
npm init         # Initialize our project and create package.json
npm init -y      # Skip configuration and create package.json automatically



But why npm? It's because npm is the default package manager for Node.js projects, and it provides a vast ecosystem of packages and libraries that we can use in our applications.

## Meet Parcel

We'll specifically explore Parcel, a zero-configuration web application bundler that simplifies the development process. To install a package with npm, you can use the following commands:

```
npm install package-name       # Install a package (creates node_modules)
npm install -D package-name    # Install as a development dependency
```


Parcel automatically generates a **`package-lock.json`** file and updates your project's dependencies in the **`node_modules`** directory. We installed Parcel as a development dependency because it's needed during development.

## **Production-Ready React**

Moving away from the React CDN approach, we'll work with React and other packages from within our project using npm. Here's how:

```

npm install react        # Install React globally
npx parcel index.html   # Execute npm with index.html as the entry point to create a local server
```


## **Common Errors & Warnings**

As we transition to using npm and modules, you might encounter a few common issues:

- "React is not defined" error: Use import statements instead of CDN links.
- "Browser does not understand import" warning: Specify the module type with **`type="module"`** in script tags.
- "createRoot is not found" warning: Use **`react-dom/client`** instead of **`react-dom`**.

## **Powerful Features of Parcel**

Parcel brings a variety of superpowers to the table, including:

- Minification
- Image optimization
- Compression
- Code cleaning
- Super-fast building
- Development and production builds
- Caching during development
- Compatibility with older browsers
- HTTPS support in development
- Consistent hashing algorithm
- Zero configuration
- Tree shaking (removing unused code)

## **Folder Management and Caching**

In your project, you should consider adding **`.parcel-cache`** to your **`.gitignore`** file. This folder is used by Parcel for processes like Hot Module Replacement (HMR), minification, and caching. Anything that can be auto-generated during the server build can be safely ignored in Git.

## **Improved Build Times**

Initial development builds may take a bit longer (around 500ms), but Parcel utilizes caching to significantly reduce build times for subsequent builds (as low as 5ms).

## **Dependency Management**

Parcel helps manage transitive dependencies, which are dependencies of dependencies. For instance, our app depends on Parcel, which, in turn, depends on other packages, creating a dependency tree.

## **Cross-Browser Compatibility**

Use the **`browserslist`** configuration in your **`package.json`** to ensure cross-browser compatibility with older browser versions:

```

"browserslist": ["last 2 versions"]

```

## **Summary Steps**

Here's a quick summary of the steps we covered:

1. Initialize your project with **`npm init`**.
2. Install Parcel as a development dependency with **`npm install -D parcel`**.
3. Install React and React-DOM with **`npm install react react-dom`**.
4. Run your development server with **`npx parcel index.html`** or build for production with **`npx parcel build index.html`**.
5. Utilize import statements for React.
6. Use **`type="module"`** in your script tags.
7. Remove **`"main": "app.js"`** from your **`package.json`**.
8. Specify browser support in your **`package.json`** using the **`browserslist`** field.

Lecture 2 empowered you with the knowledge and practical skills required to set up a production-ready React app from scratch using Parcel. We explored important theoretical concepts and performed hands-on coding tasks to ignite your React project.

Let's continue our journey and keep building amazing React applications! 🚀
