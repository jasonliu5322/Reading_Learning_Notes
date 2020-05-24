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

### Types of Elements
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

## 2. CSS
## 3. JavaScript