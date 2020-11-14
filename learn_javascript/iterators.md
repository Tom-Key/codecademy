### Higher-Order Functions
- Functions as Data
    - JavaScript functions behave like any other data type in the language; we can assign functions to variables, and we can reassign them to new variables.
    - In JavaScript, functions are first class objects. This means that, like other objects you’ve encountered, JavaScript functions can have properties and methods.
    
- Functions as Parameters


### Iterators
- [MDN’s Array iteration methods page](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array#Iteration_methods)
- `.forEach()` Method
![](https://content.codecademy.com/courses/learn-javascript-iterators/iterator%20anatomy.svg)
    - The return value for .forEach() will always be undefined.
    - `groceries.forEach(groceryItem => console.log(groceryItem));`

- The `.map()` Method
    - it takes an argument of a callback function and returns a new array
    ```js
    const numbers = [1, 2, 3, 4, 5]; 
 
    const bigNumbers = numbers.map(number => {
      return number * 10;
    });
    ```
- The `.filter()` Method 
    - .filter() returns an array of elements after filtering out certain elements from the original array
    ```js
    const words = ['chair', 'music', 'pillow', 'brick', 'pen', 'door']; 

    const shortWords = words.filter(word => {
      return word.length < 6;
    });
    ```

- The `.findIndex()` Method
    - Calling .findIndex() on an array will return the index of the first element that evaluates to true in the callback function.
    ``` js
    const jumbledNums = [123, 25, 78, 5, 9]; 

    const lessThanTen = jumbledNums.findIndex(num => {
      return num < 10;
    });
    ```
    
- The `.reduce()` Method
    ``` js
    const numbers = [1, 2, 4, 10];
    const summedNums = numbers.reduce((accumulator, currentValue) => {
      return accumulator + currentValue
    })
    console.log(summedNums) // Output: 17
    ```
    - Add a second argument of 10 to .reduce().
        - The value of accumulator:  10
- The `some()` method tests whether at least one element in the array passes the test implemented by the provided function. It returns a Boolean value.