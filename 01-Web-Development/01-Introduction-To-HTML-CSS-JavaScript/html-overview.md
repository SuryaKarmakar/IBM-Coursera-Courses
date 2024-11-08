## HTML:

HTML stands for Hypertext Markup Language, a markup language that enables documents to be displayed as web pages on the Internet. It is a markup language that was originally designed for sharing scientific documents.

## HTML5:

The HTML5 specification defines a single language called HTML5 that can be written in HTML or XML syntax. The HTML5 specification defines a processing model that can interoperate with earlier HTML implementations. HTML5 improves the markup for documents. HTML5 includes markup and APIs for idioms, such as web storage, video, and audio content.

## HTML Features:

1. It provides the means to categorize web pages into different sections, and includes tools for effective data management, drawing, video, and audio.
2. Facilitates the development of cross-browser applications for the web and portable devices.
3. Allows greater flexibility, permitting the development of exciting and interactive websites.
4. Helps to create a more engaging user experience.
5. Pages that are designed by using HTML5 can provide an experience similar to desktop applications.
6. Allows for enhanced, multiple-platform development by combining the capability of an application programming interface (API).
7. By using HTML5, developers can create a modern application experience that is uniform across platforms and devices.

```html
<html>
  <head>
    <title>Sampe Page</title>
  </head>
  <body>
    <h1>Hello World!</h1>
  </body>
</html>
```

1. The html tag is the root element of this tree.
2. This example, contains two elements: head and body.
3. The head element can contain the following tags: title, scripts, style, style sheet links, meta information, browser support information and other initialization functions.
4. The body tag contains all content that is displayed on the webpage.

## DOM Tree:

A DOM tree is an in-memory representation of a document. DOM trees contain several kinds of nodes, which include a DOCTYPE node, elements such
as headers and paragraphs, text nodes, and comment nodes.

## XHTML:

```xml
<?xml version="1.0" encoding= "UTF-8"?>
<html xmlns="https://www.w3.org/1999/xhtml">
  <head>
    <meta
      http-equiv="Content-Type"
      content="application/xhtml+ml; charset=ISO-8859-1"
    />
    <title>Example document</title>
  </head>
  <body>
    <p>Example paragraph</p>
  </body>
</html>
```

1. Extensible Markup Language (XML) documents look similar to HTML documents, except they have an XML tag on the first line.
2. In addition, with XML documents, the Content-type must be specified as an XML media type such as application or xml.
3. When a document is transmitted with an XML content type, it is treated as an XML document by a web browser and an XML processor parses the document.

## HTML vs XHTML:

1. Both HTML and XHTML use the same semantic or tags. However, XHTML tags all need to be in lowercase, while the case used does not matter in HTML.
2. In addition, XHTML must be well-formed. Every element must have an end tag. All attributes must have a value and double or single quotation marks must surround all attribute values. If an XML parser encounters a situation where the syntax is not well-formed, it stops processing. In HTML, different case, unmatched quotation marks, and non-terminated and uncontained elements are allowed and commonplace. In this regard, HTML syntax is less rigorous than XHTML syntax.

## HTML Scripting:

The use of scripting within a website, often through the use of JavaScript, can be done directly within your HTML code within the `script` tag, or within a separate file which is called in your HTML code. Scripting provides a more interactive user experience when browsing websites. It can be used for various tasks, such as form validation, dynamically changing the content of a website, and manipulating images.

Each HTML document that is loaded into a browser page becomes a Document object. The Document object provides access to all HTML elements in a page and can be accessed from within a script

```html
<html>
  <head>
    <script type="text/javascript">
      function textChecker() {
        var textField1 = document.getElementById("textField1");
        if (textField1.value == "") {
          alert("Please type in the field");
        } else {
          alert("You entered: " + textField1.value);
        }
      }
    </script>
  </head>
  <body>
    <input type="text" id="textField1" />
    <input type="button" onClick="textChecker ()" value="Submit" />
  </body>
</html>
```

1. The document.getElementById(‘textField1’) retrieves the contents of what was typed into the input field that has the id of textField1 and places this content into a variable.
2. The JavaScript logic then tests whether any data was typed into the field, and an alert dialog is displayed with the result.

