### Scope
- It may seem like a great idea to always make your variables accessible, but having too many global variables can cause problems in a program.

- Scope pollution is when we have too many global variables that exist in the global namespace, or when we reuse variables across different scopes. Scope pollution makes it difficult to keep track of our different variables and sets us up for potential accidents. 

- **global scope** variables are declared outside of blocks. These variables are called `global variables`. Because global variables are not bound inside a block, they can be accessed by any code in the program, including code in blocks.

- **Block Scope** Variables that are declared with block scope are known as local variables because they are only available to the code that is part of the same block.