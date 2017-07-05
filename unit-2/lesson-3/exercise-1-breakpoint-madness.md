After reading the page on "Responsive Concepts," let's put those skills to use and practice using breakpoints.

### Objectives

* Practice the syntax and workflow of mobile-first media queries.
* Dramatically change the appearance of a single web page.
* Create novel, engaging visual elements to strengthen interface design vocabulary.

### Create an HTML page

Create a new folder in your local directory for the class, and name it "lesson-3"

Create a new file called "breakpoints.html"

Here's the HTML starter template again:

```
<!DOCTYPE html>
<html>
    <head>
        <meta charset="UTF-8">
        <title>Page Title</title>
    </head>
    <body>
        <!-- Begin page content -->
    </body>
</html>
```

### Step 1. Add some content

Add whatever content you like. It could be a couple divs that you arrange in an interesting way, some images, text in various sizes, or anything you can think of.

The goal is to create_** a lot of breakpoints**_, and to create a single web page that changes dramatically as the user resizes the window. Imagine a strobe light, or a squirming creature wriggling around the page. This exercise doesn't need to useable or informative—it can be totally abstract. Or, if you prefer, you can include a quote or informative passage of text to provide some content to your design.

Some possible ideas:

* Include text about the science of light and cycle through the colors of the rainbow.
* Create a div with a weird shape and have it resize and move around the screen.
* Have text get progressively larger or smaller.
* ???

Whatever you choose, try to make it visually engaging. If you have a purposeful idea or concept behind your webpage, all the better!

### Step 2. Add at least 10 breakpoints

This is more breakpoints than you would probably use in a real project, but the goal here is to experiment and create a web page that's fun to resize back and forth.

\[INSERT SUBMISSION LINK\]



### Some CSS to play with

Here are some more advanced CSS properties to try out with this exercise:

#### Transitions

CSS transitions allow limited forms of animation to be added to a website without any complex Javascript programming. Here's a [great introduction to CSS transitions](https://robots.thoughtbot.com/transitions-and-transforms), but I'll provide the basics here.

If you have any element whose appearance changes—whether with media queries, hovering, or whatever— you can animate between the two states of that element with the CSS property `transition`

Here's a demo:

EMBED CODEPEN: [https://codepen.io/BenFictional/pen/pwVdEm](https://codepen.io/BenFictional/pen/pwVdEm)

Use `transition: all` to apply the animation to any properties that change and specify a duration for the animation in seconds. In the example above, if you wanted to only animate the size and have the color change instantly, you could write `transition: width 1.5s`. You can animate just about any CSS property from `font-size` to `opacity`.

Use this to create smooth transitions in your exercise \(if you want\).

#### Opacity

Opacity was mentioned in the CSS Crash course, but here's a demo of what it looks like when it's animated with CSS transitions.

EMBED CODEPEN: [https://codepen.io/BenFictional/pen/JJvOzy](https://codepen.io/BenFictional/pen/JJvOzy)

`opacity: 0;` is invisible and `opacity 1;` is default, so you can create transparency with values like 0.5 or 0.18957.

Also featured in this demo is another approach to CSS animations. It's more complex, but essentially I've created a variable called 'someAnimation' and triggered it with a CSS property called `animation`. [Learn more about it here](https://robots.thoughtbot.com/css-animation-for-beginners) or just copy and paste the code for your own use. Adjust the number value to change the duration of the animation.

#### Transform

This is a fun property to use in conjunction with CSS animations or transitions. You can specify a few different operations that will distort the shape and position of a div. This should feel familiar if you've started working with Adobe Illustrator. For example:

EMBED CODEPEN: [https://codepen.io/BenFictional/pen/awGEby](https://codepen.io/BenFictional/pen/awGEby)

[See a complete walkthrough here](https://robots.thoughtbot.com/transitions-and-transforms), including scale, translate, skew, and more!

#### Positioning

HTML elements default to `position: static` but you can arrange elements in more creative ways using the `position` element. Check the [W3 page](https://www.w3schools.com/cssref/pr_class_position.asp) for more info or look at this tutorial form our friends at [Interneting is Hard.](https://internetingishard.com/html-and-css/advanced-positioning/)

![](/assets/css-positioning.png)For this exercise, the most useful one is probably `position: fixed;`

An element with `position: fixed;` won't appear in the normal document flow \(i.e. top to bottom\), but instead it is manually positioned relative to the browser window. You have to declare at least one directional property like `top: 0;`or `left: 50%;`

EMBED CODEPEN: [https://codepen.io/BenFictional/pen/owdoow](https://codepen.io/BenFictional/pen/owdoow)

In this example, the squares are positioned in the corners no matter how you resize the browser—and just for fun, the a transition property is applied on the `:hover` state.

### SVG Patterns

The background-image property can apply any image as the background to a div, but SVG patterns are a popular way to add patterns to your websites—which means there are a lot of great libraries of free patterns. SVG's are a vector file type \(like those made in Illustrator\) and have much smaller file-sizes than raster images like JPEG's or PNG's. You can even add an SVG as raw code \(the raw code of a Jpeg would be hundreds of pages long\). Here are some great resources for finding SVG patterns:

* [Hero Patterns](http://www.heropatterns.com/)
* [SVG Pattern Gallery](https://philiprogers.com/svgpatterns/)



