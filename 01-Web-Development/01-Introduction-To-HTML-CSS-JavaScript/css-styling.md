## What is CSS ?

1. CSS is the design that is layered over the top of an HTML web page.
2. CSS is a style sheet language that describes how HTML elements are displayed.
3. What makes the style sheet “cascading” is that developers can apply CSS to create a uniform look throughout each element of each page of the website.
4. Child and descendant elements often inherit styles that are defined for parent elements.
5. For websites, it is an important concept to separate the data from the design.
6. You can code CSS as a style attribute in an HTML tag, a head section of a document, or an external document.

## Choosing a Layout:

1. Fluid layout:

A fluid layout: is a layout in which the height and width of elements is flexible and can expand or contract based on the browser window, the operating system, and other user preferences. You specify these elements mostly by using percentages and ems.

2. Fixed layout:

A fixed layout: is a layout where you specify the height and width of elements, and those values remain the same regardless of which operating system or browser you use to access the website. You specify these elements mostly by using pixels.

## Applying CSS:

1. Inline CSS:

This is used for a single HTML element, But the HTML document can get messy very quickly as more styles get added To use this method, insert the "style" attribute inside any HTML element.

```html
<p style="color:red;">Some Text</p>
```

2. Internal CSS:

This is used for a single page, however It “dirties” the page with a non-HTML code. If you copy and paste this style on each page, this approach increases the load time of each page, which causes the user to wait longer. To use this method, the \<style\> tag must be used, with your CSS code inside.

```html
<style>
  p {
    color: "red";
  }
</style>
```

3. External CSS:

This method is used to style an entire website. You can link to it from other pages, which ensures a clean HTML and a smaller page size. To use this method, the \<link\> tag must be added to the \<head\> tag section in your HTML code.

```html
<head>
  <link rel="stylesheet" type="text/css" herf="style.css" />
</head>
```

# NOTE :

The type with the highest priority will override the others and be applied to that element. The order of precedence for CSS styles is Inline CSS, which has a higher priority than Internal CSS, which, in turn, has a higher priority than External CSS.

```
Inline CSS -> Internal CSS -> External CSS
```
