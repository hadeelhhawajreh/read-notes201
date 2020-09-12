JS Object Literals; The DOM
+ Object is a non-primitive data type in JavaScript. It is like any other variable, the only difference is that an object holds multiple values in terms of properties and methods. Properties can hold values of primitive data types and methods are functions.

+ The Object class represents one of JavaScript's data types. It is used to store various keyed collections and more complex entities.

Let's learn how to create an object in JavaScript.
``var <object-name> = { key1: value1, key2: value2,... keyN: valueN};``

``var Person = function(name) {``

  ``this.name = name;``
  
  ``this.canTalk = true;``
  
``};``


+ Access JavaScript Object Properties & Methods
 + You can get or set values of an object's properties using dot notation or bracket. However, you can call an object's method only using dot notation.
 
 
`` var person = { ``

              ``  firstName: "James",``
              
              ``  lastName: "Bond", ``
              
                `` age: 25, ``
              
            ``};``

``person.firstName; // returns James``

`` person.lastName; // returns Bond ``

``person["firstName"];// returns James``

``person["lastName"];// returns Bond``


# THE DOM TREE IS A
MODEL OF A WEB PAGE
As a browser loads a web page, it creates a model of that page.
The model is called a DOM tree, and it is stored in the browsers' memory.
It consists of four main types of nodes

THE DOCUMENT NODE
, you can see the HTML code for a shopping
list, and on the right hand page is its DOM tree.
Every element, attribute, and piece of text in the
HTML is represented by its own DOM node.
At the top of the tree a document node is added; it
represents the entire page (and also corresponds to
the document object, which you first met on p36).
When you access any element, attribute, or text
node, you navigate to it via the document node. It is
the starting point for all visits to the DOM tree. 


What is the DOM?
The Document Object Model (DOM) is a programming interface for HTML and XML documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects. That way, programming languages can connect to the page.

A Web page is a document. This document can be either displayed in the browser window or as the HTML source. But it is the same document in both cases. The Document Object Model (DOM) represents that same document so it can be manipulated. The DOM is an object-oriented representation of the web page, which can be modified with a scripting language such as JavaScript.

For example, the standard DOM specifies that the getElementsByTagName method in the code below must return a list of all the <p> elements in the document:
  
![img](https://res.cloudinary.com/practicaldev/image/fetch/s--B2Ts1hyb--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/http://i67.tinypic.com/2nqegt2.jpg)
