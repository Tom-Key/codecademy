### Functions
- Function Declarations
![](https://content.codecademy.com/courses/learn-javascript-functions/Diagram/declaration.svg)
- hoisting allowed greetWorld() to be called before the greetWorld() function was defined

- Function Calling
![](https://content.codecademy.com/courses/learn-javascript-functions/Diagram/function%20execution.svg)


- Parameters and Arguments
![](https://content.codecademy.com/courses/learn-javascript-functions/Diagram/function_parameters.svg)

- Default Parameters `name = 'stranger'`

- Return `return area;`
    - if the value is omitted, undefined is returned instead
    
- helper functions: use the return value of a function inside another function


- Function Expressions
![](https://content.codecademy.com/courses/learn-javascript-functions/Diagram/expression.svg)

- Arrow Functions
    - ES6 introduced arrow function syntax, a shorter way to write functions by using the special “fat arrow” () => notation.
        ``` js
        const rectangleArea = (width, height) => {
          let area = width * height;
          return area;
        };
        ```

- Concise Body Arrow Functions
    - If a function takes zero or multiple parameters, parentheses are required.
    -  the return keyword can be removed
    ![](https://content.codecademy.com/courses/learn-javascript-functions/Diagram/return.svg)
    