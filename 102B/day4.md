# Day 4
## 1. Html
### Ordered Lists
```
An ordered list starts with the <ol> tag, and each list item is defined by the <li> tag.
The list items will be automatically marked with numbers.

<html>
   <head>
      <title>first page</title>
   </head>
   <body>
      <ol>
        <li>Red</li>
        <li>Blue</li>
        <li>Green</li>
      </ol>  
   </body>
</html>
```

### Ordered Lists
```
An unordered list starts with the <ul> tag.The list items will be marked with bullets.

<html>
   <head>
      <title>first page</title>
   </head>        
   <body>
      <ul>
        <li>Red</li>
        <li>Blue</li>
        <li>Green</li>
      </ul>  
   </body>
</html>
```

### Creating a Table
```
Tables are defined by using the <table> tag.
Tables are divided into table rows with the <tr> tag.
Table rows are divided into table columns (table data) with the <td> tag.

Here is an example of a table with one row and three columns:

<table>
   <tr>
      <td></td>
      <td></td>
      <td></td>
   </tr>
</table>

Table data tags <td> act as data containers within the table.
They can contain all sorts of HTML elements, such as text, images, lists, other tables, and so on.
```
### [The border and colspan Attributes](https://www.sololearn.com/Play/HTML)
A table cell can span two or more columns:
```
<table border="2">
   <tr>
      <td>Red</td>
      <td>Blue</td>
      <td>Green</td>
   </tr>
   <tr>
      <td><br /></td>
      <td colspan="2"><br /></td>
   </tr>
</table>
```
The border attribute is not supported in HTML5.
To make a cell span more than one row, use the rowspan attribute.

### The align and bgcolor Attributes
To change your table's position, use the **align** attribute inside your table tag.
Now let's specify a background color of red for a table cell. To do that, just use the bgcolor attribute.
```
<table align="center"> 

<table border="2">
   <tr>
      <td bgcolor="red">Red</td>
      <td>Blue</td>
      <td>Green</td>
   </tr>
   <tr>
      <td>Yellow</td>
      <td colspan="2">Orange</td>
   </tr>
</table>
```
In the case of styling elements, CSS is more effective than HTML.

### Inline and Block Elements
```
In HTML, most elements are defined as block level or inline elements.
Block level elements start from a new line.
For example: <h1>, <form>, <li>, <ol>, <ul>, <p>, <pre>, <table>, <div>, etc.

Inline elements are normally displayed without line breaks.
For example: <b>, <a>, <strong>, <img>, <input>, <em>, <span>, etc.

The <div> element is a block-level element that is often used as a container for other HTML elements.
When used together with some CSS styling, the <div> element can be used to style blocks of content:
<html>
  <body>
    <h1>Headline</h1>
    <div style="background-color:green; color:white; padding:20px;">
      <p>Some paragraph text goes here.</p>
      <p>Another paragraph goes here.</p>
    </div>
  </body>
</html>
```
```
Similarly, the <span> element is an inline element that is often used as a container for some text.
When used together with CSS, the <span> element can be used to style parts of the text:
<html>
  <body>
    <h2>Some 
      <span style="color:red">Important</span>
    Message</h2>
  </body>
</html>
```
```
Summary
The <div> element defines a block-level section in a document.
The <span> element defines an inline section in a document.
```

### Forms
```
HTML forms are used to collect information from the user.
Forms are defined using the <form> element, with its opening and closing tags:
<body>
   <form>…</form>
</body>

Use the action attribute to point to a webpage that will load after the user submits the form.
<form action="http://www.sololearn.com"> 
</form>

Usually the form is submitted to a web page on a web server.
```
### The method and name Attributes
```
The method attribute specifies the HTTP method (GET or POST) to be used when forms are submitted (see below for description):
<form action="url" method="GET">

<form action="url" method="POST">

When you use GET, the form data will be visible in the page address.

Use POST if the form is updating data, or includes sensitive information (passwords).
POST offers better security because the submitted data is not visible in the page address.

To take in user input, you need the corresponding form elements, such as text fields. The <input> element has many variations, depending on the type attribute. It can be a text, password, radio, URL, submit, etc.

The example below shows a form requesting a username and password:
<form>
   <input type="text" name="username" /><br />
   <input type="password" name="password" />
</form>
```
### Form Elements
```
If we change the input type to radio, it allows the user select only one of a number of choices:
<input type="radio" name="gender" value="male" /> Male <br />
<input type="radio" name="gender" value="female" /> Female <br />

The type "checkbox" allows the user to select more than one option:
<input type="checkbox" name="gender" value="1" /> Male <br />
<input type="checkbox" name="gender" value="2" /> Female <br />

The <input> tag has no end tag.
```
```
The submit button submits a form to its action attribute:
<input type="submit" value="Submit" /> 
After the form is submitted, the data should be processed on the server using a programming language, such as PHP.
```

### HTML Colors!
HTML colors are expressed as hexadecimal values.
0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F
As you can see, there are 16 values there, 0 through F. Zero represents the lowest value, and F represents the highest.

