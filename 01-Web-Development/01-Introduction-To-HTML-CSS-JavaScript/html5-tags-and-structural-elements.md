# Common HTML5 Tags and Structural Elements:

## Special HTML Elements:

In this reading, you will learn about some common HTML5 elements and their purpose. You will also learn about additional elements used for embedding content, which were introduced with HTML5.

## Objectives:

After completing this reading section, you will be able to:

1. Use common non-HTML5 specific tags
2. Differentiate between HTML5 structural elements including \<section\> and \<article\>
3. Use navigational and grouping elements
4. Use HTML5 elements specific for embedding different types of content

## Structural HTML5 Elements:

1. section tag:

The \<section\> element is used to group content in a more specific way than the \<div\> tag. The content within a \<section\> element is grouped in a semantically meaningful way, that is, there is a reason, other than for styling purposes for putting the content together. Content within a \<section\> tag has a theme, which is usually indicated by a heading tag (e.g. \<h1\>) used immediately after the opening \<section\> tag.

```html
<section>
  <h1>Section 1</h1>
  <p>This is text related to section 1.</p>
</section>

<section>
  <h1>Section 2</h1>
  <p>This is some text related to section 2.</p>
</section>
```

2. article tag:

An \<article\> element is even more specific than a \<section\> tag. It is used to group together semantically related, self-contained content which can be meaningful on its own. Similar to the \<section\> element, articles usually have headings immediately after their opening tag to indicate what the article is about.

```html
<article>
  <h1>Article 1</h1>
  <p>
    This paragraph is related only to article one and is meaningful on its own,
    without the rest of the code.
  </p>
</article>

<article>
  <h1>Article 2</h1>
  <p>
    This paragraph is related only to article two and is meaningful on its own,
    without the rest of the code.
  </p>
</article>
```

3. header tag:

The \<header\> element is a container used to define the introductory/header information of a page. It can be used for a navigational bar, or to wrap a table of contents.

An HTML document can contain more than one \<header\> elements, however, they cannot be placed within \<address\>, \<footer\>, or other \<header\> elements.

4. footer tag:

A \<footer\> element defines the area at the bottom of the page (known as a footer). This often contains copyright information, contact information, and contact links.

```html
<body>
  <article>
    <header>
      <h1>G8 summit protests</h1>
    </header>
    <div>
      <section id="public">
        <h1>Public demonstrations</h1>
        <p>...more...</p>
      </section>
      <section id="control">
        <h1>Crowd control</h1>
        <p>...more...</p>
      </section>
    </div>
    <footer>
      <p>Published today.</p>
    </footer>
  </article>
</body>
```

## HTML5 Elements for Grouping:

1. aside tag:

The \<aside\> element is used to provide additional information that is related to the main discussion​. It lets you display further content or additional resources without detracting from the main discussion​, and is often placed as a sidebar in a document.

While the \<aside\> element itself is not displayed different from the rest of the content, it is useful for understanding your code and for styling purposes.

```html
<p>
  This is a paragraph of text that casually mentions a concept and continues
  explaining the main point
</p>

<aside>
  <h4>Concept Definition</h4>
  <p>
    This goes over the concept mentioned in the paragraph to provide readers
    with further explanation if needed. However, it does not detract from the
    main content.
  </p>
</aside>
```

2. figure tag:

The \<figure\> tag defines self-contained content, such as a diagram or photo, that is referred to from the main content​. The content within the \<figure\> element should be related to the main content, but still independant in such a way that if removed from the document, it would not affect the flow.

3. figcaption tag:

The \<figcaption\> tag defines the caption for the contents of the \<figure\> element​. It can be placed as the first or last child element within the \<figure\> element​.

```html
<figure>
  <img src="images/IDSNlogo.png" width="500" height="500" />
  <figcaption>IBM Developer Skills Network Logo</figcaption>
</figure>
```

## Navigational Elements:

1. nav tag:

The \<nav\> element is used as a way to group navigational elements which are used to move between pages, such as the navigation bar typically found at the top of websites.

The \<nav\> tag is a convenience tag which does not alter the appearance on webpages. However, it is useful in styling all navigational elements, as well as omitting the content for certain functionalities, such as with screen readers.

```html
<nav>
  <div class="menu">
    <a href="#">Home</a> | <a href="about.html">About</a> |
    <a href="register.html">Register</a> |
    <a href="#">Sign in</a>
  </div>
</nav>
```

## Additional HTML5 Elements:

1. audio tag:

The \<audio\> element is used to embed sound content, such as music or podcasts. It contains one or more \<source\> tags with different audio sources (e.g. MP3, WAV), so the browser can select the first supported source to play.

If a browser does not support the audio formats provided, the browser will instead display any text within the \<audio\> element.

```html
<audio>
  <source src="soundtrack.mp3" type="audio/mpeg" />
  <source src="soundtrack.ogg" type="audio/ogg" />
  Your browser does not support the audio formats provided.
</audio>
```

2. canvas tag:

The \<canvas\> element is used to draw graphics via scripting. JavaScript is one way to utilize scripting to draw these graphics, as shown in the example below.

```html
<canvas> Your browser does not support the canvas tag. </canvas>

<script>
  var canvas = document.getElementsByTagName("canvas")[0];
  var context = canvas.getContext("2d");
  context.fillRect(0, 0, 100, 100);
</script>
```

3. embed tag:

The \<embed\> element is used as a container to embed external resources such as media players and plug-in applications into your web page.

```html
<embed type="text/html" src="another_webpage.html" />
```

4. track tag:

The \<track\> element defines text tracks, such as subtitles or captions, for \<audio\> and \<video\> elements. This text should be visible as the related media source it playing, and are formatted in the WebVTT (.vtt) format.

```html
<video>
  <source src="common_html_elements.mp4" type="video/mp4" />
  <track
    src="english_subtitles.vtt"
    kind="subtitles"
    srclang="en"
    label="English"
  />
  <track
    src="spanish_subtitles.vtt"
    kind="subtitles"
    srclang="es"
    label="Spanish"
  />
</video>
```
