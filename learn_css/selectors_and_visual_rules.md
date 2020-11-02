yiyidu## Cascading Style Sheets
### CSS Setup and Selectors

- Inline Styles : `<p style="color: red; font-size: 20px;>I'm learning to code!</p>`
    - The paragraph element has a style attribute within its opening tag.
    -  Make sure to end the styles with a semicolon (`;`).
    - `cloor, font-size, font-family`
    - `text-transform: uppercase` 
- Write CSS code in its own dedicated section with the `<style>` element
``` html
<head>
  <style>
    p {
      color: red;
      font-size: 20px;
    }
  </style>
</head>
```
- Linking the CSS File
    - `<link href="style.css" type="text/css" rel="stylesheet">`
    - **type** : the type of document that you are linking to (in this case, a CSS file).
    - **rel** : describes the **relationship** between the HTML file and the CSS file. Because you are linking to a stylesheet, the value should be set to stylesheet.
- CSS can select HTML elements by their tag, class, and ID
    - CSS classes are meant to be reused over many elements.
    - ID is meant to style only one element
- Class Name
    - `<p class="brand">Sole Shoe Company</p>`
    ``` css
    .brand{

    }
    ```
- Multiple Classes
    - `<h1 class="green bold"> ... </h1>`
- ID Name
    - `<h1 id="large-title"> ... </h1>`
    ``` css
    #large-title {
        font-family: cursive;
    }
    ```
- Specificity : IDs > classes > tags
    - *Selectors in the css file are rendered sequentially, and the elements at the same level are subject to the selector appearing positional  disadvantaged.*
- Chaining Selectors
    ```css
    h1.special {

    }
    ```
- Nested Elements
    ``` html
    <ul class='main-list'>
      <li> ... </li>
      <li> ... </li>
      <li> ... </li>
    </ul>
    ```
    ``` css
    .main-list li {

    }
    ```
- Chaining and Specificity :  Adding more than one tag, class, or ID to a CSS selector increases the specificity of the CSS selector.
    ``` css
    /* The !important rule will override even a more specific selector. */
    a {
     color: red !important;
    }
    ```
- Multiple Selectors
    ``` css
    h1, 
    .menu {
      font-family: Georgia;
    }
    ```
    
### CSS Visual Rules
- CSS declarations consist of a property and a value
    - Property : the property you’d like to style of that element (i.e., size, color, etc.).
    - Value : the value of the property (i.e., 18px for size, blue for color, etc.).
- [font-family](https://en.wikipedia.org/wiki/Typeface)
    - Limit the number of typefaces used on a web page to 2 or 3.
- font-size
- font-weight: bold
- text-align: left/center/right
- color/background-color
- opacity
    - Its values range from 0 (transparent) to 1 (opaque)
- background-image: url("https://www.example.com/image.jpg");
- !important : It will override any style no matter how specific it is