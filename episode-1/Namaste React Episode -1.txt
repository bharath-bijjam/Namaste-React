1 . What is Emmet?

-->Emmet is a web development toolkit that greatly enhances HTML and CSS coding efficiency. It allows developers to write shorthand code snippets, called abbreviations, and expand them into full-fledged HTML or CSS. This speeds up the coding process and improves overall productivity by reducing the amount of manual typing required. Emmet is widely used in various web development environments, including text editors and integrated development environments (IDEs).

 Here are a few more examples of Emmet abbreviations:

1. HTML Structure:
   - Abbreviation: html:5
   - Expansion:
     html
     <!DOCTYPE html>
     <html lang="en">
     <head>
         <meta charset="UTF-8">
         <meta name="viewport" content="width=device-width, initial-scale=1.0">
         <title>Document</title>
     </head>
     <body></body>
     </html>
     

2. Nested Elements:
   - Abbreviation: `div>ul>li*3`
   - Expansion:
     ```html
     <div>
         <ul>
             <li></li>
             <li></li>
             <li></li>
         </ul>
     </div>
     ```

3. Class and ID:
   - Abbreviation: `div.container#main-content`
   - Expansion:
     ```html
     <div class="container" id="main-content"></div>
     ```

4.CSS Properties:
   - Abbreviation: `p{This is a paragraph}`
   - Expansion:
     ```html
     <p>This is a paragraph</p>
     ```

5. Sibling Elements:
   - Abbreviation: `ul>li.item$*3`
   - Expansion:
	html
     <ul>
         <li class="item1"></li>
         <li class="item2"></li>
         <li class="item3"></li>
     </ul>


Emmet syntax can vary slightly between different editors, but these examples should give you a good starting point for understanding its power in quickly generating HTML and CSS code.



2. Difference between a library and framework ?

Libraries provide modular, reusable code components that developers incorporate at their discretion, offering a more granular level of control. Frameworks, on the other hand, present a comprehensive software architecture, directing the overall application structure and flow. Frameworks often follow the Inversion of Control principle, where the framework manages the flow, and developers implement custom functionalities within this structured environment.

Ex:-jQuery is a library that provides specific functions for tasks, and developers call those functions when needed. React is a framework that dictates the overall structure of an application, and developers build within that structure, allowing React to manage the flow of the application.


3. Why is React known as React?

React is known as React primarily because of its core concept: the ability to react to changes in data and efficiently update the user interface. The name "React" reflects the library's key feature, which is the ability to build dynamic and interactive user interfaces that respond to changes in application state.

React was developed by Facebook and was initially released in 2013. It is often used to build single-page applications where user interfaces need to be updated dynamically based on changing data. The name "React" emphasizes the reactive programming paradigm that the library employs.

In React, the UI is divided into components, and when the underlying data changes, React efficiently updates only the affected components rather than re-rendering the entire page. This reactive approach to building user interfaces has contributed to React's popularity and widespread use in modern web development.



4 .What is CDN ? Why do we use it ? 

A Content Delivery Network, or CDN, is a network of geographically distributed servers designed to enhance the performance and reliability of web content delivery. We use CDNs to improve the user experience by reducing latency, ensuring faster loading times, and optimizing bandwidth usage. CDNs also provide scalability, redundancy, and security features, making them a crucial component for websites with a global audience. By strategically caching and delivering content from servers closer to end-users, CDNs contribute to a more efficient and resilient web infrastructure.

5. What is crossorigin in script tag?

The `crossorigin` attribute in the `<script>` tag is used to manage how the browser handles requests for cross-origin scripts. When set to 'anonymous,' which is the default, the browser fetches the script without sending any credentials. This is suitable for most cases, especially when loading scripts from CDNs. Alternatively, when set to 'use-credentials,' the browser includes credentials with the request, and this is used when the external server requires authentication. It's a security feature ensuring that cross-origin requests for scripts adhere to the same-origin policy. In most scenarios, the default 'anonymous' setting suffices for secure script loading.


6. What is difference between react and react-dom ?

 React is the core library for building components and managing their behavior, ReactDOM is the package responsible for rendering those components into the actual HTML document. Both work in tandem to enable the development of interactive and dynamic user interfaces with React.

7. What is difference between react.development.js and react.production.js files via CDN?

"In React, the `react.development.js` and `react.production.js` files serve different purposes based on the environment in which our application is running—whether it's in development or production.

- react.development.js:
  - Environment: Intended for use in development.
  - Features:
    - Provides additional warnings, error messages, and debugging information.
    - Includes extra checks and features that aid developers in catching and resolving issues during development.
  - Usage: During development, we include this version to take advantage of its helpful development-specific features.

- `react.production.js`:
  - Environment: Optimized for use in production.
  - Features:
    - Stripped of development-specific warnings, checks, and debugging information.
    - Smaller file size to enhance performance and reduce download times.
  - Usage: In the production environment, we switch to this version to prioritize a more streamlined and efficient runtime.

It's important to use the appropriate version based on the environment. During development, the `react.development.js` file aids in catching and diagnosing issues early. In production, we switch to `react.production.js` to ensure optimal performance and a smaller production-ready bundle without unnecessary development features."


8. What is async and defer? 

In HTML, the async and defer attributes in the <script> tag impact how JavaScript files are downloaded and executed. The async attribute indicates that the script can be executed asynchronously, allowing it to download in the background and potentially interrupt HTML parsing for immediate execution. On the other hand, the defer attribute signals that the script should be executed after the HTML document is fully parsed, maintaining the order of execution and dependency on HTML structure. These attributes are useful for optimizing script loading and execution, depending on the script's requirements in relation to HTML structure and other scripts.
