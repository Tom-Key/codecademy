### Loops
``` js
for (let counter = 0; counter < 4; counter++) {
  console.log(counter);
}
```
- The iteration statement is counter++. This means after each loop, the value of counter will increase by 1.

- Nested Loops
- The while loop
    ``` js
    while (counterTwo < 4) {
      console.log(counterTwo);
      counterTwo++;
    }
    ```
- Do...While Statements
    ```js
    do {
      countString = countString + i;
      i++;
    } while (i < 5);
    ```
- The break Keyword
    ``` js
    if (i > 2 ) {
         break;
      }
    ```    
-----------
- 未声明类型也可以正常使用变量 ==
    ```js
    for (i=0;i<vacationSpots.length;i++){
      console.log(`I would love to visit ${vacationSpots[i]}`);
    }
    ```