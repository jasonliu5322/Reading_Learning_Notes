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
For example, the total width of the box with paddings will be the sum of width plus padding left and padding right.
![Image of Example](https://api.sololearn.com/DownloadFile?id=2999)

Here is another box with margins, border, and paddings.
The total width is the sum of left and right margins, left and right borders, left and right paddings, and the actual width of the content.
![Image of Example](https://api.sololearn.com/DownloadFile?id=3013)

When you set the width and height properties of an element with CSS, you set the width and height of the content area.
When setting a background-color to a box, it covers the content area, as well as the padding.
## 3. JavaScript