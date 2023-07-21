# Frontend Interview Questions & Answers

---

### Table of Contents

| Topic                     | # Qs |
| ------------------------- | ---- |
| [HTML5](#html5)           | 5    |
| [CSS](#css)               | 4    |
| [CSS Code](#css-code)     | 1    |
| [JavaScript](#javascript) | 4    |
| [React](#react)           | 0    |

## HTML5

1. <details><summary>What are semantic elements in html5?</summary>

   Semantic elements in HTML5 are tags that add meaning to the structure of web documents beyond their visual representation. By using these elements, developers can create more descriptive and organized content, which benefits developers, users who rely on **assistive technologies** and **search engines** which can lead to a better search engine rankings.

   Some of the key semantic elements include _header_, _nav_, _main_ and _section_. Some non semantic elements are _div_ and _span_.

  </details>

2. <details><summary>What is flexbox?</summary>

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

  </details>

4. <details><summary>What is the this keyword in JavaScript?</summary>

   In JavaScript, the this keyword is a special context-sensitive variable that refers to the current execution context or the "owner" of the code that is currently being executed. The value of this depends on how and where a function is called or how an object method is invoked.

  </details>

**[⬆ Back to Top](#table-of-contents)**
