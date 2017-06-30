Hyper Text Markup Language \(HTML\) isn't really programing—in the same way that languages like Java or C are—because HTML doesn't deal with logic and interaction in any complex sense. But like those programming languages, it's important to remember that HTML is text—_only text._ Which means that every webpage you visit \(including this one\) is a pretty visual display created by text.

For some upcoming exercises, we'll be writing some HTML, and even applications like Wordpress allow you to edit some of the raw HTML, so it's very useful to learn the basics. Even if you've worked with HTML before, it's always good to brush up on the specifics. If you're totally new to HTML and CSS, I recommend the fabulous [Interneting is Hard](https://internetingishard.com/html-and-css/) for further learning. 

### Syntax

Like other languages, HTML has certain rules for writing content, and if you break rules or misspell something, your finished product won't work as expected. So it's very important to check your spelling and make sure you've included the necessary punctuation—and whenever you're naming things, **use hyphens or underscores instead of spaces.**

HTML consists of elements \(sometimes called "tags"\) that are defined with opening and closing brackets. Most elements have an opening tag and a closing tag, the latter of which includes a forward slash to denote the end of the element. Here's an example:

```
<element> CONTENT </element>
```

In between the two &lt;element&gt; tags is the content of this example \(&lt;element&gt; is not a real tag, so don't try using it in your own code\). The content is what actually displays in the web browser, and the opening and closing tags are there to identify the type of content.

This line of text is inside of a paragraph element, so in raw HTML it looks like this:

```
<p> This line of text is inside of a paragraph element, so in raw HTML it looks like this: </p>
```

Text, images, links, and even videos can be displayed in HTML elements, but there are also invisible elements that are used to organize content throughout a site. The most generic sort of "organizer" element is a called a div. Here's an example:

EMBED CODE PEN: [https://codepen.io/BenFictional/pen/EmWVxd](https://codepen.io/BenFictional/pen/EmWVxd)

Don't worry about the color yet, but just note that the &lt;div&gt; acts like a container for the two paragraph elements. There's some other behavior you can observe too in this generic example: the paragraphs are on separate lines, and the div stretches to fill the entire width of the window.

In order for web browsers to render HTML correctly, it's expected to wrap the entire content of the page within an &lt;html&gt; element.   The other major standard is that each page includes a &lt;head&gt; and &lt;body&gt; section. The head is meant to contain invisible metadata like the page title and links to assets used later in the page.

The body contains the actual content of the page.

Here's a very basic template for an HTML file, including a couple standard declarations just to make sure everything runs smoothly:

```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <title>Page Title</title>
    </head>
    <body>
        <p> Some content </p>
    </body>
</html>
```

The &lt;title&gt; element defines what appears in the web browser's tab, search engine results, and other important locations.

### Common HTML Elements

You can search online for lists of complete HTML elements—here's a nice [cheat sheet](https://websitesetup.org/html5-cheat-sheet/)—but these are some of the really essential ones that you can start using right away.

#### Text

`<p>` Paragraph text

`<h1>` Header One — the largest font size available with default browser behavior.

`<h2>, <h3>, <h4>, <h5>, <h6>` Successively smaller header fonts.

`<b>` Bold text; can be used in conjunction with any of the above.

`<em>` Italic text; can be used in conjunction with any of the above.

`<ul>` Unordered list \(bullet points\)

`<ol>` Ordered List \(numbers\)

`<li>` Each element in an ordered or unordered list.

`<a>` Hyperlink to another web page. The format is `<a href="http://google.com">Some link text</a>`

#### Media

`<img>` Images—note that there is no closing tag for this; all the information is enclosed with a single tag

```
<img src="path-to-the-image" alt="Alt text" title="Image title">
```

Alt text and Image titles are not necessary, but can be included to provide additional accessibility and search-engine-optimization. Alt text is displayed if the user has images turned off \(more common in emails\), and the title is what's displayed if you hover your cursor over the image.

#### Layout

`<hr>`Horizontal rule, a line that divides sections of content.

`<br>` An empty line break.

`<div>` An invisible declaration for organizing content.

#### HTML5

The fifth worldwide update to HTML \(launched in 2014\) introduced a number of new elements designed to help organize page content. These all function the same as a `<div>` but they have more unique names so anyone reading your code can more easily figure out what you're up to.

`<header>` The top section of a webpage.

`<nav>` The navigation section, typically includes menu links.

`<main>` The main content area of a page.

`<section>` Any discrete section of a page.

`<article>` An article; one would assume with a title and author and such.

`<footer>` The footer section, usually containing site-wide info at the bottom of a page.

You could technically use these tags however you like \(for example putting a `<footer>` at the top of your page\), but search engines use these tags to analyze web pages, and it's nice to keep your code "human-readable" so that it makes sense to collaborators and yourself.

There are more HTML elements, but these should be enough to get started.

