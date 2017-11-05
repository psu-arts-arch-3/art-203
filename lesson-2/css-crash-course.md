You can meticulously build a website by hand-coding it in HTML, but it won't look very interesting. That's because web browsers render HTML in a very simple way by default: focusing only on the content with no "decoration" at all. Here's an example of what raw HTML looks like:

EMBED CODE PEN: [https://codepen.io/BenFictional/pen/Wjqoye](https://codepen.io/BenFictional/pen/Wjqoye)

By default text will be rendered in a black **serif font,** and the different headers will appear at a particular size.

In order to make fun design decisions like which fonts to use, adding colors, spacing, and other decorative elements, HTML files need declared styles.

## Cascading Style Sheets \(CSS\)

Styles can override the default way that browsers render HTML, and can contribute a really staggering amount to layout and appearance. The advantage of keeping visual styles separate from the core HTML is that they appearance of a website can be easily updated without interfering with the content. Styles are defined in a separate markup language called Cascading Style Sheets \(CSS\) that has it's own syntax and rules.

The simplest way to think about CSS is that it defines various attributes to HTML elements. For example you could set certain attributes for all a paragraph elements: font-size, text color, background color, and so on.

You can define these styles within a`<style>` element in the `<head>` of an HTML file, or within a separate .CSS file:

EMBED CODE PEN: [https://codepen.io/BenFictional/pen/aWgpbq](https://codepen.io/BenFictional/pen/aWgpbq)

This is a very simple example, but it demonstrates the formatting for CSS:

1. Set a target selector
2. Add curly brackets `{ }`
3. Within the brackets: specify a property, followed by a colon `:` , a value, and a semi-colon `;`

**Pro Tip: **_Never forget the semi-colon._

The font-size can be measured in a few different units, but I used pixels here as the simplest option. Color and background-color can accept colors represented in Hex codes \(e.g. \#FF43D2\) or one of the web-safe [HTML color names](https://www.w3schools.com/colors/colors_names.asp).

You can target all instances of an HTML element like `<p>` or `<h1>`, or you can target specific instances by naming the HTML elements with an **ID** or **Class.**

EMBED CODE PEN: [https://codepen.io/BenFictional/pen/RVzKNd](https://codepen.io/BenFictional/pen/RVzKNd)

In the HTML for each paragraph, I specified a class; in the CSS, I can assign properties to anything with that class. You can also assign ID's for an element, but unlike classes, ID's can only be used for one specific element.

While you can name elements whatever you want, it's important to spell everything correctly. Use a consistent naming convention and syntax to stay organized.

There are _a lot_ of CSS properties, and they function in complex and inter-connected ways, so we'll just go over some basic ones that are relevant to the upcoming assignment. For reference, here is a [longer list of CSS properties](https://cdn.makeawebsitehub.com/wp-content/uploads/2015/10/css3-mega-cheat-sheet.jpg) to play with.

An invaluable resource for working with CSS is the [World Wide Web Consortium ](https://www.w3schools.com/)—if you Google any of the following properties, the first result will probably be the relevant W3 page listing all possible values with examples. And for more thorough tutorials...

#### CSS Tutorials:  [Interneting is Hard. ](https://internetingishard.com/html-and-css/)

_**Don't panic! You can skim this page and come back to it when you start working on upcoming assignment. **_

### **Text**

These properties can be applied to a `<p>` or any header element, or if you declare them with reference to a container, like a `<div>`, the styles will be applied to any text elements within the container.

`font-family:` can take the value of any of the [standard web fonts.](https://www.w3schools.com/cssref/css_websafe_fonts.asp) In order to use other fonts, you'll have to include them as dedicated font files or use fonts hosted on a public library like [Google fonts](https://designshack.net/articles/css/a-beginners-guide-to-using-google-web-fonts/).

`font-size:` takes a number value with any of the standard HTML units.

`font-weight:` set to normal or bold.

`color:` takes any of the [standard HTML color names](https://www.w3schools.com/colors/colors_names.asp) or color values inputed via Hex-code. We'll get into more advanced color details later.

`text-decoration:`set to "none" or "underline"

`line-height:` the space between lines—set to "auto" by default, but you can also set with a number and unit.

### Layout

These properties are mostly used with `<div>` elements or other containers, but can be applied to images and other elements too.

`width:` "auto" by default. Set with a number and unit—note that some a `<div>` will not have any width or height unless it has content within it, or you set the dimensions via CSS.

`height:` works similar to width; height can not be set to 100%.

`margin:` set with a number/unit; adds space around an element.

`margin-left:` adds a margin to only one side; you can sub in "right", "top", or "bottom".

`padding:`set with a number/unit. adds space inside an element, surrounding the content.

`padding-top:` padding for just one side; use with all four directions.

`float:`takes "left" or "right" will force an element to the left/right until it hits another element. Images and text will normally be placed on a new row _below_ the previous element, but this will force things to sit next to each other—if there's room.

`text-align:`Sets paragraph alignment for text within a container. Takes "left", "right", or "center."

`opacity:` takes a number between "1.0" \(full opacity\) and "0.0" \(invisible\).

![](/assets/lesson-2/box-demo.png)

### **Border**

Apply to container elements or images.

`border-style:` "solid", "dashed", or "dotted."

`border-color:` takes color value.

`border-width:` takes number/unit.

`border:` set all of the above properties with one line: `border: 1px solid red;`

`border-bottom:` set border for only one side \(can also use "top", "left", or "right"\).

### **Background**

`background-color:` takes a color value.

`background-image:` set an image as the background: `background-image: url("path-to-image/file.jpg");`

`background-repeat:` if a background image is smaller than it's container, set whether it tiles or displays only once. Set to "repeat", "repeat-x", "repeat-y", or "no-repeat".

`background-size:`default is "auto" but you can specify a number/unit or, more commonly, set this to "cover" to display the image as large as possible to fill the element.

`background:` set either a background color or image, can be overridden if you declare competing rules.

### Colors

We'll talk more about how to use color effectively, but for now, just know that any color can be represented as a six digit string of numbers and letters called a **Hex-code **\(or Hex triplet\). We'll go over the details later, but for now just use a color picker with a graphic interface and copy and paste the Hex value \(e.g. "\#5D32F0"\) into your CSS.

I recommend using [Adobe Color](https://color.adobe.com/), or you can just search Google for "color picker" and access a simpler one.

### Units

Many of the properties above take number values, and while a number without a unit will default to pixels, there are a bunch of other units that are very useful.

**Pixels **\(e.g. "700px"\) Sets dimensions with a **static** value measured in your screen's pixels.

**Percent **\(e.g. "50%\) Sets dimensions in with a **relative** value, as a percent of the parent element. This means that as the size of the browser window \(or device\) changes, the size of the element will change.

**Viewport** \(e.g. "20vw" or "20vh"\) Sets dimensions as a percent of the browser window width \(vw\) or height \(vh\). This is different from percent, because percent measures from the parent element, not necessarily the browser window \(an element of `width: 50%;` within an element of `width: 400px;` will be always be 200px.

**Font Size** \(e.g. "2em"\) sets dimensions based on the size of a text character \(1em\). This is a little more advanced, but is frequently used by designers as a slightly more dynamic value than pixels.

Here's a demo to help visualize these different units—try resizing the browser:

EMBED CODE PEN: [https://codepen.io/BenFictional/pen/GmVBZz](https://codepen.io/BenFictional/pen/GmVBZz)

