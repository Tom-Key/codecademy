### The box Model
- How elements are positioned and displayed on a website.
- All elements on a web page are interpreted by the browser as “living” inside of a box.
![A visual representation of the box model](https://content.codecademy.com/courses/updated_images/diagram-boxmodel_Updated_1-01.svg)
---
- height and width
    ``` css
    p {
      height: 100%;
      width: 240px;
    }
    ```
- border: `border: 3px solid coral;`
    - style:  [10 different styles](https://developer.mozilla.org/en-US/docs/Web/CSS/border-style#Values)
    - The default border is `medium none color`
- `border-radius: 100% ` perfect circle
---
- padding
    - padding-top/padding-right/padding-bottom/padding-left
    - padding/margin: 6px 11px 4px 9px *same order*
    - padding/margin: 5px 10px;  top = bottom & left = right
- margin
    - margin-top/margin-right/margin-bottom/margin-left
- auto
    ``` css
    /* center the divs in their containing elements */
    div {
      margin: 0 auto;
    }
    ```
- Margin Collapse
![](https://content.codecademy.com/courses/updated_images/diagram-verticalmargins_Updated_1-01.svg)
---
- min-width/max-width
- min-height/max-height

- overflow
    - hidden : when set to this value, any content that overflows will be hidden from view.
    - scroll : when set to this value, a scrollbar will be added to the element’s box so that the rest of the content can be viewed by scrolling.
    - visible : when set to this value, the overflow content will be displayed outside of the containing element. Note, this is the default value.
    
- visibility: hidden/visible 
- The difference between display: none and visibility: hidden? An element with display: element with visibility: hidden, but the space reserved for it will.

### Changing the Box Model
- border-box: The border thickness and padding will be included inside of the box, which means the overall dimensions of the box do not change.
    ``` css
    * {
      box-sizing: border-box;
    }
    ```
    - default value: content-box