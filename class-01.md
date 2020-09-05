duckett_html.
## 1. HTML 
HTML is used to create web pages,e. You then add tags
or elements to the words so that the browser knows what is a heading, where a paragraph begins and ends, and so on.
## 2. CSS 
 that explains how CSS uses rules to enable you to control the styling and layout of web pages
Presentation: How to control things like the color of text, the fonts you want to use and the size of those fonts, how to add
background colors to pages (or parts of a page), and how to add background images.

--------------------------------------------------------------------------------------------------------------------------------------------------
**Layout:
 How to control where the different elements are positioned on the screen,s use to make
their pages more attractive.**

  > HTML5 is the latest version of HTML (still under development at the time of writing)*

#  How People Access the Web :different ways in which people access the web and clarify some terminology
 * Browsers People access websites using software called a web browser. 
* Web Servers: When you ask your browser for a web page, the request is sent across the Internet to a special computer known as a web server which hosts  he website.
  * what is the Web servers?
   * Web servers are special computers that are constantly connected to the Internet, and are optimized to send web pages out to people who request them.
* Devices
* Screen readers
  * what is Screen readers?
  * Screen readers are programs that read out the contents of a computer screen to a user. They are commonly used by people with visual impairments.

----------------------------------------------------------------------------------------------------------------------------------------------------
# How Websites Are Created?
All websites use HTML and CSS, but content management systems, blogging software, and e-commerce platforms often add a few more
technologies into the mix.

# How the Web Works?

+ When you connect to the web, you do so via an Internet Service Provider (ISP). You type a domain name or web address into your browser to visit a site.

+ Your computer contacts a network of servers called Domain Name System (DNS) servers. These act like phone
books; they tell your computer the IP address associated with the requested domain name. An IP address is a number of up to 12 digits separated by periods / full stops. Every device connected to the web has a unique IP address; it is like the phone number for that computer.

+ The unique number that the DNS server returns to your computer allows your browser to contact the web server that hosts the website you requested. A web server is a computer that is constantly connected to the web, and is set up especially to send web pages to users.

+ The web server then sends the page you requested back to your web browser.
-------------------------------------------------------------------------------------------------------------------------------------------------

**The HTML code**  is made up of characters that live inside angled
brackets — these are called HTML elements. Elements are usually
made up of two tags: an opening tag and a closing tag. (The closing tag
has an extra forward slash in it.) Each HTML element tells the browser
something about the information that sits between its opening and
closing tags
``<p>`` opening tag
``</p>`` closing tag

Attributes provide additional information
about the contents of an element. They appear
on the opening tag of the element and are
made up of two parts: a name and a value,
separated by an equals sign.
``<p lang="en-us">Paragraph in English</p>``
``lang ``  Attribute Name
``"en-us"`` Attribute Value

``<body>`` Everything inside this element is
shown inside the main browser
window.
``<head>``
This contains information
about the page (rather than
information that is shown within
the main part of the browser
window that is highlighted in
blue on the opposite page).
You will usually find a`` <title>``
element inside the`` <head>``
element.
``<title>``
The contents of the`` <title>``
element are either shown in the
top of the browser, title tags will appear in the
title bar (or tabs) at the top of
the browser window

 versions of HTML.
| version   |  Released | properties |
|----------|:-------------:|------:|
| HTML4  |  1997 | Although HTML 4 had some presentational elements to control the appearance of pages, authors are not recommended to use them any more |
| XHTML |    2000   |   it was decided that HTML 4 should be reformulated to follow the rules of XML and it was renamed XHTML.  |
| HTML5 | latest version-2000  |   In HTML5, web page authors do not need to close all tags, and new elements and attributes will be introduced.  |
 

``DOCTYPEs``Because there have been
several versions of HTML, each
web page should begin with a
DOCTYPE declaration to tell a
browser which version of HTML
the page is using

**Comments in HTML** ``<!-- comment goes here -->``
It is a good idea to add
comments to your code because,
no matter how familiar you
are with the page at the time
of writing it, when you come
back to it later (or if someone
else needs to look at the code),
comments will make it much
easier to understand

| ID Attributes|Class Atrributes|
|--------------|----------------|
| Every HTML element can carry  the id attribute. It is used to uniquely identify that element from other elements on the page. Its value should start with a letter or an underscore (not a number or any other character). |   Sometimes, rather than uniquely identifying one element within a document, you will want a way to identify several elements |
|Block Elements |INline Elements |
|--------------|----------------|
|Some elements will always appear to start on a new line in the browser window. These are known as block level elements``.<h1>``, ``<p>``,`` <ul>``, and`` <li>.``|Some elements will always appear to continue on the same line as their neighbouring elements. These are known as inline elements. Examples of inline elements are ``<a>``, ``<b>``, ``<em>``, and ``<img>``.|

+ The`` <div>`` and ``<span> ``elements allow you to group block-level and inline elements together.
+`` <iframes> ``cut windows into your web pages through which other pages can be displayed.
+ The ``<meta>`` tag allows you to supply all kinds of
information about your web page.
+ Escape characters are used to include special
characters in your pages such as`` <``, ``>``, and`` ©``

*What is a wireframe?

A wireframe is a simple sketch of the key
information that needs to go on each page of a
site. It shows the hierarchy of the information
and how much space it might require.

+ The new HTML5 elements indicate the purpose of
different parts of a web page and help to describe
its structure.
+  The new elements provide clearer code (compared
with using multiple ``<div>`` elements).
X Older browsers that do not understand HTML5
elements need to be told which elements are
block-level elements.
+  To make HTML5 elements work in Internet Explorer 8
(and older versions of IE), extra JavaScript is needed,
which is available free from Google.
