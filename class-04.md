Read: 04 - HTML Links, CSS Layout, JS Functions

Links are created using the ``<a>`` element. Users can click on anything
between the opening ``<a>`` tag and the closing ``</a>`` tag. You specify which page you want to link to using the href attribute.

+ Writing Links
``<a href="http://www.link.com">link</a>``

The text between the opening ``<a>`` tag and closing ``</a>`` tag is known as link text

``<a>`` element which has an attribute called ``href``. The value of the
href attribute is the page that you want people to go to when they click on the link. Users can click on anything that appears between the opening
``<a>`` tag and the closing ``</a>``

what is the **URL**?

**URL** stands for Uniform Resource Locator

what is **absolute URL**?
When you link to a different website, the value of the href attribute will be the full web address for the site, which is
known as an  **absolute URL**

  + Every web page has its own URL. This is the web address that you would type into a browser if you wanted to visit that specific page.
  + An absolute URL starts with the domain name for that site, and can be followed by the path to a specific page. If no page is specified, the site will display the homepage

what is **relative URL**?

 + When you are linking to other pages within the same site, you do not need to specify the domain name in the URL. You can use a shorthand known as a relative URL
 + When linking to other pages within the same site, you can use relative URLs. These are like a shorthand version of absolute URLs because you do not need to specify the domain name.

**Email Links**
- mailto:To create a link that starts up the user's email program and addresses an email to a specified email address, you use the ``<a>`` element. However, this time the value of the href attribute starts with mailto: and is followed by
the email address you want the email to be sent to.

How to Opening Links in a New Window?

target If you want a link to open in a new window, you can use the target attribute on the opening ``<a>`` tag. The value of this attribute should be`` _blank.``

``<a href="http://www.imdb.com" target="_blank">Internet Movie Database</a> ``(opens in new window)



- if you are linking to a page within your own site, it is best to use relative links rather than qualified URLs.
-  You can create links to open email programs with an email address in the "to" field.
-  You can use the id attribute to target elements within a page that can be linked to.




+ <div> elements are often used as containing elements to group together sections of a page.

+ Browsers display pages in normal flow unless youspecify relative, absolute, or fixed positioning.

+ The float property moves content to the left or right of the page and can be used to create multi-column layouts. (Floated items require a defined width.)

+ Pages can be fixed width or liquid (stretchy) layouts.

+ Designers keep pages within 960-1000 pixels wide, and indicate what the site is about within the top 600 pixels (to demonstrate its relevance without scrolling).

+ Grids help create professional and flexible designs.

+ CSS Frameworks provide rules for common tasks.

+ You can include multiple CSS files in one page


---------------------------------------------------

**WHAT IS A FUNCTION?**
Functions let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of statements). 


JavaScript functions are defined with the function keyword.

You can use a function declaration or a function expression.
``function functionName(parameters) {``
 `` // code to be executed``
``} ``
**Function Expressions**
+ A JavaScript function can also be defined using an expression.

+ A function expression can be stored in a variable:
+ The function above is actually an anonymous function (a function without a name). Functions stored in variables do not need function names. They are always invoked (called) using the variable name.
``var x = function (a, b) {return a * b};``

VARIABLE SCOPE :

![SPCOPU](https://www.bookofnetwork.com/images/javascript-images/JS_Slide-120_03Mar17_1111.png)



WHAT IS AN OBJECT? 
Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names. 



