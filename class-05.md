Readings : Images, Color, Text

``<img>``
To add an image into the page
you need to use an ``<img>``
element. This is an empty
element (which means there is
no closing tag). It must carry the
following two attributes:
``src``
This tells the browser where
it can find the image file. This
will usually be a relative URL
pointing to an image on your
own site. (Here you can see that
the images are in a child folder
called images — relative URLs
were covered on pages 83-84).
``alt``
This provides a text description
of the image which describes the
image if you cannot see it.
``title``
You can also use the title
attribute with the ``<img>`` element
to provide additional information
about the image. Most browsers
will display the content of this
attribute in a tootip when the
user hovers over the image.

You will also often see an ``<img>``
element use two other attributes
that specify its size:
``height``
This specifies the height of the
image in pixels.
``width``
This specifies the width of the
image in pixels.

``align ``
The align attribute was
commonly used to indicate how
the other parts of a page should
flow around an image. It has
been removed from HTML5
and new websites should use
CSS to control the alignment of
images 
The align attribute can take these horizontal values:
+ ``left``
This aligns the image to the left
(allowing text to flow around its
right-hand side).

+ ``right``
This aligns the image to the right (allowing text to flow around its left-hand side).

There are three values that the
align attribute can take that
control how the image should
align vertically with the text that
surrounds it:
+ ``top``
This aligns the first line of the
surrounding text with the top of
the image.
+ ``middle``
This aligns the first line of the
surrounding text with the middle
of the image.
+ ``bottom``
This aligns the first line of the
surrounding text with the bottom
of the image.
 
 There are three rules to remember when you
are creating images for your website which are
summarized below. We go into greater detail
on each topic over the next nine pages  

1. Save images in
the right format
2. Save images at
the right size
3. Use the correct
resolution





The properties that allow you to control the appearance of text can be split into two groups:

● Those that directly affect the font and its appearance (including the typeface, whether it is regular, bold or italic, and the size of the text)

● Those that would have the same effect on text no matter what font you were using (including the color of text and the spacing between words and letters)

*Choosing a Typeface for your Website*
When choosing a typeface, it is important to understand that a browser will usually only display it if it's installed on that user's computer As a result, sites often use a small set of typefaces that are installed on most computers .

Browsers are supposed to support at least one typeface from each of the groups above. For this reason, it is common to add the generic font  name after your preferred choice of typefaces.
For example, if you wanted serif type, you could write the following: ``font-family: Georgia, Times, serif;``

 Typefaces are subject to copyright, so the techniques you can choose from are limited by their respective licenses
 
 + Specifying Typefaces
   + font-family :The font-family property allows you to specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies. The value of this      property is the name of the typeface you want to use
     ``body { font-family: Georgia, Times, serif;}``
   + Size of Type 
     + font-size
     The font-size property enables you to specify a size for the font. There are several ways to specify the size of a font. The most common are:

      + pixels Pixels are commonly used because they allow web designers very precise control over how much space their text takes up. The number of pixels is  followed by the       letters px. percentages The default size of text in browsers is 16px. So a size of 75% would be the equivalent of 12px, and 200% would be 32px.
      + ems An em is equivalent to the width of a letter m.
       `` body {font-family: Arial, Verdana, sans-serif;font-size: 12px;}``
         `` h1 {font-size: 200%;}``
         ``h2 {font-size: 1.3em;}``
         
         
  + More Font Choice
  
   allows you to use a font, even if it is not installed on the computer of the person browsing, by allowing you to specify a path to a copy of the font,    which will be downloaded if it is not on the user's machine

**font-weight**

The font-weight propertyallows you to create bold text. There are two values that this property commonly takes:
 + normal This causes text to appear at a normal weight.
 + bold This causes text to appear bold.

**font-style**

 If you want to create italic text, you can use the font-style property. There are three values this property can take:
 + normal This causes text to appear in a normal style (as opposed to italic or oblique).
 + italic This causes text to appear italic.
 + oblique This causes text to appear oblique
 
**text-transform**

 The text-transform property is used to change the case of text giving it one of the following values:
 + uppercase This causes the text to appear uppercase.
 + lowercase This causes the text to appear lowercase.
 + capitalize This causes the first letter of each word to appear capitalized.
 
 **text-decoration**
 
 The text-decoration property allows you to specify the following values:
 + none This removes any decoration already applied to the text. underline This adds a line underneath the text.
 + overline This adds a line over the top of  the text.
 + line-through This adds a line through words.
 + blink This animates the text to make it flash on and off (however this is generally frowned upon, as it is considered rather annoying).
 
 **line-height**
 
 Leading (pronounced ledding) is a term typographers use for the vertical space between lines of text. 
  ``p {line-height: 1.4em;}``
  
  **letter-spacing, word-spacing**
  You can also control the gap
between words using the
word-spacing property.
When you specify a value for
these properties, it should
be given in ems, and it will be
added on top of the default value
specified by the font.

**The text-align**
property allows
you to control the alignment of
text. The property can take one
of four values:
+ left
This indicates that the text
should be left-aligned.
+ right
This indicates that the text
should be right-aligned.
center
This allows you to center text.
+ justify
This indicates that every line in
a paragraph, except the last line,
should be set to take up the full
width of the containing box.

It is more commonly used with
inline elements such as <img>,
<em>, or <strong> elements.
When used with these elements,
it performs a task very similar to
the HTML align attribute used
on the <img> element, which
you met on pages 103-106. The
values it can take are:
+ baseline
+ sub
+ super
+ top
+ text-top
+ middle
+ bottom
+ text-bottom
  
 **Indenting Text** 
  text-indent
    ``text-indent: -9999px;``.
    
 The text-shadow property has become commonly used despite lacking support in all browsers..
  + The value of this property is
quite complicated because it can
take three lengths and a color for
the drop shadow.
The first length indicates how
far to the left or right the shadow
should fall.
 + The second value indicates the
distance to the top or bottom
that the shadow should fall.
+ The third value is optional and
specifies the amount of blur that
should be applied to the drop
shadow.
+ The fourth value is the color of
the drop shadow.

 ``text-shadow: 1px 1px 0px #000000;``
 
 **Styling Links**
:link, :visited
 In CSS, there are two pseudoclasses that allow you to set
different styles for links that
have and have not yet been  visited.
+ :link
This allows you to set styles
for links that have not yet been visited.
+ :visited
This allows you to set styles for
links that have been clicked on. 
+ :hover
This is applied when a user
hovers over an element with a
pointing device such as a mouse.
This has commonly been used
to change the appearance of
links and buttons when a user
places their cursor over them. 

+ :active
This is applied when an element
is being activated by a user; for
example, when a button is being
pressed or a link being clicked.
Sometimes this is used to make
a button or link feel more like it
is being pressed by changing the
style or position of the element
slightly.
+ :focus
This is applied when an element
has focus. Any element that
you can interact with, such as a
link you can click on or any form
control can have focus.
