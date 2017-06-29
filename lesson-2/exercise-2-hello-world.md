Before completing this exercise, make sure you have read through the previous pages from this lesson on HTML, CSS, and the infrastructure of the Internet.

### Objectives:

* Examine how CSS is used in real world websites
* Practice using a browser inspector 
* Remix found material into new forms

This is a quick exercise to explore what different CSS properties can do. We'll also be using some essential tools for web development.

### Requirements

[Google Chrome](https://www.google.com/chrome/browser/desktop/index.html) web browser — you can use a different one if you prefer, but Chrome has an easy-to-use web inspector.

### Choose a website

You can try this exercise with a few websites, so don't worry too much about which one you choose. Choose a site with a variety of content.

We'll use the [Penn State homepage](http://psu.edu) for the demo.

Once you've pulled up a website, right click anywhere on the screen and choose "Inspect."

![](/assets/lesson-2/psu-home.png)

Also of note here, is the option for "View page source" which will display a the raw HTML for the current page in a new tab.

The "Inspect" option however, offers a ton of cool features in the splitscreen window seen below.

![](/assets/lesson-2/inspector.png)

The left side of the window shows the HTML and the right side shows CSS properties \(by default; if yours shows something else, click on the "Styles" tab\). If you don't see either of these panels, you'll need to click on the Elements tab along the top of the Inspector window.

\_**Pro Tip: **\_Click on the three vertical dots in the upper right of the Inspector window to move the whole Inspector to the left, right, or a separate window.

As you move your cursor around the website, you'll see visual elements highlighted in sync with the code. For example, when I opened up the Inspector, I right-clicked on the words "This is Penn State" in the top navigation menu—highlighted in the code, I can see that this is an `<a>` element within an `<li>` within an `<ul>` and so on.

If you double click on HTML content, you can edit the code. For example, here I changed the text of the link to say "This is a swell website."

![](/assets/lesson-2/ swell-website.png)

Pressing Return makes the changes take effect, and the new text appears in the website!

**These changes only appear in your web browser! **

**And they're temporary, so if you refresh the page, your changes will be gone.**

![](/assets/lesson-2/inspector-font-size.png)

You can change CSS properties in real time too. Here, I scrolled down in the Styles panel, until I found the CSS property `font-size` — which was 18px. I changed the code to 80px to see what would happen. In some cases, the whole navigation menu might expand to make room for the enormous text, but one of the HTML elements containing this `<a>` element has a property of `overflow: hidden;` and a fixed dimension of `height: 32px;`

**Optional Challenge:** Search through the CSS properties of [psu.edu](http://psu.edu) and try to find those declarations; unchecking the blue check boxes, will turn off the properties, and you'll be rewarded with a giant navigation menu of overlapping text.

![](/assets/lesson-2/inspector-nav.png)

## Exercise 2: Break The Internet

Using a website of your choice \(don't use the PSU homepage\), use the web inspector to modify the CSS and make the website look dramatically different. It can be distorted beyond recognition; think of this as making an abstract painting, use dynamic colors and scale changes.

Use this as an opportunity to experiment with CSS properties and see what happens.

**Some tips:**

* You can edit the HTML too, but it's not necessary. 
* HTML elements that contain other elements will have gray arrows that you can click to reveal the contents of the container.
* The easiest way to target a specific element is to right-click on it and choose Inspect again.
* If you find an image \(either in the HTML or CSS\), you can replace it with any image on the Web by replacing the filepath with a new URL \(the URL needs to be for the image itself, ending in .jpg or .png or the like\).

* You can stretch and distort images by altering their width and height values.

* You can add all new CSS properties in addition to modifying existing ones.

* Change fonts to any of the main [web-safe fonts ](https://www.w3schools.com/cssref/css_websafe_fonts.asp)\(including Comic Sans\).

* If you find a color property in the CSS, you can click on the colored square to open a color picker widget.

* If you're struggling to make something interesting, just start unchecking boxes at random.

![](/assets/lesson-2/color-picker.png)

Try it with a couple websites if you want, but when you've created something **weird** and **dramatically different** than the original site, take a screen shot and submit it below.

**Mac:** ⌘+Shift+4 \(select part of the screen\) or open the [Grab utility](http://appletoolbox.com/2013/01/how-to-use-mac-os-x-grab-utility-to-take-screenshots/).

**Windows:** Open the [Snip application](https://support.microsoft.com/en-us/help/13776/windows-use-snipping-tool-to-capture-screenshots).

\[INSERT SUBMISSION LINK\]

Here's the PSU homepage after some further CSS alterations"

![](/assets/lesson-2/psu-hack.png)

The magnifying glass in the search bar was set via a `background-image` CSS property, which included the declaration `no-repeat`; I changed it to `repeat` and increased the width and height to create a big pattern square \(and used some other properties to move it away from the upper-right of the screen\).

