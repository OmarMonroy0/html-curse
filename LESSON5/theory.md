# TABLES.

We use the tag

```html
<table> 

</table>
```

To create a table, the table will consist of a some number of rows and columns


```html
<table> 
    <tr>
        <td> $100</td>
        <td> $200 </td>
    </tr>
</table>
```
**tr** indicates  a row and **td** indicates a new table data so for this code we get

| $100 | $200  |
| ---- | :---: |

Now we can add another row and we obtained the next table

```html
<table> 
    <tr>
        <td> $100</td>
        <td> $200 </td>
    </tr>
    <tr>
        <td> $300 </td>
        <td> $400 </td>
    </tr>
</table>
```

| $100 | $200  |
| ---- | :---: |
| $300 | $400  |

As you can see in the table we have to place headings, to add heading to table we have to add the next code

```html
<table> 
    <tr>
        <th>First Heading</th>
        <th>Second Heading </th>
    </tr>
    <tr>
        <td> $100</td>
        <td> $200 </td>
    </tr>
    <tr>
        <td> $300 </td>
        <td> $400 </td>
    </tr>
</table>
```

| Head 1 | Head 2 |
| ------ | ------ |
| $100   | $200   |
| $300   | $400   |


As you can see the head tag is in black, but we can also use headers in the next rows not only in the first

### adding some headers in each row
<table>
    <tr>
        <th scope = "col"> First </th>
        <th scope = "col"> Second </th>
        <th scope = "col"> Third </th>
    </tr>
    <tr>
        <th scope = "row"> Product 1 </th>
        <td> $100 </td>
        <td> $200 </td>
    </tr>
    <tr>
        <th scope = "row"> Product 1 </th>
        <td> $300 </td>
        <td> $400 </td>
    </tr>
</table>

We use the scope to indicate if the header is for a column 
or for the row.


But as we have seen until this moment in html we have semantic grouping tags the first part only contains headers and the rest of the table is the body of the table.

### table head and table body

<table>
    <thead>
        <tr>
            <th scope = "col"> First </th>
            <th scope = "col"> Second </th>
            <th scope = "col"> Third </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope = "row"> Product 1 </th>
            <td> $100 </td>
            <td> $200 </td>
        </tr>
        <tr>
            <th scope = "row"> Product 2 </th>
            <td> $300 </td>
            <td> $400 </td>
        </tr>
    </tbody>
</table>


We have the same result however we have enclosed the corresponding tags into semantic grouping tags for the table


### Table footer

We can also add a footer to the table

<table>
    <thead>
        <tr>
            <th scope = "col"> First </th>
            <th scope = "col"> Second </th>
            <th scope = "col"> Third </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope = "row"> Product 1 </th>
            <td> $100 </td>
            <td> $200 </td>
        </tr>
        <tr>
            <th scope = "row"> Product 2 </th>
            <td> $300 </td>
            <td> $400 </td>
        </tr>
    </tbody>
    <tfoot>
        <th scope = "row"> Total </th>
        <td> $400 </td>
        <td> $600 </td>
    </tfoot>

</table>

### Naming the table


<table>
    <caption> Name of the table </caption>
    <thead>
        <tr>
            <th scope = "col"> First </th>
            <th scope = "col"> Second </th>
            <th scope = "col"> Third </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope = "row"> Product 1 </th>
            <td> $100 </td>
            <td> $200 </td>
        </tr>
        <tr>
            <th scope = "row"> Product 2 </th>
            <td> $300 </td>
            <td> $400 </td>
        </tr>
    </tbody>
    <tfoot>
        <th scope = "row"> Total </th>
        <td> $400 </td>
        <td> $600 </td>
    </tfoot>

</table>


### ATRIBUTE "COLSPAN"

This attribute is used to indicate how many columns is going to use 

<table>
    <thead>
        <tr>
            <th colspan="2" scope = "col"> First (this cell uses 2 columns)</th>
            <th scope = "col"> Second </th>
            <th scope = "col"> Third </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope = "row"> Product 1 </th>
            <td> $100 </td>
            <td> $200 </td>
        </tr>
        <tr>
            <th scope = "row"> Product 2 </th>
            <td> $300 </td>
            <td> $400 </td>
        </tr>
    </tbody>
    <tfoot>
        <th scope = "row"> Total </th>
        <td> $400 </td>
        <td> $600 </td>
    </tfoot>

</table>

As you can see now the table takes 2 columns 


### COLGROUP TAG

This tag is used to perform actions in a certain group of columns

<table>
    <colgroups>
        <col span="2" style="background: red"/>
    </colgroups>
    <thead>
        <tr>
            <th colspan="2" scope = "col"> First (this cell uses 2 columns)</th>
            <th scope = "col"> Second </th>
            <th scope = "col"> Third </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <th scope = "row"> Product 1 </th>
            <td> $100 </td>
            <td> $200 </td>
        </tr>
        <tr>
            <th scope = "row"> Product 2 </th>
            <td> $300 </td>
            <td> $400 </td>
        </tr>
    </tbody>
    <tfoot>
        <th scope = "row"> Total </th>
        <td> $400 </td>
        <td> $600 </td>
    </tfoot>

</table>


As you can see in the output we are giving color to 2 columns because of the span = 2 this really helpful when we need to give styles.