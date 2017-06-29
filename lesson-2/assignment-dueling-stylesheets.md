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

`<link rel="stylesheet" type="text/css" href="css/styles-modern.css"> `

Now add your new CSS properties to "styles-modern.css"

Remember, don't spend too long on this, just focus on colors, fonts, and layout. What are some quick changes you can make to create a design that feels more like website today—we'll talk more about specific trends in contemporary design later, but for now, just go with your gut. It can still be colorful or "program-y" but try to make it look substantially different than the 90's site. 

+ Brackets Live edit tutorial

+ Explanation of HTML page links







