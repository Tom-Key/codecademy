### Conditional Statements
- If...Else Statements
``` js
if (false) {
  console.log('The code in this block will not run.');
} else if(true){
  console.log('But the code in this block will!');
}
```
- Is equal to: `===` / Is not equal to: `!==`
- Logical Operators `&& / || /!`
- falsy values:`0 "" null undefined NaN`  

- Truthy and Falsy Assignment
    - `let defaultName = username || 'Stranger';`
    
- Ternary Operator
    - `isNightTime ? console.log('Turn on the lights!') : console.log('Turn off the lights!');`
----
- switch
    ``` js
    let groceryItem = 'papaya';

    switch (groceryItem) {
      case 'tomato':
        console.log('Tomatoes are $0.49');
        break;
      case 'lime':
        console.log('Limes are $1.49');
        break;
      case 'papaya':
        console.log('Papayas are $1.29');
        break;
      default:
        console.log('Invalid item');
        break;
    }
    ```