### HTML Forms
#### How a Form Works
- We can think of the internet as a network of computers which send and receive information.
- The `<form>` element is a great tool for collecting information, but then we need to send that information somewhere else for processing.

``` html
<!-- The action attribute determines where the information is sent. -->
<!-- The method attribute is assigned a HTTP verb that is included in the HTTP request. -->
<form action="/example.html" method="POST">
    <label for="username">Username</label>
    <input type="text" name="username_" value="already pre-filled" id="username">
</form>
```
- `type="password"`:replace input text with another character like an asterisk (*) or a dot (•). 
- `type="number"`restrict what users type into the input field to just numbers (and a few special characters like -, +, and .).
    - `step="1"`
    -  `type="range" min="0" max="100"`
- `<input type="checkbox" id="lettuce" name="topping" value="lettuce">
`
- Radio Button Input
``` html
<form>
  <p>What is sum of 1 + 1?</p>
  <input type="radio" id="two" name="answer" value="2">
  <label for="two">2</label>
  <br>
  <input type="radio" id="eleven" name="answer" value="11">
  <label for="eleven">11</label>
</form>
```
- dropdown list
``` html
<form>
  <label for="lunch">What's for lunch?</label>
  <select id="lunch" name="lunch">
    <option value="pizza">Pizza</option>
    <option value="curry">Curry</option>
    <option value="salad">Salad</option>
    <option value="ramen">Ramen</option>
    <option value="tacos">Tacos</option>
  </select>
</form>
```
- Datalist Input
``` html
<form>
  <label for="city">Ideal city to visit?</label>
  <input type="text" list="cities" id="city" name="city">

  <datalist id="cities">
    <option value="New York City"></option>
    <option value="Tokyo"></option>
    <option value="Barcelona"></option>
  </datalist>
</form>
```
- Text Area
``` html
<textarea id="blog" name="blog" rows="5" cols="30">
</textarea>
```
- Submit Form
- `<input type="submit" value="Send">`
### Form Validation
    