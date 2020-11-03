### Flexbox
``` css
/* In the example above, all divs with the class container are flex containers. 
If they have children, the children are flex items. */
div.container {
  display: flex;
}
```
- Flexible Box Layout : A new tool developed for CSS3 that greatly simplifies how to position elements
-  flex containers and flex items
- A div with the declaration display: flex; will remain block level;it will change the behavior of its child elements. Child elements will not begin on new lines.
---
- `display: inline-flex;`  : flex containers that are also inline elements·
- `justify-content: flex-end`
    - flex-start : in order starting, from the left of the parent container, with no extra space between or before them.
    - flex-end: positioned in order, with the last item starting on the right side of the parent container, with no extra space between or after them.
    - center:  in the center of the parent container with no extra space before, between, or after them.
    - space-around:positioned with equal space before and after each item, resulting in double the space between elements.
    - space-between：be positioned with equal space between them, but no extra space before the first or after the last elements.
    
---

- `align-items:`: makes it possible to space flex items vertically
    - flex-start : all elements will be positioned at the top of the parent container
    - flex-end: all elements will be positioned at the bottom of the parent container.
    - center : all elements will be positioned halfway between the top and bottom of the parent container.
    - baseline : the **bottom** of the the content of all items will be aligned with each other.
    - stretch ： if possible, the items will stretch from top to bottom of the container (this is the default value; elements with a specified height will not stretch; elements with a minimum height or no height specified will stretch)
--- 
- `flex: 2(flex-grow) 1(flex-shrink,optional) 150px(flex-basis,optional)`
    - The flex property is different from the flex value used for the display property.
- `flex-grow:ratio`: specify if items should grow to fill a container and also which items should grow proportionally more or less than others.
- `flex-shrink:1(default)` property can be used to specify which elements will shrink and in what proportions.
- `flex-basis`:allows us to specify the width of an item before it stretches or shrinks.
---
- `flex-flow: column wrap;` declare both the flex-wrap and flex-direction properties in one line.

- `flex-wrap`: flex items to move to the next line when necessary
    - wrap
    - wrap-reverse
    - nowrap:  override a wrap value set by a different CSS rule.
- `align-content`: space the rows from top to bottom.
    - *The parameters are the same as align-items*
- `flex-direction: column;`
    - `row/row-reverse/column/column-reverse`
---- 
#### Nested Flexboxes
``` html
<div class="container">
  <div class="left">
    <img class="small" src="#"/>
    <img class="small" src="#"/>
    <img class="small" src="#" />
  </div>
  <div class="right">
    <img class="large" src="#" />
  </div>
</div>
```
``` css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}

.left {
  display: inline-flex;
  flex: 2 1 200px;
  flex-direction: column;
}

.right {
  display: inline-flex;
  flex: 1 2 400px;
  align-items: center;
}

.small {
  height: 200px;
  width: auto;
}

.large {
  height: 600px; 
  width: auto;
}
```
