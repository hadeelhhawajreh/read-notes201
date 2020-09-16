form and event
The ``<form>`` Element
The HTML ``<form>`` element is used to create an HTML form for user input.

 The ``<form>`` element is a container for different types of input elements, such as: text fields, checkboxes, radio buttons, submit buttons, etc.


The <input> Element
The HTML <input> element is the most used form element.

An <input> element can be displayed in many ways, depending on the type attribute.

|Type |	Description |
|----:|-----------:|
|``<input type="text">``|Displays a single-line text input field|
|``<input type="radio">``|	Displays a radio button (for selecting one of many choices)|
|``<input type="checkbox">``|	Displays a checkbox (for selecting zero or more of many choices)|
|``<input type="submit">``|Displays a submit button (for submitting the form)|
|``<input type="button">`` |Displays a clickable button|
+ Text Fields

The ``<input type="text"> ``defines a single-line input field for text input.
The ``<label> ``Element
Notice the use of the ``<label>`` element in the example above.

The ``<label>`` tag defines a label for many form elements.

The ``<label> ``element is useful for screen-reader users, because the screen-reader will read out loud the label when the user focus on the input element.

The ``<label>`` element also help users who have difficulty clicking on very small regions (such as radio buttons or checkboxes) - because when the user clicks the text within the ``<label>`` element, it toggles the radio button/checkbox.

The for attribute of the <label> tag should be equal to the id attribute of the <input> element to bind them together.

+ Radio Buttons
The ``<input type="radio"> ``defines a radio button.

![radio](https://i.stack.imgur.com/JLiqT.png)

Radio buttons let a user select ONE of a limited number of choices.


+ Checkboxes
The <input type="checkbox"> defines a checkbox.

Checkboxes let a user select ZERO or MORE options of a limited number of choices.
![check](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQgxMKJOXeNbH9G-6CnyzNjhb1_9BIrYy_Xag&usqp=CAU)

+ The Submit Button
The``<input type="submit">`` defines a button for submitting the form data to a form-handler.

The form-handler is typically a file on the server with a script for processing input data.

The form-handler is specified in the form's action attribute.


- The formmethod Attribute
>The input formmethod attribute defines the HTTP method for sending form-data to the action URL.

>The formmethod attribute works with the following input types: submit and image.
>The form-data can be sent as URL variables (method="get") or as an HTTP post transaction (method="post").

+ Notes on the "get" method:

>This method appends the form-data to the URL in name/value pairs
>This method is useful for form submissions where a user want to bookmark the result
>There is a limit to how much data you can place in a URL (varies between browsers), therefore, you cannot be sure that all of the form-data will be correctly transferred
>Never use the "get" method to pass sensitive information! (password or other sensitive information will be visible in the browser's address bar)

+ Notes on the "post" method:

>This method sends the form-data as an HTTP post transaction
>Form submissions with the "post" method cannot be bookmarked
>The "post" method is more robust and secure than "get", and "post" does not have size limitations



What can JavaScript Do?
Event handlers can be used to handle, and verify, user input, user actions, and browser actions:

Things that should be done every time a page loads
Things that should be done when the page is closed
Action that should be performed when a user clicks a button
Content that should be verified when a user inputs data
And more ...
Many different methods can be used to let JavaScript work with events:

- HTML event attributes can execute JavaScript code directly
+ HTML event attributes can call JavaScript functions
+ You can assign your own event handler functions to HTML elements
+ You can prevent events from being sent or being handled ,And more ...

![event](https://data-flair.training/blogs/wp-content/uploads/sites/2/2019/07/Ways-of-Using-JavaScript-Events.png)