## HTML5 Overview:

1. DOCTYPE tag:

All HTML documents must start with this declaration. It tells the browser what document type to expect. Note that this element has no ending tag.

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- Metadata Here -->
  </head>
  <body>
    <!-- Document Body Here -->
  </body>
</html>
```

2. html tag:

The root element of an HTML document. All other tags in the document should be contained in this tag.

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- Metadata Here -->
  </head>
  <body>
    <!-- Document Body Here -->
  </body>
</html>
```

3. head tag:

Contains metadata and should be placed after the \<html\> tag and before the \<body\> tag.

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- Metadata Here -->
  </head>
  <body>
    <!-- Document Body Here -->
  </body>
</html>
```

4. title tag:

Defines the title of the HTML document displayed in the browser’s title bar and tabs. It is required in all HTML documents. It should be contained in the \<head\> tag.

```html
<!DOCTYPE html>
<html>
  <head>
    <title>Document Title</title>
  </head>
</html>
```

5. meta tag:

Used to provide metadata about the HTML document.

```html
<head>
  <meta name="author" content="Christopher" Moore />
</head>
```

6. script tag:

Used to embed JavaScript in an HTML document.

```html
<script>
  alert(“Hello World”);
</script>
```

7. link tag:

Used to link an external document, such as a CSS file, to an HTML document.

```html
<head>
  <link rel="stylesheet" href="styles.css" />
</head>
```

8. body tag:

Contains the contents of the HTML document. It should contain all other tags besides the \<head\> element to display the body of the document.

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- Metadata Here -->
  </head>
  <body>
    <!-- Document Body Here -->
  </body>
</html>
```

9. div tag:

Often used to separate sections in the body of a document in order to style that content with CSS.

```html
<div>
  This element has no particular semantic meaning but is often used in
  conjunction with CSS for styling purposes.
</div>
```

10. p tag:

This tag is used to identify a paragraph. It places a line break after the text it is enclosed in.

```html
<p>This is a paragraph of text. It can be as short or as long as needed.</p>
```

11. h1 tag:

Adds a level 1 heading to the HTML document.

```html
<h1>Thomas J. Watson</h1>
```

12. a tag:

This tag, called an “anchor tag” creates hyperlinks using the href attribute. In place of path enter the URL or path name to the page you want to link to.

```html
<a href="https://www.ibm.com">IBM</a>
```

13. img tag:

This tag is used to place an img. In place of path insert a URL or a relative file path to the image location. Other optional attributes include width and height of the image in pixels.

```html
<img
src=“https://upload.wikimedia.org/wikipedia/commons/7/7e/Thomas_J_Watson_Sr.jpg”
width=“300” height=“300”/>
```

14. table tag:

This tag is used to denote a table. Should be used with \<tr\> (defines a table row) and \<td\> (defines a table cell within a row) tags. The \<th\> tag can also be used to define the table header row.

```html
<table>
  <tr>
    <th>Header cell 1</th>
    <th>Header cell 2</th>
  </tr>
  <tr>
    <td>First row first cell</td>
    <td>First row second cell</td>
  </tr>
  <tr>
    <td>Second row first cell</td>
    <td>Second row second cell</td>
  </tr>
</table>
```

15. tr tag:

Denotes a row within a table.

```html
<tr>
  <th>Header cell 1</th>
  <th>Header cell 2</th>
</tr>
```

16. th tag:

Denotes the header cells within a row within a table.

```html
<th>Header cell</th>
```

17. td tag:

Denotes a cell within a row, within a table.

```html
<td>Cell Content</td>
```

18. li tag:

Element that creates bulleted line items in an ordered or unordered list. Should be used in conjunction with the \<ul\> or \<ol\> tags.

```html
<li>Bullet point 2</li>
```

19. ol tag:

Element that creates an ordered list using numbers. Should be used in conjunction with the \<li\> tag.

```html
<ol>
  <li>Numbered bullet point 1</li>
  <li>Numbered bullet point 2</li>
</ol>
```

20. ul tag:

Element that creates an unordered list using bullets. Should be used in conjunction with the \<li\> tag.

```html
<ul>
  <li>Bullet point 1</li>
  <li>Bullet point 2</li>
</u
```

##
