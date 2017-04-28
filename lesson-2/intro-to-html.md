

Given that every website you visit begins with "http," you can probably guess that Hyper Text is an essential building block of the Internet. In fact, building blocks are a great analogy for thinking about HTML. Hyper Text Markup Language \(HTML\) isn't really programing, in the same way that languages like Java or C are, because HTML doesn't deal with logic and interaction in any complex sense. But like those programming languages, it's important to remember that HTML is text—_only text._ Which means that every webpage you visit \(including this one\) is a pretty visual display that is created by programmatic text. 

You can see the raw HTML of any web page by right clicking on the page and selecting "View Page Source." Give it a try, I'll wait. 

...

We'll get into some of the details about what all the code means and how to interact with it, but for now just remember that what you see in your browser is the finished product, and that the HTML is the raw material.

For the assignment on the next page, we're going to write some HTML, so let's take a few minutes to review the basic elements...

### Syntax

Like other languages, HTML has certain rules for writing content, and if you break some rules or misspell something, your finished product won't work as expected.

HTML consists largely of elements \(sometimes called "tags"\) that are defined with opening and closing  brackets. Most elements have an opening tag and a closing tag, the latter of which includes a forward slash to denote the end of the element. Here's an example:

```
<element> CONTENT </element>
```

In between the two &lt;element&gt; tags is the content of this example. The content is what actually displays in the web browser, and the opening and closing tags are there to identify the type of content. 

This text is inside of a paragraph element, so in raw HTML it looks like this:

```
<p> This text is inside of a paragraph element, so in raw HTML it looks like this: </p>
```

Text, images, links, and even videos can be displayed in HTML elements, but there are also invisible elements that are used to organize content throughout a site. The most generic sort of "organizer" element is a called a div. Here's an example:

EMBED CODEPEN

https://codepen.io/BenFictional/pen/EmWVxd

Don't worry about the color yet, but just note that the &lt;div&gt; acts like a container for the two paragraph elements. There's some other behavior you can observe too in this generic example: the paragraphs are on separate lines, and the div stretches to fill the entire width of the window. 

In order for web browsers to render HTML correctly, it's expected to wrap the entire content of the page within an &lt;html&gt; element.   The other major standard is that each page includes a &lt;head&gt; and &lt;body&gt; section. The head is meant to contain invisible metadata like the page title and links to assets used later in the page. The body contains the actual content of the page. It's also good to include an additional declaration that the web browser should render this text as HTML just to make sure everything works properly: 

```
<!DOCTYPE html>
<html>
    <head>
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

&lt;p&gt; Paragraph text

&lt;h1&gt; Header One — the largest font size available with default browser behavior.

&lt;h2&gt;, &lt;h3&gt;, &lt;h4&gt;, &lt;h5&gt;, &lt;h6&gt; Successively smaller header fonts.

&lt;b&gt; Bold text; can be used in conjunction with any of the above. 

&lt;em&gt; Italic text; can be used in conjunction with any of the above. 

&lt;ul&gt; Unordered list \(bullet points\)

&lt;ol&gt; Ordered List \(numbers\)

&lt;li&gt; Each element in an ordered or unordered list. 

&lt;a&gt; Hyperlink to another web page. The format is &lt;a href="http://google.com"&gt;Some text&lt;/a&gt;

#### Media

&lt;img&gt;

&lt;video&gt;

&lt;audio&gt;

#### Layout

&lt;hr&gt;

&lt;br&gt;

&lt;div&gt;

#### HTML5

The fifth worldwide update to HTML \(2014\) introduced a number of new elements designed to help organize page content. These all function the same as a &lt;div&gt; but they have more unique names so anyone reading your code can more easily figure out what you're up to. 

&lt;header&gt; The top section of a webpage. 

&lt;nav&gt; The navigation section, typically includes menu links.

&lt;main&gt; The main content area of a page.

&lt;section&gt; Any discrete section of a page. 

&lt;article&gt; An article; one would assume with a title and author and such. 

&lt;footer&gt; The footer section, usually containing site-wide info at the bottom of a page.

You could technically use these tags however you like \(for example putting a &lt;footer&gt; at the top of your page\), but search engines use these tags to analyze what content is important on a web page. It's also important to keep your code "human-readable" so that it makes sense to collaborators and yourself. 







