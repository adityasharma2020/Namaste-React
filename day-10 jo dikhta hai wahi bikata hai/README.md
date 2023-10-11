# Chapter 10 - Jo dikhta hai wahi bikata hai

👀 In Chapter 10, "Jo dikhta hai wahi bikata hai" we delved into the UI layer of our application, recognizing the critical importance of the user interface. The look and feel of the app attracts the user. Various ways of writing CSS (styling) were discussed in this chapter, and we recreated the entire app using Tailwind CSS.

## Key Learnings

### The Need for Frameworks

1. **Optimized CSS**: Frameworks offer pre-optimized CSS, enhancing application performance.

2. **Consistent UI**: Frameworks ensure a uniform and polished user interface, which is crucial for a seamless user experience.

3. **Time Savings**: Leveraging frameworks accelerates development by providing ready-to-use styling components.

4. **Multiple Frameworks**: It's possible to use more than one framework, but it can lead to inconsistency in styling.

### Variety of Styling Methods

1. **Native CSS**: Traditional CSS, with all component styles in a single file (index.css).

2. **SCSS**: Syntactical CSS, which is converted to standard CSS.

3. **Inline CSS**: Utilizing the style attribute to pass styling as an object (e.g., `{{backgroundColor: "red"}}`).

4. **Component Libraries**: Harnessing component libraries like MaterialUI, Bootstrap, Base Web UI, Ant Design, Chakra UI.

5. **CSS Frameworks**: Adopting CSS frameworks such as Tailwind CSS for efficient styling.

6. **Styled Components**: Popular in React projects for component-specific styling.

### Choosing the Right Styling Approach

In system design interviews and real-world projects, it's vital to select the appropriate styling method based on the specific requirements. Pros and cons of different methods must be considered:

- **Native CSS vs. SCSS**: Pros and cons should be weighed, addressing aspects like maintainability, ease of development, and customization.

- **Pros & Cons of Component Libraries**: While they ensure consistency and save time, they may result in larger bundle sizes and limited customization.

### Embracing Tailwind CSS

Tailwind CSS is a versatile styling framework with several benefits:

1. **On-the-Go Styling**: CSS can be written directly in the same file, promoting flexibility.

2. **Reusability**: Tailwind CSS supports reusing CSS classes, promoting efficient development.

3. **Reduced Bundle Size**: Only includes the CSS classes actually used in the project, leading to a smaller bundle.

4. **Flexible UI**: Tailwind CSS allows for extensive customization.

### Setting Up Tailwind CSS

To integrate Tailwind CSS into your project, follow these steps:

1. **Installation**: Use `npm install -D tailwindcss postcss` to install Tailwind CSS and its peer dependencies, then run `npx tailwindcss init` to generate `tailwind.config.js`.

2. **Configure Tailwind**: Customize your project by specifying paths to template files in `tailwind.config.js`.

3. **Configure PostCSS**: Create a `.postcssrc` file and enable the Tailwind CSS plugin.

4. **Tailwind Directives**: In your `index.css` file, use the `@tailwind` directives for Base, Components, and Utilities.

Tailwind CSS offers a range of benefits, including time savings, easy debugging, reduced shipped code, smaller bundle sizes, and more customization. However, it may come with an initial learning curve and the challenge of managing an extensive number of classes.

✨ Tailwind CSS empowers you to build stunning and highly customizable user interfaces without leaving your JavaScript file. Let your application shine and ensure a delightful user experience with Tailwind CSS!

## Additional Notes

**Why frameworks?**

Frameworks are essential for various reasons:

- **Optimized CSS**: They provide pre-optimized CSS, leading to better application performance.

- **Consistent UI**: Frameworks maintain a consistent and polished user interface, ensuring a seamless user experience.

- **Time Savings**: Using frameworks accelerates development by offering ready-to-use styling components.

**Can we use more than one framework?**

It's possible to use multiple frameworks, but it can result in inconsistent styling across the application. Therefore, it's important to choose one that best suits your needs.

**Different Ways to Write CSS:**

1. **Normal Native CSS**: Traditional CSS with all component styles in a single file (index.css).

2. **SCSS**: Syntactical CSS, which is ultimately converted to standard CSS.

3. **Inline CSS**: Styling using the style attribute, where styling is passed as an object (e.g., `{{backgroundColor: "red"}}`).

4. **Component Libraries**: Utilizing component libraries like MaterialUI, Bootstrap, Base Web UI, Ant Design, Chakra UI.

5. **CSS Frameworks**: Adoption of CSS frameworks like Tailwind.

6. **Styled Components**: Commonly used in React projects for component-specific styling.

**Choosing the Right Styling Approach**

In system design interviews and real-world projects, it's vital to choose the appropriate styling method based on specific requirements. It's essential to understand the pros and cons of each method.

- **Native CSS vs. SCSS**: Consider factors such as maintainability, ease of development, and customization.

- **Pros & Cons of Component Libraries**: While these libraries ensure consistency and save time, they may lead to larger bundle sizes and limited customization.

**Conclusion**

Chapter 10 taught us the significance of the UI layer in our application. A well-designed user interface is crucial to attract and engage users effectively. We explored various styling methods, with a particular focus on Tailwind CSS, a powerful framework that offers flexibility, reusability, and optimized bundle sizes. By understanding the advantages and disadvantages of different styling methods, we can make informed decisions to create visually appealing and efficient user interfaces.

For more details, refer to the content of Chapter 10. Happy styling! 🚀