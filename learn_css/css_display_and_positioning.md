### CSS Display and Positioning
- position: static(default)/relative/absolute/fixed
    - `relative` : position an element relative to its default static position on the web page
        ``` css
        .box-bottom {
          background-color: DeepSkyBlue;
          position: relative;
          top: 20px;
          left: 50px;
        }
        ```
    - `absolute`: all other elements on the page will ignore the element and act like it is not present on the page. The element will be positioned relative to its closest positioned parent element.
    - `fixed` :  fix an element to a specific position on the page (regardless of user scrolling) 
---
- `z-index:int`: controls how far “back” or how far “forward” an element should appear on the web page when elements overlap.
    - *The larger value appears on the top layer.*
- display: inline/blcok/inline-block;
    - The default display for some tags, such as `<em>`, `<strong>`, and `<a>`, is called inline. 
    -  Inline elements have a box that wraps tightly around their content.
    - The height and width of these elements cannot be specified in the CSS document.
        ``` css
        /* The CSS display property provides the ability to make any element an inline element */
        h1 {
          display: inline;
        }
        ```
    -  For a complete list of block level elements, visit the [MDN documentation](https://developer.mozilla.org/en-US/docs/Web/HTML/Block-level_elements).
    - Inline-block display combines features of both inline and block elements. Inline-block elements can appear next to each other and we can specify their dimensions using the width and height properties.
---
- float: right
- clear：left/right/both/none
    -  the * side of the element will not touch any other element within the same containing element.