### HTML Color Model
Colors are displayed in combinations of ***red, green, and blue light (RGB).***
Hex values are written using the **ashtag symbol (#)**, followed by either three or six hex characters.
RGB color values are supported in all browsers.

### Color Values
All of the possible red, green, and blue combinations potentially number over 16 million.Here are only a few of them: **#FF0000, #00FF00, #777777**.
We can mix the colors to form additional colors:
**Orange and red** mix: #C1250F
Hexadecimal color values are supported in all browsers.

### Background and Font Colors
```
The bgcolor attribute can be used to change the web page's background color.

This example would produce a dark blue background with a white headline:
<html>
   <head> 
      <title>first page</title>  
   </head>
   <body bgcolor="#000099">
       <h1>
        <font color="#FFFFFF"> White headline </font>
       </h1> 
   </body>
</html>

The color attribute specifies the color of the text inside a <font> element.
```

### The <frame> Tag
```
 A page can be divided into frames using a special frame document.

The <frame> tag defines one specific window (frame) within a <frameset>. Each <frame> in a <frameset> can have different attributes, such as border, scrolling, the ability to resize, etc.

The <frameset> element specifies the number of columns or rows in the frameset, as well as what percentage or number of pixels of space each of them occupies.
<frameset cols="100, 25%, *"></frameset>
<frameset rows="100, 25%, *"></frameset>

The <frameset> tag is not supported in HTML5.
```

## 2. CSS
### The text-transform Property
```
The text-transform CSS property specifies how to capitalize an element's text. For example, it can be used to make text appear with each word capitalized.

The HTML:
<p class="capitalize">
    The value capitalize transforms the first 
    character in each word to uppercase; 
    all other characters remain unaffected.
</p>

The CSS:
p.capitalize {
   text-transform: capitalize;
}
```
### text-transform Values
```
Using text-transform property you can make text appear in all-uppercase or all-lowercase. Here is an example:

The HTML:
<p class="uppercase">This value transforms all characters to uppercase.</p>
<p class="lowercase">This value transforms all characters to lowercase.</p>

The CSS:
p.uppercase {
   text-transform: uppercase;
}
p.lowercase {
   text-transform: lowercase;
}
```
### The letter-spacing Property
```
The letter-spacing property specifies the space between characters in a text. The values can be set as:
- normal defines the default style with no extra space between characters
- length defines an extra space between characters using measurement units like px, pt, cm, mm, etc.;
- inherit inherits the property from its parent element;

The HTML:
<p class="normal">This paragraph has no additional letter-spacing applied.</p>
<p class="positive ">This paragraph is letter-spaced at 4px.</p>

The CSS:
p.normal { 
   letter-spacing: normal; 
}
p.positive { 
   letter-spacing: 4px; 
}

For defining an extra space between characters, negative values are also permitted.
Here is an example demonstrating the difference between positive and negative values:

The HTML:
<p class="positive">This paragraph is letter-spaced at 4px.</p>
<p class="negative">This paragraph is letter-spaced at -1.5px</p>

The CSS:
p.positive { 
   letter-spacing: 4px; 
}
p.negative { 
   letter-spacing: -1.5px; 
} 
```
### The word-spacing Property
```
The word-spacing property specifies the space between words in a text. Just like the letter-spacing property, you can set the word-spacing values as normal, length, and inherit.

The HTML:
<p class="normal">This paragraph has no additional word-spacing applied.</p>
<p class="px">This paragraph is word-spaced at 30px.</p>

The CSS:
p.normal { 
   word-spacing: normal;
}
p.px { 
   word-spacing: 30px;
}

Measurement Units

To define an extra space between words, you can use positive measurement values like px, pt, pc, cm, mm, inches, em, and ex.
Negative values are also permitted. Here is an example to show the difference.

The HTML:
<p class="positive">This paragraph is word-spaced at 20px.</p>
<p class="negative">This paragraph is word-spaced at -5px.</p>

The CSS:
p.positive { 
   word-spacing: 20px;
}
p.negative { 
   word-spacing: -5px;
}
```
### The white-space Property
```
The white-space property specifies how white-space inside an element is handled. The values can be set as normal, inherit, nowrap, etc.

The nowrap value makes the text continue on the same line until a <br> tag is encountered, and also collapses all sequences of whitespace into a single whitespace.

The HTML:
<p>
This paragraph has         multiple spaces      and
a line break, but it will be ignored, as we used the nowrap value. 
</p>

The CSS:
p {
   white-space: nowrap;
}
```
### The CSS Box Model
All HTML elements can be considered as boxes. The CSS box model represents the design and layout of the site. It consists of margins, borders, paddings, and the actual content.

The properties work in the same order: top, right, bottom, and left.

**More on Box Models**

Every element of the webpage is a box.
CSS uses the box model to determine how big the boxes are and how to place them.
The box model is also used to calculate the actual width and height of the HTML elements.

**Total Width of an Element**

When working with boxes, it is important to understand how the total width of an element is calculated.
For example, the total width of the box with paddings will be the sum of **width plus padding left and padding right**.
![Image of Example](https://api.sololearn.com/DownloadFile?id=2999)

Here is another box with margins, border, and paddings.
The total width is the sum of **left and right margins, left and right borders, left and right paddings, and the actual width of the content**.
![Image of Example](https://api.sololearn.com/DownloadFile?id=3013)

When you set the width and height properties of an element with CSS, you set the width and height of the content area.
When setting a background-color to a box, it covers the content area, as well as the padding.

### The border Property

The CSS border property allows you to customize the borders of HTML elements.
In order to add a border to the element, you need to specify the **size, style, and color** of the border.
The example below shows how to add a solid green border to the paragraph.
```
The HTML:
<p>This is an example of a solid border.</p>

The CSS:
p {
   padding: 10px;    
   border: 5px solid green;
}
```
**Border Width**
```
The properties for the border can be set separately. The border-width property specifies the width of the border.

The HTML:
<p class="first">
    Border width of this paragraph is set to 2px.
</p>
<p class="second">
    Border width of this paragraph is set to 5px.
</p>

The CSS:
p.first {
   padding: 10px;    
   border-style: solid;
   border-width: 2px;
}
p.second {
   padding: 10px;    
   border-style: solid;
   border-width: 5px;
}
```

**Border Color**
```
The border color of the element can be defined using a color name, RGB, or Hex values.
The HTML:
<p class="first">
   Border color has been created using <strong>color name.</strong>
</p>
<p class="second">
   Border color has been created using <strong>Hex values.</strong> 
</p>
<p class="third">
   Border color has been created using <strong>RGB values.</strong> 
</p>

The CSS:
p.first {
   padding: 10px;
   border-style: solid;
   border-width: 2px;
   border-color: blue;
}
p.second {
   padding: 10px;    
   border-style: solid;
   border-width: 2px;
   border-color: #FF6600;
} 
p.third {
   padding: 10px;    
   border-style: solid;
   border-width: 2px;
   border-color: rgb(0, 153, 0);
} 

None of the border properties will have any effect unless the border-style property is set.
```
### The border-style Property

The default value of border-style is none, which defines no border.
There are various styles supported for the border-style property: **dotted, dashed, double,** etc. The example below illustrates the differences between them.
```
The HTML:
<p class="none">This paragraph has no border.</p>
<p class="dotted">This is a dotted border.</p>
<p class="dashed">This is a dashed border.</p>
<p class="double">This is a double border.</p>
<p class="groove">This is a grooved border.</p>
<p class="ridge">This is a ridged border.</p>
<p class="inset">This is an inset border.</p>
<p class="outset">This is an outset border.</p>
<p class="hidden">This is a hidden border.</p>

The CSS:
p.none {border-style: none;}
p.dotted {border-style: dotted;}
p.dashed {border-style: dashed;}
p.double {border-style: double;}
p.groove {border-style: groove;}
p.ridge {border-style: ridge;}
p.inset {border-style: inset;}
p.outset {border-style: outset;}
p.hidden {border-style: hidden;}
```
![image of example](https://api.sololearn.com/DownloadFile?id=2620)

In CSS, it is possible to specify different borders for different sides, using the following properties: **border-top-style, border-right-style, border-bottom-style, and border-left-style for the corresponding sides.**

### CSS Width and Height
```
To style a <div> element to have a total width and height of 100px:

The HTML:
<div>The total width and height of this element is 100px.</div>

The CSS:
div {
   border: 5px solid green;    
   width: 90px;
   height: 90px;
}
The total width and height of the box will be the 90px+5px (border)+5px(border) = 100px;
```
![image of example](https://api.sololearn.com/DownloadFile?id=2621)

### Width and Height Measurement
The width and height of an element can be also assigned using **percents**.
In the example below the width of an element is assigned in percentages, the height is in pixels.
```
The HTML:
<div>The total width of this element is <strong>100%</strong> and the total height is <strong>100px</strong> .</div>

The CSS:
div {
   border: 5px solid green;    
   width: 100%;
   height: 90px;
}
```
### The background-color Property
```
The background-color property is used to specify the background color of an element.

The HTML:
<p>The background color of this page is set to LightSkyBlue.</p>

The CSS:
body {
    background-color: #87CEFA;
}
```
```
The Background Color Values

The color of the background can be defined using three different formats: a color name, hexadecimal values, and RGB.

In the example below, the body, h1, and p elements are assigned different background colors:

The HTML:
<h1>This is a heading</h1>
<p>This is a paragraph</p>

The CSS:
body {
   background-color: #C0C0C0;
}
h1 {
   background-color: rgb(135,206,235);
}
p {
   background-color: LightGreen;
}
```
![image of examle](https://api.sololearn.com/DownloadFile?id=2625)

### The background-image Property
```
The background-image property sets one or several background images in an element. Let's set a background-image for the <body> element.

The CSS:
body {
   background-image: url("http://www.sololearn.com/uploads/css_logo.png");
   background-color: #e9e9e9;
}
The url specifies the path to the image file. Both relative and absolute paths are supported.
```
![image of example](https://api.sololearn.com/DownloadFile?id=2626)
By default, a background-image is placed at the top-left corner of an element, and is repeated both vertically and horizontally to cover the entire element.
```
Background-image can be set not only for the whole page, but for individual elements, as well.
Below we set a background image for the <p> element.
```
```
The HTML:
<p>This paragraph has a background image.</p>

The CSS:
p {
   padding: 30px;
   background-image: url("green_photo.jpg");
   color: white;   
}
```
![image of example](https://api.sololearn.com/DownloadFile?id=2627)
To specify more than one image, just separate the URLs with commas.
### The background-repeat Property

The background repeat property specifies how background images are repeated. A background image can be repeated along the horizontal axis, the vertical axis, both axes, or not repeated at all.

The repeat-x will repeat a background image only horizontally.
The CSS:
```
body {
   background-image: url("css_logo.png");
   background-repeat: repeat-x;  
}
```
If you want the image to be shown only once, use the **no-repeat** value.

### Setting the Value to Inherit

When you set the background-repeat property to inherit, it will take the same specified value as the property for the element's parent.

For example, we set the body background repeat only horizontally. If we set some paragraph background-repeat values to be inherited, they will take the same property value as the body element.
```
The CSS:
body {
   background-image: url("css_logo.png");
   background-repeat: repeat-x;
}
p {
   background-image: url("css_logo.png");
   background-repeat: inherit;
   margin-top: 100px;
   padding: 40px;
}
```
### The background-attachment Property

The background-attachment property sets whether a background image is fixed or scrolls with the rest of the page.
Even if an element has a scrolling mechanism, a "fixed" background doesn't move with the element.
```
The CSS:
body {
   background-image: url("css_logo.png");
   background-repeat: no-repeat;
   background-attachment: fixed;
}
```
### The background-attachment Values

You can also set the background-attachment to **inherit or scroll.**
When you set the background-attachment to inherit, it will inherit the value from its parent element.

When you set the background-attachment to scroll, the background image will scroll with the rest of the content.
```
The CSS:
body {
   background-image: url("css_logo.png");
   background-repeat: no-repeat;
   background-attachment: scroll;
}
```
### The list-style-type Property
```
The CSS list properties allow us to set different list item markers. In HTML, there are two types of lists:
unordered lists (<ul>) - the list items are marked with bullets
ordered lists (<ol>) - the list items are marked with numbers or letters
With CSS, lists can be styled further, and images can be used as the list item marker.
One of the ways is to use the list-style-type property, which can be set to circle, square, decimal, disc, lower-alpha, etc.

The HTML:
<ol class="lower-alpha">
   <li>Red</li>
   <li>Green</li>
   <li>Blue</li>
</ol>
<ul class="circle">
   <li>Red</li>
   <li>Green</li>
   <li>Blue</li>
</ul>
<ul class="square">
   <li>Red</li>
   <li>Green</li>
   <li>Blue</li>
</ul>

The CSS:
ol.lower-alpha {
   list-style-type: lower-alpha;
}
ul.circle {
   list-style-type: circle;
}
ul.square {
   list-style-type: square;
}
```
![image of example](https://api.sololearn.com/DownloadFile?id=2634)

### The List Image and Position

There are also other list properties, such as:
list-style-image - specifies an image to be used as the list item marker.
list-style-position - specifies the position of the marker box (inside, outside).

In the example below, we use an image as the list item marker, and specify the position to be inside of the content flow.
```
The HTML:
<p>The following list has list-style-position: <strong>inside</strong>.</p>
<ul>
   <li>Red</li>
   <li>Green</li>
   <li>Blue</li>
</ul>

The CSS:
ul {
   list-style-image: url("logo.jpg");
   list-style-position: inside;
}
```
"list-style-position: outside" is the default value.

### The list-style Property

The list-style property is a shorthand property for setting list-style-type, list-style-image and list-style-position. It is used to set all of the list properties in one declaration:
ul {
   list-style: square outside none;
}
```
This would be the same as the longhand version.
ul {
   list-style-type: square;
   list-style-position: outside;
   list-style-image: none;
}
```
### The Table Properties

The look of an HTML table can be greatly improved with CSS.

The border-collapse property specifies whether the table borders are collapsed into a single border or separated as default. If the borders are separate, the border-spacing property can be used to change the spacing.
```
The HTML:
<table border="1">
   <tr>
     <td>Red</td>
     <td>Green</td>
   </tr>
   <tr>
      <td>Blue</td>
      <td>Yellow</td>
   </tr>
</table>

The CSS:
table {
   border-collapse: separate;
   border-spacing: 20px 40px;
}
```
### The caption-side Property
```
The caption-side property specifies the position of a table caption. The values can be set as top or bottom.
In the example below, we specify the placement of a table caption to top.

The HTML:
<table border="1">
<caption>Some of Our Courses</caption>
<tr>
  <th>Course name</th>
  <th>Lessons</th>
  <th>Quizzes</th>
</tr>
<tr>
  <td>C++</td>
  <td>81</td>
  <td>363</td>
</tr>
<tr>
  <td>JavaScript</td>
  <td>48</td>
  <td>144</td>
</tr>
<tr>
  <td>HTML</td>
  <td>38</td>
  <td>119</td>
</tr>
<tr>
  <td>CSS</td>
  <td>70</td>
  <td>174</td>
</tr>
</table>

The CSS:
caption {
   caption-side: top;
}
```
### The empty-cells Property
```
The empty-cells property specifies whether or not to display borders and background on empty cells in a table.
Possible values are:
show: the borders of an empty cell are rendered
hide: the borders of an empty cell are not drawn

Here is the empty-cells property that is used to hide borders of empty cells in the <table> element.

The HTML:
<table border="1">
  <tr>
    <td>HTML</td>
    <td>CSS</td>
  </tr>
  <tr>
    <td>JavaScript</td>
    <td></td>
  </tr>
</table>

The CSS:
table {
   border-collapse: separate;
   empty-cells: hide;
}
```
### The table-layout Property

The table-layout specifies how the width of table columns is calculated. The possible values are:
auto - when column or cell width are not explicitly set, the column width will be in proportion to the amount of content in the cells that make up the column
fixed - when column or cell width are not explicitly set, the column width will not be affected by the amount of content in the cells that make up the column.

The table layout is set to auto by default.
The example below shows the difference between auto and fixed.
```
The HTML:
<p>Table-layout is set to <strong>auto</strong></p>
<table class="auto">
  <tr>
    <td width=“10%">500.000.000.000.000</td>
    <td width="90%">20.000</td>
  </tr>
</table>

<p>Table-layout is set to <strong>fixed</strong></p>
<table class="fixed">
  <tr>
    <td width="10%">500.000.000.000.000</td>
    <td width="90%">20.000</td>
  </tr>
</table>

The CSS:
table {
   border-collapse: separate;
   width: 100%;
   border: 1px solid gray;
} 
td {
   border: 1px solid gray;
}
table.auto {
   table-layout: auto;
}
table.fixed {
   table-layout: fixed;
}
```
![image of example](https://api.sololearn.com/DownloadFile?id=2640)

### Setting Styles to Links

Links can be styled with any CSS property (e.g., color, font-family, background, etc.).
In addition, links can be styled differently, depending on what state they are in. The following pseudo selectors are available:
a:link - defines the style for normal unvisited links
a:visited - defines the style for visited links
a:active - a link becomes active once you click on it
a:hover - a link is hovered when the mouse is over it

The example below creates a link that will change the style when the mouse is moved over it.
```
The HTML:
<p><a href="http://www.sololearn.com" target="_blank">
   This link is hovered when we mouse over it
</a></p>

The CSS:
a:hover {
   color: red;
}

Links' Text Decoration

By default, text links are underlined by the browser.
One of the most common uses of CSS with links is to remove the underline. In the example below, the text-decoration property is used to remove the underline.

The HTML:
<p><a href="http://www.sololearn.com" target="_blank">
   This link has no underline.
</a></p>

The CSS:
a:link {
   text-decoration: none;
}
The following properties are used to control the look and feel of links:
border:none - removes border from images with links
outline:none - removes the dotted border on clicked lines in IE
```
### Setting the Mouse Cursor Style

CSS allows you to set your desired cursor style when you mouse over an element. For example, you can change your cursor into a hand icon, help icon, and much more, rather than using the default pointer.
```
In the example below, the mouse pointer is set to a help icon when we mouse over the span element:
<span style="cursor:help;">
   Do you need help?
</span>

The cursor Property Values

There are numerous other possible values for the cursor property, such as:
default - default cursor
crosshair - cursor displays as crosshair
pointer - cursor displays hand icon
The list of possible values is quite long. The image below demonstrates the various available styles:
```
![image of example](https://api.sololearn.com/DownloadFile?id=2983)

### display: block
```
Every element on a web page is a rectangular box.The display property determines how that rectangular box behaves. A block element is an element that takes up the fullest width available, with line breaks before and after.
The style rules in the following example display the inline <span> elements as block-level elements:

The HTML:
<span>First paragraph.</span>
<span>Second paragraph.</span>
<span>Third paragraph.</span>
<span>Fourth paragraph.</span>
<span>Fifth paragraph.</span>

The CSS:
span {
   display: block;
}
```
### display: inline

An inline element only takes up as much width as necessary, and does not force line breaks.
The CSS:
p {
   display: inline;
}
### display:none
```
display:none hides an element, so it does not take up any space. The element will be hidden, and the page will be displayed as if the element is not there.

The HTML:
<h1>This text will not display, as we set the value to none.</h1>
<p>Headline of this paragraph is not displayed, as we set the value to none.</p>

The CSS:
h1 {
   display: none;
}
```
### The visibility Property

The visibility property specifies whether an element is visible or hidden. The most common values are visible and hidden.

Hiding an element can be done by setting the display property to "none" or the visibility property to "hidden". However, notice that these two methods produce different results:
visibility:hidden hides an element, but it will still take up the same space as before. The element will be hidden, but it will still affect the layout:

### Positioning Elements

The CSS positioning properties allow you to position an element. It can also place an element behind another, and specify what should happen when an element's content is too big.

Elements can be positioned using the top, bottom, left, and right properties. However, these properties will not work unless the position property is set first. They also work differently depending on the positioning method.

Static Positioning
HTML elements are positioned static by default. A static positioned element is always positioned according to the normal flow of the page.
```
The HTML:
<p>Paragraph with no position.</p>
<p>Paragraph with no position.</p>
<p>Paragraph with no position.</p>
<p>Paragraph with no position.</p>
<p>Paragraph with no position.</p>
<p class="position_static">This paragraph has a static position.</p>

The CSS:
p.position_static {
   position:static;
   top: 30px;
   right: 5px;
   color: red;
}
```
### Fixed Positioning

An element with a fixed position is positioned relative to the browser window, and will not move even if the window is scrolled.
The position can be specified using one or more of the properties top, right, bottom, and left.
In the example below, the paragraph is fixed to 30px from the top and 5px from the right.

The CSS:
p.position_fixed {
   position: fixed;
   top: 30px;
   right: 5px;
   color: red;
}
### Fixed Positioning

An element with a fixed position is positioned relative to the browser window, and will not move even if the window is scrolled.
The position can be specified using one or more of the properties top, right, bottom, and left.
In the example below, the paragraph is fixed to 30px from the top and 5px from the right.

The CSS:
p.position_fixed {
   position: fixed;
   top: 30px;
   right: 5px;
   color: red;
}

### Relative Positioning

A relative positioned element is positioned relative to its normal position.
The properties top, right, bottom, and left can be used to specify how the rendered box will be shifted.

The CSS:
p {
   width: 350px;
   border: 1px black solid;
   position: fixed;
}
span {
   background: green;
   color:white;
   position: relative;
   top: 150px;
   left: 50px;
}
The content of relatively positioned elements can be moved and overlap other elements, but the reserved space for the element is still preserved in the normal flow.
This value cannot be used for table cells, columns, column groups, rows, row groups, or captions.

### Absolute Positioning
```
An absolute position element is positioned relative to the first parent element that has a position other than static. If no such element is found, the containing block is <html>.

Absolutely positioned elements are removed from the normal flow. The document and other elements behave like the absolutely positioned element does not exist.
Absolutely positioned elements can overlap other elements.
```
### Floating

With CSS float, an element can be pushed to the left or right, allowing other elements to wrap around it.
Float is often used with images, but it is also useful when working with layouts.
The values for the float property are left, right, and none.
Left and right float elements in those directions, respectively. none (the default) ensures that the element will not float.
Below is an example of an image that is floated to the right.
```
The HTML:
<p><img src="css_logo.png" />
This paragraph has an image that is floated to the <strong>right.</strong> 
It is highly recommended to add a margin to images so that the text does 
not get too close to the image. If you want your text to be easily read, you 
should always add a few pixels between words and borders, images, 
and other content. 
</p>

The CSS:
img {
   float: right;
}
```
### Elements Next to Each Other

If you place several floating elements one after the other, they will float next to each other if there is enough room.
As an example, in a print layout, images may be set into the page such that text wraps around them as needed.
```
The CSS:
img {
   float: left;
   width: 120px;
   margin-right: 10px;
}
p {
   width: 120px;   
   float: left;
}
```
1[image of example](https://api.sololearn.com/DownloadFile?id=2656)

### Clearing the Float

Elements that come after the floating element will flow around it. To avoid this, use the clear property.
The clear property specifies the sides of an element where other floating elements are not allowed to be.

In the example below, if we set the float property to the div, only the paragraph that comes after the div will be wrapped around the image.
```
The HTML:
This paragraph is above the div element 
and is not affected by the float right property. 
<br /><br />
<div class="floating">
   <img src="css_logo.png" />
</div>
This paragraph comes after the div element 
and is affected by the float right property. 
<br /><br />
This paragraph also comes after the div element
and is affected by the float right property.
<br /> <br />

The CSS:
.floating {
   float: right;
}
```
![image of example](https://api.sololearn.com/DownloadFile?id=2657)

### Clearing Floats
```
both is used to clear floats coming from either direction.

The HTML:
This paragraph is above the div element 
and is not affected by the float right property. 
<br/><br/>
<div class="floating">
   <img src="css_logo.png" />
</div>
This paragraph comes after the div element 
and is affected by the float right property. 
<br/><br class="clearing"/>
This paragraph is out of the floating group 
and is not affected by the float right property.
<br/> <br/>

The CSS:
.floating {
   float: right;
}
.clearing {    
   clear: both;
}
```

### The overflow Property

As discussed earlier, every element on the page is a box. If the height of the box is not set, the height of that box will grow as large as necessary to accommodate the content.
```
The HTML:
<div>
This text is inside the div element, which has a blue 
background color and is floated to the left. We set a specific 
height and width for the div element, and as you can see, 
the content cannot fit. 
</div>

The CSS:
div {
  width: 150px;
  height: 150px;
  background-color: LightBlue;
  float: left;
}
```
![image of example](https://api.sololearn.com/DownloadFile?id=2659)
The CSS overflow property specifies the behavior that occurs when an element's content overflows the element's box.

### The overflow Property Values

There are four values for the overflow property: visible (the default value), scroll, hidden, and auto.

The value scroll results in clipped overflow, but a scrollbar is added, so the rest of the content may be seen.
```
The CSS:
div {
   width: 150px;
   height: 150px;
   background-color: LightBlue;
   float: left;
   overflow: scroll;
}
```
![image of example](https://api.sololearn.com/DownloadFile?id=2660)

### The z-index Property

When elements are positioned outside the normal flow, they can overlap other elements.
The z-index property specifies the stack order of an element (which element should be placed in front of, or behind, the others).
```
The CSS:
.blue { 
   background-color: #8EC4D0;
   margin-bottom: 15px;
   width: 120px;
   height: 120px;
   color: #FFF;
}
.red {
   background-color: #FF4D4D;
   position: relative;
   width: 120px;
   height: 120px;
   color: #FFF;
   margin-top: -50px;
   margin-left: 50px;
}
```
![image of example](https://api.sololearn.com/DownloadFile?id=2662)
The red box overlaps the blue box, because it was placed later in the HTML markup.
The z-index property can change this order.

### Assigning the z-index Property

Assigning a higher z-index value to the blue div and a lower z-index value to the red div will result in the following:
```
The CSS:
.blue {
   z-index: 3; 
   position: relative;
}
.red {
   z-index: 2;
   position: relative;
}
```
![image of example](https://api.sololearn.com/DownloadFile?id=2663)
The z-index works only on positioned elements (position:absolute, position:relative, or position:fixed).

### CSS3
CSS3 is the latest standard for CSS.
CSS3 is completely backwards-compatible with earlier CSS versions.

Some of the most significant new features are:
Border radius - allows us to create rounded corners for elements.
Border images - allows us to specify an image as the border around an element.
Multiple backgrounds - applies multiple backgrounds to elements.
Animations and effects, and much more!

To make web development easier and faster, CSS3 introduces additional new features, including the following:

Box Shadow
With the box-shadow property, you can attach one or more shadows to an element by specifying values for color, size, blur, and offset.

Gradients
CSS3 gradients allow us to set the background color of the element to a gradient. Two types of gradients are available: Linear and Radial.

CSS Vendor Prefixes

CSS vendor prefixes or CSS browser prefixes are a way for browser makers to add support for new CSS features during periods of testing and experimentation. Browser prefixes are used to add new features that may not be part of the final and formal CSS specification.

For example, the prefix for Safari and Chrome is -webkit. The border-radius property is currently supported in Chrome, Safari, and Mozilla, as long as it is accompanied by the browser prefix.
To specify the border-radius in Chrome and Safari, the following syntax is used:
-webkit-border-radius: 24px;

The prefix is added to the property to make it work in the unsupported browsers. So, you might end up with multiple definitions of the same property, each with the specific browser prefix.
While most browsers today will work without prefixes, it is essential to know these for backwards capability and understanding older codes.

Browser Prefixes
Here is the list of vendor prefixes for each browser:
![image of example](https://api.sololearn.com/DownloadFile?id=2665)
It might feel annoying and repetitive to have to write the properties two to five times to get them to work in all browsers, but it's temporary. As browsers improve, they add support for the standards based version of the properties, and you can remove the prefixed versions.

### The border-radius Property
With CSS3, you can give any element "rounded corners" by using the border-radius property.
```
The CSS:
border-radius: 20px;
background-color: green;
color: white;
```
![image](https://api.sololearn.com/DownloadFile?id=2666)

```Specific border radius values can be applied for the border-radius property in the following order: top-left, top-right, bottom-right, bottom-left.
border-radius: 0 0 20px 20px;

The value of border-radius can also be specified in percentages.
```
![image](https://api.sololearn.com/DownloadFile?id=2667)

### Creating a Circle

A rectangle can be turned into a circle using only CSS.
To create a circle, the border radius should be half of the height and the width.

The rectangle in the example below has a width and height of 200px. By setting the border radius to 100px, the corners will be rounded to form a circle:
```
div {
   width: 200px;
   height: 200px;
   border-radius: 100px;
   background-color: green;
   color: white;
}
```
### The box-shadow Property

The CSS3 box-shadow property applies shadow to elements.
Components of the box-shadow property are decoded by browsers in the following manner:
- **The first length for the horizontal offset will cast the shadow to the right of the box (required)**
- **The second length is for the vertical offset that will cast the shadow to below the box (required)**
- **The color of the shadow (optional)**
```
In the example below, the horizontal and vertical offsets have been set to 10px:
div {
   width: 300px;
   height: 100px;
   background-color: #9ACD32;
   box-shadow: 10px 10px #888888;
}
```
### Blur and Spread

Besides color, there are also two optional values for the box-shadow element, which are blur and spread.
The blur and spread values should be used before the color value.

box-shadow: 10px 10px 5px 5px #888888;

### Negative Values

Negative values can also be used for the box-shadow property.

horizontal offset - the shadow will be to the left of the box
vertical offset - the shadow will be above the box
blur radius - negative values are not allowed
spread radius - negative values will cause the shadow to shrink

For example:
box-shadow: -10px -10px 5px -5px #888888;

### Creating an Inner Shadow

The "inset" keyword allows to draw an inner shadow in the box. To show an inset shadow, just add the inset keyword:
box-shadow: inset 10px 10px 5px #888888;
![image](https://api.sololearn.com/DownloadFile?id=2672)
You can simultaneously create inner and outer shadows by separating each shadow with a comma.

### Layering Multiple Shadows

You can define as many shadows for the same box as you want by writing all of them comma-separated in the same rule.

In the example below, two inner shadows have been created by separating each shadow with a comma.
box-shadow: 
inset 10px 10px 5px #888888, 
inset -10px -10px 5px #888888;
![image](https://api.sololearn.com/DownloadFile?id=2673)

In case we specify more than one value, the one which comes last will be positioned at the back of all shadows.
Here is an example:
box-shadow: 0 0 10px 4px #FF6347, 
0 0 10px 30px #FFDAB9, 
30px 0 20px 30px #B0E0E6;
![image](https://api.sololearn.com/DownloadFile?id=2674)
As expected, the blue shadow (#B0E0E6) comes last.

### Transparency Effect

Before CSS3, transparent background images were used to create transparency effects. The new features of CSS3 now make it easier to create transparency effects.

CSS supports color names, hexadecimal, and RGB colors.
In addition, CSS3 introduces the following:

RGBA Colors
RGBA color values are an extension of RGB color values with an alpha channel, which specifies the opacity for a color.
An RGBA color value is specified with: rgba(red, green, blue, alpha). The alpha parameter is a number between 0.0 (fully transparent) and 1.0 (fully opaque).

HSL (Hue, Saturation, Lightness) Colors
An HSL color value is specified with: hsl(hue, saturation, lightness).
Hue is a degree on the color wheel ranging from 0 to 360
0 (or 360) is red, 120 is green, 240 is blue.
Saturation is a percentage value: 100% is the full color.
Lightness is also a percentage; 0% is dark (black) and 100% is white. HSLA color values are an extension of HSL color values with an alpha channel - which specifies the opacity for a color (just like RGBA).

In the example below, a transparent glass menu bar is created with CSS3.
```
In the HTML file, a <nav> tag containing an <ul> list with links has been added:
<nav>
   <ul>
       <li><a href="#">COURSES</a></li>
       <li><a href="#">DISCUSS</a></li>
       <li><a href="#">TOP LEARNERS</a></li>
       <li><a href="#">BLOG</a></li>
   </ul>
</nav>
```
A number of CSS3 features are used to create the effects:
body {
   background:url("bg.jpg");
}
nav {
   padding: 50px 0;
   min-width: 500px; 
}
nav ul {
   background: linear-gradient(90deg, 
     rgba(255, 255, 255, 0) 0%, 
     rgba(255, 255, 255, 0.2) 25%, 
     rgba(255, 255, 255, 0.2) 75%, 
     rgba(255, 255, 255, 0) 100%);
   box-shadow: 0 0 25px rgba(0, 0, 0, 0.1),
     inset 0 0 1px rgba(255, 255, 255, 0.6);
}
nav ul li {
   display: inline-block;
}
nav ul li a {
   padding: 10px; 
   color: #FFFFFF;
   font-size: 18px;
   font-family: Arial;
   text-decoration: none;
   display: block;
 }

 ### The text-shadow Property

The text-shadow property defines one or more comma-separated shadow effects, to be applied to the text content of the current element.

The image below shows how the text-shadow property is applied:
![image](https://api.sololearn.com/DownloadFile?id=2676)
- The offset-x and offset-y values are required for the CSS text-shadow property.
- The color value is not required, but since the default for the text-shadow is transparent, the text-shadow will not appear unless you specify a color value.

### Multiple Text Shadows

The text-shadow style can accept multiple values in a comma-separated list.
According to CSS2, the shadows are laid down in the order they appear, so if they overlap, the last one that is specified should appear on top. CSS3 has now changed that so they are applied in reverse order.

To create multiple shadows, the shadows are separated with a comma. Here is an example:
h1 {
   text-shadow: 5px 10px 2px #93968f, 
      -3px 6px 5px #58d1e3;
}
To make a text shadow look realistic, remember these few shadow characteristics:

- A shadow which is close to the text is normally not as blurred as a shadow that is far from the text. A shadow that is far from the text usually implies a light source which is also far from the text. 
- A shadow which is close to the text usually implies that the underlying surface is close, that the light is close, or both. A close shadow is often darker than a distant shadow, because less light can get in between the shape and the underlying surface.
To remove a text-shadow, set the text-shadow property to none; no shadows will be associated with that element.

### Working with Pseudo-Classes

The CSS pseudo-classes allow us to style elements, or parts of elements, that exist in the document tree without using JavaScript or any other scripts. A pseudo-class starts with a ":" (colon).
The most commonly used pseudo-classes are :first-child and :last-child.

The :first-child pseudo-class matches an element that is the first child element of some other element.
In the following example, the selector matches any <p> element that is the first child of the div element:
```
The HTML:
<div id="parent">
   <p>First paragraph</p>
   <p>Second paragraph</p>
   <p>Third paragraph</p>
   <p>Fourth paragraph</p>
</div>
```
The CSS:
#parent p:first-child {
   color: green;
   text-decoration: underline;   
}

The :last-child pseudo-class matches an element that is the last child element of some other element.

In the example below, the selector will match any <p> element that is the last child of the div element:
#parent p:last-child {
   color: green;
   text-decoration: underline;   
}

### Working with Pseudo Elements

Pseudo elements are used to select specific parts of an element.
There are five pseudo elements in CSS, each starting with a double colon (::):

::first-line - the first line of the text in a selector
::first-letter - the first letter of the text in a selector
::selection - selects the portion of an element that is selected by a user
::before - inserts some content before an element
::after - inserts some content after an element

In the example below, the ::first-line pseudo element is used to style the first line of our text:
p::first-line {
   color: #589432;
}

The ::selection pseudo element styles the selected text:
p::-moz-selection {
   background: #8bc34a;
   color: #fff;
}
The -moz- prefix is used, as the ::selection element is not supported by Mozilla yet.

### Working with Pseudo Elements

Using ::before and ::after pseudo elements allows us to add a wide variety of content to the page.
```
In the example below, the ::before pseudo element is used to add an image before the list.
The HTML:
<p>You can insert text, images, and other resources using <strong>:before </strong>pseudo element.</p>
<p>You can insert text, images, and other resources using <strong>:before </strong>pseudo element.</p>
<p>You can insert text, images, and other resources using <strong>:before </strong>pseudo element.</p>

The CSS:
p::before {
   content: url("logo.jpg");
}
```
Note the content keyword in the syntax.
![image](https://api.sololearn.com/DownloadFile?id=2682)
If you change the ::before element to ::after in the example above, the images will appear at the end of the list.

### The word-wrap Property

The word-wrap property allows long words to be broken and wrapped into the next line. It takes two values: normal and break-word.

In the example below, the word-wrap property is set to normal.
The CSS:
p {
   width: 210px; 
   height: 100px;
   border: 1px solid #000000;
   word-wrap: normal;
}

![image](https://api.sololearn.com/DownloadFile?id=2683)

Now let's see what happens when we use this same example and set the word-wrap property to break-word:
p {
   width: 210px; 
   height: 100px;
   border: 1px solid #000000;
   word-wrap: break-word;
}

![image](https://api.sololearn.com/DownloadFile?id=2684)

When the word-wrap property is set to break-word, the browser breaks a word when it is too long to fit within its container.

## 3. JavaScript