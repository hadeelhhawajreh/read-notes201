Read: 07 - HTML Tables; JS Constructor Functions


Definition and Usage
The`` <table> ``tag defines an HTML table.

An HTML table consists of one ``<table> ``element and one or more ``<tr>``, ``<th>``, and ``<td>`` elements.

The ``<tr>`` element defines a table row, the ``<th>`` element defines a table header, and the ``<td> ``element defines a table cell.

An HTML table may also include ``<caption>``, ``<colgroup>``, ``<thead>``, ``<tfoot>``, and ``<tbody> ``elements.

+ Table Heading
Table heading can be defined using ``<th>`` tag. This tag will be put to replace ``<td>`` tag, which is used to represent actual data cell. Normally you will put your top row as table heading as shown below, otherwise you can use ``<th> ``element in any row. Headings, which are defined in <th> tag are centered and bold by default.
  
+ Cellpadding and Cellspacing Attributes
There are two attributes called cellpadding and cellspacing which you will use to adjust the white space in your table cells. The cellspacing attribute defines space between table cells, while cellpadding represents the distance between cell borders and the content within a cell.

Colspan and Rowspan Attributes
You will use colspan attribute if you want to merge two or more columns into a single column. Similar way you will use rowspan if you want to merge two or more rows.

	
   ``<body>``
   
      ``<table border = "1">``
      
        `` <tr>``
        
          ``  <th>Column 1</th>``
          
          ``<th>Column 2</th>``
          
            ``<th>Column 3</th>``
            
         ``</tr>``
         
        
         ``<tr>``
         
          ``  <td rowspan = "2">Row 1 Cell 1</td>``
          
           `` <td>Row 1 Cell 2</td>``
           
            ``<td>Row 1 Cell 3</td>``
            
         ``</tr>``
         
         ``<tr>``
         
           `` <td>Row 2 Cell 2</td>``
           
            ``<td>Row 2 Cell 3</td>``
            
        `` </tr>``
        
       
         ``<tr>``
         
          ``  <td colspan = "3">Row 3 Cell 1</td>``
          
        `` </tr>``
        
      ``</table>``
      
   ``</body>``
   
   
   + Tables Backgrounds
    You can set table background using one of the following two ways −

    + bgcolor attribute − You can set background color for whole table or just for one cell.

    
     + background attribute − You can set background image for whole table or just for one cell. You can also set border color also using bordercolor attribute.
     
  
  + Table Caption
The caption tag will serve as a title or explanation for the table and it shows up at the top of the table. This tag is deprecated in newer version of HTML/XHTML.

**Table Header, Body, and Footer**
Tables can be divided into three portions − a header, a body, and a foot. The head and foot are rather similar to headers and footers in a word-processed document that remain the same for every page, while the body is the main content holder of the table.

The three elements for separating the head, body, and foot of a table are −

``<thead> ``− to create a separate table header.

``<tbody>`` − to indicate the main body of the table.

``<tfoot>`` − to create a separate table footer.

A table may contain several ``<tbody>`` elements to indicate different pages or groups of data. But it is notable that ``<thead>`` and ``<tfoot>`` tags should appear before ``<tbody>``


 -------------------------------------------------------------------------------------------------------------------------------------  
 + Object Properties
Object properties can be any of the three primitive data types, or any of the abstract data types, such as another object. Object properties are usually variables that are used internally in the object's methods, but can also be globally visible variables that are used throughout the page.

The syntax for adding a property to an object is −

objectName.objectProperty = propertyValue;
For example − The following code gets the document title using the "title" property of the document object.

``var str = document.title;``

+ Object Methods
Methods are the functions that let the object do something or let something be done to it. There is a small difference between a function and a method – at a function is a standalone unit of statements and a method is attached to an object and can be referenced by the this keyword.

Methods are useful for everything from displaying the contents of the object to the screen to performing complex mathematical operations on a group of local properties and parameters.

For example − Following is a simple example to show how to use the write() method of document object to write any content on the document.

``document.write("This is test");``

``var book = new Object();   // Create the object``

   ``      book.subject = "Perl";     // Assign properties to the object``
   
        `` book.author  = "Mohtashim";``
        

+ The`` this`` Keyword
In JavaScript, the thing called this is the object that "owns" the code.

The value of this, when used in an object, is the object itself.

In a constructor function this does not have a value. It is a substitute for the new object. The value of this will become the new object when a new object is created.

Note that this is not a variable. It is a keyword. You cannot change the value of this.

> Did You Know?
As you can see above, JavaScript has object versions of the primitive data types String, Number, and Boolean. But there is no reason to create complex objects. Primitive values are much faster.

> ALSO:

Use object literals {} instead of new Object().

Use string literals "" instead of new String().

Use number literals 12345 instead of new Number().

Use boolean literals true / false instead of new Boolean().

Use array literals [] instead of new Array().

Use pattern literals /()/ instead of new RegExp().

Use function expressions () {} instead of new Function().
