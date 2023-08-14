# Frontend Interview Questions & Answers

---

### Table of Contents

| Topic                     | # Qs |
| ------------------------- | ---- |
| [HTML5](#html5)           | 6    |
| [CSS](#css)               | 4    |
| [CSS Code](#css-code)     | 1    |
| [JavaScript](#javascript) | 6    |
| [React](#react)           | 7    |

[React Native](markdown/react-native.md)

## HTML5

1. <details><summary>What are semantic elements in html5?</summary>

   Semantic elements in HTML5 are tags that add meaning to the structure of web documents beyond their visual representation. By using these elements, developers can create more descriptive and organized content, which benefits developers, users who rely on **assistive technologies** and **search engines** which can lead to a better search engine rankings.

   Some of the key semantic elements include _header_, _nav_, _main_ and _section_. Some non semantic elements are _div_ and _span_.
   </details>

2. <details><summary>What is doctype?</summary>

   In HTML5, the <!DOCTYPE> declaration is used to specify the type and version of the HTML being used in the web document. The purpose of the <!DOCTYPE> declaration is to tell the web browser which version of HTML to expect and how to parse and render the content.

   Including the <!DOCTYPE html> declaration in your HTML documents is important because it ensures that modern web browsers interpret and render the content correctly.
   </details>

3. <details><summary>What is block and inline elements?</summary>

   Block-level elements create blocks of content that stack vertically, taking up the full width of their parent container, while inline elements flow within the text and do not create new lines.

   Common block-level elements include _div_, _p_, _header_ and _section_.

   Common inline elements include _span_, _img_, _br_ and _input_.
   </details>

4. <details><summary>What is the datalist tag?</summary>

   The `datalist` tag is an HTML5 element that is used in conjunction with the `input` element to provide a predefined list of options for user input. It allows web developers to create a dropdown list of options that users can select from while entering data in an input field. The `datalist` element is particularly useful for autocompletion or suggesting valid options to users, thereby improving the user experience and data entry efficiency.
   </details>

5. <details><summary>What is the class and id attribute?</summary>

   In HTML, the class and id attributes are used to add specific identifying information to elements, allowing developers to apply CSS styles or JavaScript functionality to those elements.

   You use IDs when you need unique identification for an element, and classes when you want to group elements with shared characteristics.
   </details>

6. <details><summary>What are empty elements in HTML?</summary>

   In HTML, an "empty element" refers to an element that doesn't have any content between an opening tag and a closing tag because it doesn't require any inner text or nested elements. Empty elements are also known as "self-closing elements" or "void elements."

   These elements are used to embed or represent various types of content within a web page and don't require a closing tag. Instead, they are typically written using a single tag, sometimes followed by a forward slash (/) before the closing angle bracket (>).

   Some examples are `<img>`, `<br>`, `<input>`, `<hr>`, `<meta>` and `<link>`.
   </details>

**[⬆ Back to Top](#table-of-contents)**

## CSS

1. <details><summary>What is the difference between display:none and visibility:hidden?</summary>

   The display:none and visibility:hidden are both CSS properties used to hide elements on a web page.

   The main difference between display: none; and visibility: hidden; is that display: none; removes the element from the document flow entirely, while visibility: hidden; hides the element from view but retains its space in the layout.
   </details>

2. <details><summary>What is flexbox?</summary>

   Flexbox is a CSS layout model introduced in CSS3 that allows developers to create flexible and responsive layouts for web applications and user interfaces. Flexbox is designed to distribute space and align items within a container, making it easier to create dynamic and adaptive designs without the need for complex CSS calculations or JavaScript.
   </details>

3. <details><summary>What is a pseudo class and pseudo elements?</summary>

   In CSS, pseudo-classes and pseudo-elements are special selectors that allow you to target specific elements under certain conditions or states. They extend the standard CSS selectors and provide additional styling options for more dynamic and interactive designs.

   Pseudo-classes are used to select and style elements based on their state or relationship with the user or the document. They begin with a colon (:) followed by the pseudo-class name. Some common examples are `:hover`, `:focus` and `:first-child`.

   Pseudo-elements are used to style specific parts of an element's content. They begin with two colons (::) followed by the pseudo-element name.
   Some common examples of pseudo-elements include `::before`, `::after` and `first-line`.
   </details>

4. <details><summary>What is the box-model property?</summary>

   The box model is a fundamental concept in CSS that describes how elements are displayed and how their content, padding, borders, and margins are calculated and rendered within the layout. The total width of an element is calculated by adding the content width, left and right padding, left and right border, and left and right margin. The total height is calculated similarly, but considering the top and bottom properties instead.

   Padding and margins are often used to create proper spacing between elements, while borders are used to add visual separation or decoration to elements.
   </details>

**[⬆ Back to Top](#table-of-contents)**

## CSS code

1. <details><summary>Write code to center a div horizontally and vertically</summary>

   Using Flexbox:

   ```CSS
   .container {
     display: flex;
     justify-content: center; /* Horizontal centering */
     align-items: center; /* Vertical centering */
   }
   ```

   </details>

**[⬆ Back to Top](#table-of-contents)**

## JavaScript

1. <details><summary>What is closure?</summary>

   A closure is a programming concept that occurs when a function is defined inside another function and retains access to the variables, parameters, and scope of its outer (enclosing) function, even after the outer function has finished executing or its execution context has been destroyed.

   Closures are powerful tools in programming as they enable private variables and data encapsulation by making those variables become inaccessible from outside the function, and facilitate the creation of higher-order functions (functions that take other functions as arguments or return functions as results). They are commonly used in scenarios like callbacks and event handlers.
   </details>

2. <details><summary>What is the difference between null and undefined?</summary>

   In JavaScript, null and undefined are two distinct values used to represent the absence of meaningful data. Undefined indicates the absence of a value, often due to variables or properties not being assigned or not existing, while null represents the intentional absence of a value, typically used when explicitly indicating that a value is not available or relevan
   </details>

3. <details><summary>What is hoisting</summary>

   Hoisting is a JavaScript behavior in which variable and function declarations are moved to the top of their containing scope during the compilation phase, before the code is executed. This means that you can access variables and functions before they are declared in the code.

   However, it's essential to note that only the declarations are hoisted, not the initializations (assignments). The variables will be initialized with the value undefined until the actual assignment is encountered during runtime.

   Function declarations are also hoisted to the top of their scope, and this behavior allows you to call functions before their actual declarations in the code. However, function expressions (functions assigned to variables including arrow functions) are not hoisted in the same way as function declarations.
   </details>

4. <details><summary>What is the this keyword in JavaScript?</summary>

   In JavaScript, the `this` keyword is a special context-sensitive variable that refers to the current execution context or the "owner" of the code that is currently being executed. The value of `this` depends on how and where a function is called or how an object method is invoked. Some common uses are:

   - Method Invocation: When a function is called as a method of an object, `this` is used to access the properties and methods of that object. It allows the method to reference and operate on the data within the object.
   - Constructor Functions: `This` is used inside constructor functions to refer to the newly created object instance. It allows the constructor to set properties and initialize the object's state.
   - Event Handlers: In event handlers, such as those used with HTML elements, `this` often refers to the element that triggered the event. It allows you to manipulate the element or access its attributes and data.

   Here is how `this` behaves in other scenarios:

   - Global Context: In the global scope (outside of any function), `this` refers to the global object. In a web browser, the global object is typically the window object.
   - Function Context: Inside a regular function (not an arrow function), the value of `this` is determined by how the function is called. When a function is called as a standalone function (not attached to an object), `this` will also refer to the global object.
   - Arrow Functions: Arrow functions have a different behavior for `this`. They capture the value of `this` from the surrounding (lexical) context at the time of their creation, rather than when they are executed. As a result, the value of `this` inside an arrow function is not affected by how the function is called.
   </details>

5. <details><summary>What are higher-order functions (HOFs)?</summary>

   A HOF is a function that takes another function as an argument. In JavaScript, functions are considered "first-class citizens," meaning they can be treated like any other data type, including being passed as arguments to other functions. The function passed as an argument is called a callback.
   </details>

6. <details><summary>What are callbacks?</summary>

   Callbacks are functions passed as arguments to other functions in JavaScript. They allow you to execute a piece of code at a later time or after a certain event has occurred. Callbacks are an essential concept in asynchronous programming, where tasks might take some time to complete, and you want to specify what to do once the task is finished.
   </details>

7. <details><summary>What is Mutability in JavaScript?</summary>

   In JavaScript, mutability refers to the property of an object whose state or values can be changed after it has been created. In other words, mutable objects can be modified, while immutable objects cannot be changed once they are created.
   </details>

8. <details><summary>Is string a primitive or a reference data type?</summary>

   In JavaScript, a string is immutable making it a primitive data type. Even though string have methods, any operations you perform on the string, such as using methods like .toUpperCase() or .substring(), do not modify the original string. Instead, they create and return new strings based on the original one, leaving the original string unchanged.
   </details>

9. <details><summary>How many primitive data types exists and what are they?</summary>

   There are 7 primitive data types in JS: String, Number, Boolean, Undefined, Null, Symbol and Bigint.
   </details>

10. <details><summary>What is the difference between primitive and reference data types?</summary>

    The main difference between primitive and reference data types in JavaScript lies in how they are stored and how they behave when assigned to variables or passed as arguments to functions.

      <details><summary>Storage and Assignment</summary>

    Primitive Data Types: When a variable is assigned a primitive data type (e.g., number, string, boolean, null, undefined, symbol, or bigint), the variable stores the actual value of that data type. Assigning a primitive value to a new variable creates a copy of that value.

    ```js
    let a = 5;
    let b = a; // 'b' gets a copy of the value stored in 'a'.
    a = 10; // Changing the value of 'a' doesn't affect 'b'.
    console.log(a); // Output: 10
    console.log(b); // Output: 5
    ```

    Reference Data Types: On the other hand, when a variable is assigned a reference data type (e.g., objects, arrays, functions), the variable stores a reference or memory address pointing to the location in memory where the actual data is stored. Assigning a reference value to a new variable creates a new reference to the same data, not a new copy of the data itself.

    ```js
    let arr1 = [1, 2, 3];
    let arr2 = arr1; // 'arr2' gets a reference to the same array as 'arr1'.
    arr1.push(4); // Modifying 'arr1' also affects 'arr2'.
    console.log(arr1); // Output: [1, 2, 3, 4]
    console.log(arr2); // Output: [1, 2, 3, 4] (Both 'arr1' and 'arr2' reference the same array.)
    ```

      </details>

      <details><summary>Mutability</summary>

    Primitive Data Types: Primitive values are immutable, meaning their values cannot be changed after they are created. Operations on primitive values create new values rather than modifying the original values.

    ```js
    let str1 = "Hello";
    let str2 = str1.toUpperCase(); // 'toUpperCase()' creates a new string; 'str1' remains unchanged.
    console.log(str1); // Output: "Hello"
    console.log(str2); // Output: "HELLO"
    ```

    Reference Data Types: Reference values are mutable, meaning their properties or elements can be modified after they are created. Changes to a referenced object are reflected in all references to that object.

    ```js
    let obj1 = { name: "John" };
    let obj2 = obj1; // 'obj2' gets a reference to the same object as 'obj1'.
    obj1.age = 30; // Modifying 'obj1' also affects 'obj2'.
    console.log(obj1); // Output: { name: "John", age: 30 }
    console.log(obj2); // Output: { name: "John", age: 30 } (Both 'obj1' and 'obj2' reference the same object.)
    ```

      </details>

    In summary, primitive data types store the actual values, are copied by value, and are immutable. In contrast, reference data types store memory references, are copied by reference, and are mutable. Understanding these differences is crucial for correctly handling and manipulating data in JavaScript.
    </details>

11. <details><summary>What is event delegation?</summary>

    Event delegation is a design pattern in web development where you attach a single event listener to a higher-level or parent element, rather than attaching individual event listeners to multiple child elements. This pattern is used to efficiently handle events on a large number of elements, especially when those elements share a common ancestor or container.

    **Benefits of Event Delegation:**

    **Efficiency**: Event delegation reduces the number of event listeners in the DOM, leading to better performance and less memory consumption, especially when dealing with a large number of elements.

    **Dynamic Content**: It works seamlessly with dynamically added or removed elements, as you don't need to attach new event listeners when elements are added or replaced.

    **Simplicity**: You only need to manage one event listener on a parent element, simplifying your code and making it easier to maintain.

    **Memory Management**: Event delegation can help avoid memory leaks, as it doesn't require you to manually remove event listeners when elements are removed from the DOM.
    </details>

**[⬆ Back to Top](#table-of-contents)**

## REACT

1. <details><summary>What is the Virtual DOM?</summary>

   The Virtual DOM is a concept in React that serves as an intermediary representation of the actual DOM (Document Object Model) used by web browsers.

   Here are some benefits:

   **Efficient Updates:** When state or props of a component change, React performs a process known as "reconciliation." It calculates the difference between the previous Virtual DOM and the new Virtual DOM to identify the minimal set of changes needed to update the actual DOM. This process is called "diffing."

   **Batch Updates:** React optimizes DOM updates by batching multiple changes together. Instead of updating the actual DOM after each individual change, React performs a batch update, making it more efficient.
   </details>

2. <details><summary>What are React hooks, and how do they differ from class-based components?</summary>

   React hooks are functions that allow functional components in React to have state and perform lifecycle-related tasks, which were previously only possible with class-based components. Hooks were introduced in React version 16.8 to provide a more concise and intuitive way of managing state and side effects in functional components. In general, hooks provide a more concise, readable, and powerful way of handling state and side effects in React components.

   Here are some benefits:

   **No Class Syntax:** One of the primary advantages of hooks is that they eliminate the need to use class syntax in functional components. Class-based components involve boilerplate code for constructor, lifecycle methods, and binding event handlers. Hooks, on the other hand, use regular JavaScript functions, making the code cleaner and more straightforward.

   **Lifecycle Management with useEffect:** The useEffect hook handles side effects in functional components. It replaces various lifecycle methods (such as componentDidMount, componentDidUpdate, and componentWillUnmount) that were used in class-based components. This makes it easier to organize and manage side effects.

   **Custom Hooks for Code Reusability:** With hooks, you can create custom hooks to encapsulate and share stateful logic across components. This promotes code reusability and abstraction without the need for higher-order components (HOCs) or render props.
   </details>

3. <details><summary>What are higher-order components (HOCs) and how do you use them?</summary>

   HOCs are a design pattern in React where a function that takes a component as an argument and returns a new component with additional props or functionality. It allows you to abstract logic that can be shared across multiple components, promoting code reusability.

   While HOCs can be powerful, they can also lead to a complex component hierarchy if used excessively. As an alternative, you can consider using custom hooks, which provide a more concise and elegant way to share logic between components without the nesting involved in HOCs.
   </details>

4. <details><summary>What are the major features of React?</summary>

   React is a popular JavaScript library for building user interfaces, and it comes with a range of powerful features that make it efficient and flexible. Some of the major features of React include:

   1. Component-Based Architecture: React's component-based architecture promotes reusability, modularity, and maintainability, allowing developers to build UIs as a collection of reusable and independent components.

   2. Virtual DOM: React's Virtual DOM optimizes rendering by updating only the necessary parts of the actual DOM, resulting in improved performance and a smoother user experience.

   3. JSX (JavaScript XML): JSX simplifies the creation of React elements by allowing developers to write HTML-like code directly in JavaScript, making the code more readable and intuitive.

   4. Unidirectional Data Flow: React's unidirectional data flow ensures predictable state management, making it easier to understand how data changes and flows through the application.

   5. React Hooks: Hooks provide a functional approach to state management and lifecycle methods in functional components, resulting in more concise and readable code.

   These are some of the major features that make React a powerful and widely used library for building modern web applications with a focus on performance, reusability, and maintainability.
   </details>

5. <details><summary>How do you handle routing in a React application?</summary>

   There are several ways to handle routing in a React application. One popular approach is to use the third-party library "React Router." It provides a declarative way to define routes and handle navigation in a single-page application (SPA) without reloading the entire page. By defining routes using Router, Route, and Switch components, and using Link for navigation, React Router efficiently manages navigation between different views.
   </details>

6. <details><summary>How can you optimize the performance of React applications?</summary>

   1. **Minimize Rendering and Reconciliation:**
      Use React's memoization techniques like React.memo and shouldComponentUpdate (for class components) to prevent unnecessary re-renders of components.
      Utilize the PureComponent (for class components) or React.PureComponent (for functional components) to automatically handle shallow prop and state comparisons for updates which prevent unnecessary re-renders of components when there are no changes to the component's props or state.
   2. **Virtualization and Infinite Scrolling:**
      For long lists or data grids, consider using virtualization libraries like react-virtualized or react-window to render only the visible items, reducing the DOM size and improving initial loading times.
   3. **Optimize Images and Assets:**
      Compress and optimize images and other assets to reduce their file size. Use modern image formats like WebP and consider lazy-loading images.
   4. **Avoid Unnecessary State Updates:**
      Be mindful of when and where you update state, as unnecessary updates can trigger additional re-renders. Use useCallback to memoize event handlers and prevent them from changing on every render.
   5. **Performance Profiling:**
   Use browser developer tools to profile your application's performance. Identify bottlenecks and areas for improvement.
   </details>

7. <details><summary>Explain React's context API and its use cases?</summary>

   React's Context API is a feature that allows data to be passed down the component tree without the need to pass props explicitly at every level. It helps in managing global or shared state in a React application and simplifies the process of sharing data between components that are not directly related in the component tree.

   The Context API consists of two main parts:

   1. **Context Provider:**
      The Context Provider is a React component that wraps the component tree and holds the data that needs to be shared across components. It provides a context object to its descendants.

   2. **Context Consumer:**
   The Context Consumer is a React component that accesses the data provided by the Context Provider. It can be used within components that need the shared data, and it allows them to subscribe to changes in that data.
   </details>

**[⬆ Back to Top](#table-of-contents)**
