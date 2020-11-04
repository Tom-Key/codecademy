### HTML Tables
``` html
<table > <!-- create the table that will contain the data -->
   <tr>
    <th></th> <!--  table heading element -->
    <th scope="col">Saturday</th>
    <th scope="col">Sunday</th>
  </tr>
  <tr> <!-- table rows -->
    <td>73</td> <!-- add data using the table data element: <td> -->
    <td>81</td>
  </tr>
</table>
``` 
- `<td colspan="2">Out of Town</td>` span columns using the `colspan/rowspan` attribute.
- 

- In older versions of HTML, a border could be added to a table using the border attribute and setting it equal to an integer.You can achieve the same table border effect using CSS.
    ``` css
    table, td {
      border: 1px solid black;
    }
    ```
- Long tables can be sectioned off using the table body element: `<tbody>`
- `<thead>` element: table’s column headings 
- `<tfoot>` element: sectioned off
--- 
#### Styling with CSS
``` css
table, th, td {
  border: 1px solid black;
  font-family: Arial, sans-serif;
  text-align: center;
}
```