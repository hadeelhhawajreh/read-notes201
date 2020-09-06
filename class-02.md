Readings : Basics of HTML, CSS & JS

● **Structural markup:** 
the elements that you can use to describe both headings and paragraphs

● **Semantic markup:** which provides extra information; such as where emphasis is placed in a sentence, that something you have written is a quotation (and who said it), the meaning of acronyms, and so on

Headings

``<h1>`` -->  is used for main headings

``<h2>``  is used for subheadings
``<h3>``
``<h4>``
``<h5>``
``<h6>``

``<p>`` 
To create a paragraph, surround the words that make up the paragraph with an ``<p>`` opening  tag and  `` </p> ``closing tag.

``<b>``
By enclosing words in the tags ``<b>`` and`` </b>`` we can make
characters appear bold. The`` <b>`` element also represents a section of text that would be presented in a visually different way.

``<i>`` By enclosing words in the tags ``<i>`` and ``</i>`` we can make characters appear italic.

``<sup>``
The ``<sup>`` element is used to contain characters that should be superscript such as the suffixes of dates or mathematical concepts like raising a number to a power 

``<sub>`` The`` <sub>`` element is used to
contain characters that should be subscript. It is commonly used with foot notes or chemical formulas such as H20.

what is white space collapsing?
When the browser comes across two or more spaces next to each other, it only displays one space. Similarly if it comes across a line break, it treats that as a single space too. This is known as *white space collapsing*

``<br />``
if you wanted  to add a line break inside the middle of a paragraph you can  use the line break tag <br />.

``<hr />``
— you can add a horizontal rule between sections using the <hr /> tag. There are a few elements that do not have any words between an opening and closing tag. They
are known as *empty elements

``<strong>`` The use of the <strong> element indicates that its content has strong importance. 
  
 `` <em>``
The`` <em>`` element indicates emphasis that subtly changes the meaning of a sentence. By default browsers will show the contents of an`` <em> ``element
in italic.
> There are two elements commonly used for marking up quotations:
* ``<blockquote>``
The ``<blockquote>`` element is used for longer quotes that take up an entire paragraph. 
* ``<q>``
The `` <q> ``element is used for shorter quotes that sit within a paragraph.

``<abbr>``
If you use an abbreviation or an acronym, then the <abbr> element can be used. A title attribute on the opening tag is used to specify the full term.
  
 `` <cite>``
When you are referencing a piece of work such as a book, film or research paper, the ``<cite>`` element can be used to indicate where e the citation is
from.
In HTML5,`` <cite>`` should not really be used for a person's name
  Browsers will render the content of a`` <cite> ``element in italics.
 The ``<dfn>`` element is used to the defining instance of a new term. Some browsers show the content of the`` <dfn>`` element in italics.
 
`` <address>``
The <address> element has quite a specific use: to contain contact details for the author of the page.
+It can contain a physical address, phone number or email address.
 + Browsers often display the content of the  ``<address> `` element in italics.
  
 ``<ins>`` ,``<del>``
The ``<ins>`` element can be used to show content that has been inserted into a document, while the`` <del>`` element can show text that has been deleted from it. The content of a ``<ins>`` element is usually underlined, while the content of a ``<del>`` elementusually has a line through it.
`` <s>``
element will usually be displayed with a line through the center.
# css 
CSS allows you to create rules that specify how the content of
an element should appear. For example, you can specify that
the background of the page is cream, all paragraphs should
appear in gray using the Arial typeface, or that all level one
headings should be in a blue, italic, Times typeface.

# CSS Associates Style rules with HTML elements

CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration.
p {
 font-family: Arial;}
 P -> is a  Selectors indicate which element the rule applies to.  The same rule can apply to more than one element if you separate the element names
with commas.
font-family: Arial; -> Declarations indicate how the elements referred to in the selector should be styled. Declarations are split into two parts (a property and a value),
and are separated by a colon.
 -> CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon. You can specify
 several properties in one declaration, each separated by a semi-colon.
  
  **Common  Type of selector**
  |Selector           | Meaning                                 |  Example  |
  |-------------------|:---------------------------------------:|----------:|
  |Universal Selector |  Applies to all elements in the documen | * {}      |
  |Type Selector      |  Matches element namesn                 |h1,h2...   |
  |Class Selector     |Matches an element whose class attribute |.className |
  |ID Selector        | Matches an element whose id attribute   |#id        |
  
  
  *another type selector:
  -Child Selector
  -Descendant Selector
  -Adjacent Sibling
  -Selector
  -General Sibling
  -Selector
  
  
# HOW APPLAYING CSS
1.INLINE
2.EXTERNAL
3.EXTERNAL


* CSS treats each HTML element as if it appears inside its own box and uses rules to indicate how that element should look.
*  Rules are made up of selectors (that specify the elements the rule applies to) and declarations (that indicate what these elements should look like).
*  Different types of selectors allow you to target your rules at different elements.
*  Declarations are made up of two parts: the properties of the element that you want to change, and the values of those properties. For example, the font-family property sets
----------------------------------------------------------------------------------------------------------

+ A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon. 

+ You should write comments to explain what your code does. They help make your code easier to read and understand. This can help you and others who read your code.


 |MULTI-LINE COMM ENTS| SINGLE-LINE COMMENTS|
 |--------------------|:-------------------:|
 |To write a comment that stretches over more than one line, you use a multi-line comment, starting with the ``/* characters and ending with the */ characters.``|In a single line comment, anything that follows the two forward slash characters I/ on that line will not be processed by the JavaScript interpreter|
|M ulti-line comment s are often used for descriptions of how the script works, or to prevent a section of the script from running when testing it| Singleline comments are often used for short descriptions of what the code is doing.|

+ VARIABLES :
  ``var x=5;``
  + RULES FOR NAMING VARIABLES
  +The name must begin with a letter, dollar sign ($),or an underscore (_). It must not start with a number. 
  + The name can contain letters, numbers, dollar sign ($), or an underscore (_). Note that you must not use a dash(-) or a period (.) in a variable name
  + You cannot use keywords or reserved words.
  + All variables are case sensitive, so score and Score would be different variable names

+ DATA TYPES 

 |NUMERIC DATA TYPE            | STRING DATA TYPE  |  BOOLEAN DATA TYPE  |
 |-------------------|:---------------------------------------:|----------:|
 |The numeric data type handles numbers. |The strings data type consists of letters and other characters. |Boolean data types can have one of two values: true or false.|
 |Example: 7.5|'hi,how are you'|true|
 
