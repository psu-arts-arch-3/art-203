You can meticulously build a website by hand-coding it in HTML, but it won't look very interesting. That's because web browsers render HTML in a very simple way by default: focusing only on the content with no "decoration" at all. Here's an example of what raw HTML looks like:

EMBED CODE PEN: [https://codepen.io/BenFictional/pen/Wjqoye](https://codepen.io/BenFictional/pen/Wjqoye)

By default text will be ver rendered in a black **serif font,** and the different headers will appear at a particular size. 

For the record there are three families of fonts:

![](/assets/font-demo.png)

Serifs are the "feet" on the ends of characters; they're designed to guide the reader's eye along each line of text. We'll talk more about typography soon...

In order to make the fun design decisions like which fonts to use, adding colors, spacing, and other decorative elements, HTML files need declared styles.

Styles can override the default way that browsers render HTML, and can contribute a really staggering amount to a website. The advantage of keeping visual styles separate from the core HTML is that they appearance of a website can be easily updated without interfering with the content. Styles are defined in a separate markup language called Cascading Style Sheets \(CSS\) that has it's own syntax and rules. 

The simplest way to think about CSS is that it defines various attributes to HTML elements. For example you could set certain attributes for all a paragraph elements: font-size, text color, background color, and so on. 

You can define these styles within a` <style>` element in the `<head>` of an HTML file:

EMBED CODE PEN: [https://codepen.io/BenFictional/pen/aWgpbq](https://codepen.io/BenFictional/pen/aWgpbq)

This is a very simple example, but it demonstrates the formatting for CSS. The font-size can be measured in a few different units, but I used pixels here as the most basic option. color and background-color can accept colors represented in Hex codes \(e.g. \#FF43D2\) or one of the web-safe [HTML color names](https://www.w3schools.com/colors/colors_names.asp).

You can target all instances of an HTML element like &lt;p&gt; or &lt;h1&gt;, or you can target specific instances by naming the HTML elements with an **ID** or **Class.** 

EMBED CODE PEN: [https://codepen.io/BenFictional/pen/RVzKNd](https://codepen.io/BenFictional/pen/RVzKNd)

I added some new properties in this example. Note that you can make text bold in CSS instead of using a `<b>` element in HTML.

ID's target one specific instance within the HTML, and classes can target multiple instances—for example, you might want to include several pieces of big header text throughout a page, and you could give them all `class="big-awesome" `





