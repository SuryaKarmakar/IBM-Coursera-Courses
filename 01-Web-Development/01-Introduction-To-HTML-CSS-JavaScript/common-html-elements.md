# Common HTML Elements:

This reading will introduce you to the most common HTML elements you need to know as a web developer. The HTML elements described in this reading are key to your learning.

## HTML Setup:

Recall that an HTML document must always start by specifying the DOCTYPE. The entire content is then enclosed within an \<html\> tag. Within this tag, the content is further segregated into either the \<head\> or \<body\> elements of the code. The \<head\> tag contains all the metadata about the page, and the \<body\> tag contains the content that is displayed to the end user.

As per this setup, an empty HTML document without content or metadata should look as follows:

```html
<!DOCTYPE html>
<html>
  <head>
    <!-- Metadata goes here -->
  </head>
  <body>
    <!-- Content goes here -->
  </body>
</html>
```

## Browser Tab Title:

The title of the page appears on the browser tab when you open a webpage in the browser. For example, if you open Google in a new tab, the browser title will display as “Google” along with the Google logo.

You can define the browser title using the \<title\> tag, which is placed within the \<head\> section of your HTML markup as follows:

```html
<head>
  <title>Sample Page Title</title>
</head>
```

## Page Headings:

You can separate your information into different sections by using headings, as can be seen in this reading. HTML defines six different font sizes for headings. Each heading represents a different level of importance and text size.

HTML headings are defined with the following tags: \<h1\>, \<h2\>, \<h3\>, \<h4\>, \<h5\>, and \<h6\>. The number in these tags specifies the importance, with \<h1\> being the largest heading and \<h6\> being the smallest heading.

Since this element defines the content within a web page, it should be placed in the \<body\> section of your markup as follows:

```html
<body>
  <h1>Most Important (and Largest) Heading</h1>
  <h6>Least Important (and Smallest) Heading</h6>
</body>
```

## Adding Text:

The \<p\> tag should be used to insert text into your HTML document. This element stands for paragraph and includes any text content, whether it is a single word or a 10-page essay.

Since this element defines content within a web page, it should be placed in the \<body\> section of your markup as follows:

```html
<body>
  <p>
    This is some text. The content within this paragraph element can be as short
    or as long as needed.
  </p>
  <p>This is another paragraph of text.</p>
</body>
```

## Using Line Breaks:

A line break is used to complete one line and continue the remaining text
at the start of a new line, like what was just done here.

This can be useful in many scenarios, such as when writing addresses. You can use the \<br\> tag to insert a line break in HTML. This is not a container tag and therefore does not have an end tag.

```html
<body>
  <p>
    This is some text that needs to be split up <br />here, <br />here, and
    <br />here.
  </p>
</body>
```

## Add Links to Other Pages:

Web pages can link to other pages or other places on the same page via a hyperlink. The \<a\> tag defines a hyperlink in HTML, followed by the href attribute to define the destination address of the hyperlink.

Hyperlinks are normally inserted into text so that when you click some hyperlinked text, it takes you to the destination. For example, if you want to hyperlink the word “IBM” to the official IBM website, you can use the \<a\> tag with the href attribute as shown below:

```html
<a href="https://www.ibm.com">IBM</a>
```

## Create a List:

To create a list of items, you can use the \<ol\> (ordered list) tag for numbered lists and the \<ul\> (unordered list) tag for bulleted lists.

Each point within a list will be enclosed by a \<li\> opening and closing tag, which represents a list item. This same tag is used for both ordered and unordered lists.

```html
<body>
  <!-- Unordered List -->
  <ul>
    <li>This is a bullet point</li>
    <li>The items in this list have no particular order</li>
    <li>Each item will appear as a bullet, rather than a number</li>
  </ul>

  <!-- Ordered List -->
  <ol>
    <li>This is an ordered list</li>
    <li>The items in this list have a particular order</li>
    <li>Each item will be numbered, starting from 1</li>
    <li>This is the fourth point in the list</li>
  </ol>
</body>
```

## Add a Table:

A table is created with HTML using the \<table\> tag. Within the table, each row of data is represented using the \<tr\> (table row) tag. The column or row headings can be specified by the \<th\> (table heading) element. Finally, each data element within the table cells is specified using the \<td\> (table data) tag.

```html
<body>
  <table>
    <!-- Table Row -->
    <tr>
      <!-- Table Heading -->
      <th>Heading 1</th>
      <th>Heading 2</th>
      <th>Heading 3</th>
    </tr>
    <tr>
      <!-- Table Data -->
      <td>H1 - Data Item 1</td>
      <td>H2 - Data Item 1</td>
      <td>H3 - Data Item 1</td>
    </tr>
    <tr>
      <td>H1 - Data Item 2</td>
      <td>H2 - Data Item 2</td>
      <td>H3 - Data Item 2</td>
    </tr>
    <tr>
      <td>H1 - Data Item 3</td>
      <td>H2 - Data Item 3</td>
      <td>H3 - Data Item 3</td>
    </tr>
  </table>
</body>
```

## Add an Image:

Images can be added within a web page by using the \<img\> tag. Both external images (for instance, from the internet) and local images (for instance, files saved on your computer) can be used in this tag.

To add an image, you need to know the image file name and include it in the ‘src’ attribute. The ‘src’ attribute specifies an external resource that you want to link, such as the URL of an image. If you are referencing a file online, you can insert the URL of the image in this attribute. If you want to insert a local image, you should insert the file path of the image relative to the location of your HTML file.

The \<img\> tag also requires the ‘alt’ attribute, which defines alternative text to be displayed in the event the image cannot be loaded and when a screen reader is used.

The size of an image can also (optionally) be specified using the ‘width’ and ‘height’ attributes, with the numbers listed in pixels.

```html
<body>
  <!-- External Image -->
  <img
    src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/51/IBM_logo.svg/440px-IBM_logo.svg.png"
    alt="IBM Logo"
    width="300"
    height="300"
  />
  <!-- Local Images -->
  <img src="images/IBMlogo.png" alt="IBM Logo" width="300" height="300" />
</body>
```
