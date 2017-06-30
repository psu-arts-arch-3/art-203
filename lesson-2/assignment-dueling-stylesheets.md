After completing Exercise 1 and 2 for this lesson, you should have a basic understanding of HTML and CSS. This assignment will provide further experience designing with code, and connect with the subject of this lesson's blog entry.

### Objectives

* Apply visual styles to a ready-made HTML project. 
* Recreate the aesthetics and design trends of a specific period of web design.
* Imagine multiple design solutions for a single piece of content. 

### Get the Template Files

Download the sample HTML project from this GitHub repository.

1. Click the green "Clone or Download" button.
2. Choose "Download Zip"
3. Unzip the file on your computer by double-clicking. 
4. Copy the contents of the "lesson-2" folder to your local-directory folder, and place it inside your art203 subdirectory. 

The file structure should be: "../local-directory/art203/lesson-2/index.html"

The sample project includes two HTML files and a folder called "css" that contains two files: "styles-90s.css" and "styles-modern.css"

CSS properties can be included in the `<head>` section of a single html page, but it's common practice to place all the CSS in a separate file to keep things organized.

The "index.html" file contains a link to "style-90s.css" in the `<head>` section—this imports the file and applies all the CSS values.

Open the HTML file in a web browser and take a look at the structure of the website and how it is defined in the code.

## Assignments: Duelling Stylesheets

### **Part 1**

** **Edit "styles-90s.css" to create a stylesheet \(i.e. list of CSS properties\) that makes the sample webpage look like finsihed website from the 1990's. Based on your research for this week's blog post, consider the colors, fonts, and design styles used by designers of that era.

Ignore the file called "index-alt.html" for now.

The "index.html" file is set to use the "styles-90s.css" by default, so add your properties there. The design doesn't have to be a masterpiece, in fact, you should feel free to make your design ugly or simplistic if that's how you choose to interpret the aesthetics of the 90's. But try to make your design look _complete_—like you've spent some time on it.

You can leave the HTML alone, but you are encouraged to add new text and images to make the site look more complete—for example, add some images of some Tamagotchis, and write a few sentences to make the site appear to be a a [Tamagotchi](https://en.wikipedia.org/wiki/Tamagotchi) advice column, or Pepsi recipe collection, or sneaker collection blog, etc. **Creativity will be rewarded! **

To add new images, place JPEG or PNG files in the folder called "img" and change the links in the HTML to match the filename of your images.

Just stick to the [web-safe fonts](https://www.w3schools.com/cssref/css_websafe_fonts.asp) for historical accuracy.

### **Part 2**

Create an alternate stylesheet to apply a modern look to the same HTML content. Leave whatever 90's text and images you added, and let's just focus on the visual design. The second version of the site should look _substantially_ different from the 90's version.

Once you're ready to work on the modern version, change the link in the `<head>` to the other CSS file:

`<link rel="stylesheet" type="text/css" href="css/styles-modern.css">`

Now add your new CSS properties to "styles-modern.css"

Remember, don't spend too long on this, just focus on colors, fonts, and layout. What are some quick changes you can make to create a design that feels more like website today—we'll talk more about specific trends in contemporary design later, but for now, just go with your gut. It can still be colorful or "program-y" but try to make it look substantially different than the 90's site.

### Using Brackets

You should use Brackets to edit the template files; just select Filer &gt;&gt;&gt; Open folder

Brackets has several features that will make your job easier. It automatically color-codes different properties to help you understand the code, and it offers prompts as you begin typing. For example, if I type `<div>` in an HTML file, it will automatically generate the closing `</div>` tag. Or if I type the letter "b" in a CSS file, it will suggest a variety of properties starting with that letter.



You should also try out the Live Preview mode by pressing the Lighting Bolt icon in the upper-right of the Brackets window. This opens a special web browser that shows a live preview of your files; it even changes dynamically as you edit the HTML or CSS. If you click on an HTML tag or a CSS selector the targeted area will be highlighted in the Live Preview browser, similar to how the web inspector works in Chrome.



### Finishing Up

Once you've created your two stylesheets, we're going to set up a second HTML page, so that a user can see both stylesheets without having to edit the code. 

1. Set the stylesheet link in "index.html" back to "styles-90s.css"
2. Save
3. Copy everything within the `<body>` and `</body>` tags from "index.html" \(but don't copy the body tags themselves\).
4. Paste that text in between the `<body>` tags in "index-alt.html" beneath the comment that says "Paste content here"
5. Save

"index-alt.html" is set to apply the CSS from "styles-modern.css" — so you should have two different HTML pages, each with identical HTML, but linking to different stylesheets. I would have done this for you at the beginning, but this way if you edited the HTML content at all, it will be the same in both pages. 

The `<a>` links in the `<nav>` menu are set to the two different HTML files, so that when you click on the links, you should be able to switch back and forth between your two stylesheets. You can't dynamically apply new stylesheets to a single HTML file without programming some Javascript, so we just set up two identical HTML pages.

Upload your entire "lesson-2" folder to your PSU server using Filezilla like we did in Exercise 1. Make sure you upload the folder itself into the "art203" folder online, and include the image and CSS folders. 

The resulting filepath should be `http://pass.psu.edu/user123/art203/lesson-2/index.html`

\[INSERT SUBMISSION LINK\]





