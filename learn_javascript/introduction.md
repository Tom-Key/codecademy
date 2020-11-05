### Introduction to JavaScript
- `console.log(info);`
    -  print values to the console, so we can see the work that we’re doing
-  Ending each statement with a semicolon so you never leave one out in the few instances when they are required
- `//comment`
    ``` js
    /* multi-line
    comment */
    console.log(/*cmment in the middle of a line*/ 5);
    ```
---
- Data Types
    - Number / String / Boolean / `null` / `undefined`
    - Symbol: A newer feature to the language, symbols are unique identifiers, useful in more complex coding. No need to worry about these for now.
    - Objects: Collections of related data.
    - The first 6 of those types are considered primitive data types.
- Arithmetic Operators
    - Remainder %
- String Concatenation
    - `console.log('I love to ' + 'code.')`
- Properties
    - `console.log('Hello'.length);`
- Methods
    - `console.log('hello'.toUpperCase());`
    - `console.log('Hey'.startsWith('H')); // true`
    -  [JavaScript documentation.](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String)

- [Built-in Objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects)
    - `Math.random() // random number between 0 and 1`
    - `Math.floor(2.5)  // round down a number` / ceil向上取整 
    - `Number.isInteger(34.2)`
    
### Variables
- `var myName = 'Arya';`
    - camel casing
    - myName and myname would be different variables
    - It is bad practice to create two variables that have the same name using different cases.
    - [MDN’s keyword documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Lexical_grammar#Keywords)
- `let meal = 'Enchiladas';`
    -  The let keyword signals that the variable can be **reassigned** a different value. 
    - If we don’t assign a value to a variable declared using the let keyword, it automatically has a value of `undefined`
- `const myName = 'Gilberto';`
    -  a const variable cannot be reassigned 
---
- Mathematical Assignment Operators
    - `*=` supported
- The Increment and Decrement Operator
    - `++/--`
- String Interpolation
    - a template literal is wrapped by backticks **`**
    ``` js
    const myPet = 'armadillo';
    console.log(`I own a pet ${myPet}.`);
    // Output: I own a pet armadillo.
    ```
- `console.log(typeof unknown1); // Output: string`
