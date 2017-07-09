## Designers & Developers

When discussing websites, apps, and software creation, the workload is frequently split into two categories: **designers **create the visual look of the content, and create a layout that organizes everything in a logical way; **developers **take the visual design and turn it into a functional website or app using whatever platform best fits the job \(usually involving a lot of coding\). 

This workflow allows designers and developers to specialize in their areas, and leave some details to their collaborators—but for individuals and small teams, the distinction may not be as clear. Even if you are working in one of those roles, it's very useful to know some of the work associated with the other side of the job. Today designers are more frequently expected to build functioning prototypes of websites,  prepare files for development use, and understand what is and isn't possible in a design. 

## HTML

Hyper Text Markup Language \(HTML\) isn't really programing—in the same way that languages like Java or C are—because HTML doesn't deal with logic and interaction in any complex sense. But like those programming languages, it's important to remember that HTML is text—_only text._ Which means that every webpage you visit \(including this one\) is a pretty visual display created by text.

While this course focuses on the overall design of web content, we will be doing one assignment involving a bit of HTML, and even applications like Wordpress allow you to edit some raw HTML, so it's very useful to learn the basics. If you're totally new to HTML and CSS, I recommend the fabulous [Interneting is Hard](https://www.gitbook.com/book/psu-arts-arch/dart-203/edit#) for further learning.

### Syntax

Like other languages, HTML has certain rules for writing content, and if you break rules or misspell something, your finished product won't work as expected. So it's very important to check your spelling and make sure you've included the necessary punctuation—and whenever you're naming things, **use hyphens or underscores instead of spaces.**

HTML consists of elements \(sometimes called "tags"\) that are defined with opening and closing brackets. Most elements have an opening tag and a closing tag, the latter of which includes a forward slash to denote the end of the element.

This line of text is inside of a paragraph element, so in raw HTML it looks like this:

```
<p> This line of text is inside of a paragraph element, so in raw HTML it looks like this: </p>
```

Text, images, links, and even videos can be displayed in HTML elements, but there are also invisible elements that are used to organize content throughout a site. The most generic sort of "organizer" element is a called a div. Here's an example:

EMBED CODE PEN: [https://codepen.io/BenFictional/pen/EmWVxd](https://codepen.io/BenFictional/pen/EmWVxd)

Don't worry about the color yet, but just note that the &lt;div&gt; acts like a container for the two paragraph elements. There's some other behavior you can observe too in this generic example: the paragraphs are on separate lines, and the div stretches to fill the entire width of the window. Divs, paragraphs, images, and other HTML elements act like building blocks, stacking and nesting inside each other to make up the contents of a web page.

In order for web browsers to render HTML correctly, it's expected to wrap the entire content of the page within an &lt;html&gt; element.   The other major standard is that each page includes a &lt;head&gt; and &lt;body&gt; section. The head is meant to contain invisible metadata like the page title; the body contains the actual content of the page.

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

The &lt;title&gt; element defines what appears in web browser tabs, search engine results, and other important locations.

### Common HTML Elements

You can search online for lists of complete HTML elements—here's a nice [cheat sheet](https://websitesetup.org/html5-cheat-sheet/)—but these are some of the really essential ones that you can start using right away.

#### Text

`<p>` Paragraph text

`<h1>` Header One — the largest font size available with default browser behavior.

`<h2>, <h3>, <h4>, <h5>, <h6>` Successively smaller header fonts.

`<ul>` Unordered list \(bullet points\)

`<ol>` Ordered List \(numbers\)

`<li>` Each element in an ordered or unordered list.

`<a>` Hyperlink to another web page. The format is `<a href="http://google.com">Some link text</a>`

#### Media

`<img>` Images—note that there is no closing tag for this; all the information is enclosed with a single tag

```
<img src="path-to-the-image/file.jpg" alt="Alt text" title="Image title">
```

The **alt text** and **image title** are not necessary, but can be included to provide additional accessibility and search-engine-optimization. Alt text is displayed if the user has images turned off \(as is common in emails\), and the title is what's displayed if you hover your cursor over the image.

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

`<aside>` Supplementary content like a sidebar.

`<footer>` The footer section, usually containing site-wide info at the bottom of a page.

You could technically use these tags however you like \(for example putting a `<footer>` at the top of your page\), but search engines use these tags to analyze web pages, and it's nice to keep your code "human-readable" so that it makes sense to collaborators and yourself.

