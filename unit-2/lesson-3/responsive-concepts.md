You've probably heard the terms "responsive," "fluid," or "mobile-first" used in refernece to web design, but let's take a look at exactly what they mean and how to best utilize responsive practices in your own projects.

## Screen Sizes

In our CSS Crash Course, a number of different units were provided, including "px," "em," and "%." Recall that these units specify the size of any elements in a website. For a long time the most popular unit was "px" \(pixel\) because it was most familiar unit for many designers.

An "em" is equal to the height of the current font-size. For most browsers, the base font-size is 18px high, but that will change if you're working with a header element \(which is much taller than a regular paragraph\).

"Em" and "px" are both fixed units, and the problem with using them for the overall layout of a site is illustrated by the following Codepen—try resizing your browser window and watch what happens:

EMBED CODEPEN [https://codepen.io/BenFictional/pen/WOJEwv](https://codepen.io/BenFictional/pen/WOJEwv)

As the browser width shrinks, the content is clipped—preventing a reader from seeing everything. And as the browser expands, there is eventually a bunch of wasted space outside the main content area.

Compare that to this example of a weather site:

![](/assets/responsive-demo.gif)

This example showcases several of the terms mentioned at the beginning:

**Fluid**: The content uses percentage-based dimensions to stretch with the size of the screen.

**Adaptive**: At certain screen sizes, the content actually changes it's layout entirely \(in this case, the list of days shifts from a row to a column\).

**Responsive:** A combination of fluid and adaptive properties optimized for making the content look good across devices and screen sizes.

It goes without saying that websites today need to look good on any device. In the 1990's, most screens displayed somewhere from 640-1040px wide, but today's websites need to work on a variety of screen sizes:

#### Mobile \(&lt;600px wide\)

While many new phone screens are full HD \(1920px x 1080px\), if they rendered text with the same em height at an HD computer screen, the text would be incredibly tiny. For example, the iPhone 6 renders web browsers at 375px x 559px \(more details on [iphone screen sizes](http://www.kylejlarson.com/blog/iphone-6-screen-size-web-design-tips/)\)

#### Tablet \(~700–1000px\)

Intermediary screen sizes get a lot of use, and some people opt for a category between mobile and tablets \(called "phablets"\). Websites will frequently be displayed in this range of laptops and desktops too, since many people don't maximize their web browsers to fill the entire screen.

#### Desktop \(~1000–1920px\)

HD video is 1920px x 1080px, and that's a common size for computer screens, so this is usually a good number to think about as a maximum screen size \(such as when creating images to be used as backgrounds\).

#### Extra Large \(&gt;1920px\)

The rise of 4K video \(3840px x 2160px\) has paved the way for even larger screens, sometimes labeled as Ultra-High Definition \(UHD\). Apple's Retina displays aren't quite this large, but they are larger than HD, however most people keep their displays scaled down to HD or smaller to keep text large enough to read. I usually work with HD as a target size, but if you think people will look at your site on UHD screens, then include some extra high-res images.

## Mobile-first

In addition to screen size, the popularity of smartphones means that websites need to load _fast_. Users frequently access websites over cellular networks with limited bandwidth, so including data-heavy assets like images, videos, and plugins can really slow down a site's performance.

In order to deliver content as fast as possible, most websites aim to deliver optimized content specifically for mobile users... and then if a user is on a larger screen \(usually signifying that they're on a computer and a proper WIFI connection, then the website will serve up larger images and extra content. This approach is called **mobile-first**, and also implies that the design for the website** begins with mobile-users in mind,** and then expands—as opposed to beginning a design with desktop site, and then removing elements to make it fit on a smartphone.

#### The mobile-first approach forces the designer to identify the simplest, most essential aspects of the content. 

Keep that in mind with our upcoming projects.

One of the main ways that designers restrict content depending on screen size is by using **media-queries**—which we'll get to in a second—but a website might also present different content depending on a user's browser, location, or installed applications.

**Check out **[**clickclickclick.click**](https://clickclickclick.click/#0ceb8962712a9ca28de290b4264c72da)** **for a weird and wonderful look at the type of information transmitted by your web browser. 

## Media Queries

Media queries are a CSS element that lets you target specific screen sizes, just as you might target specific classes or id's. Pretty much all platforms for web development use media queries, so whether you're coding a site from scratch, or using Wordpress, Squarespace, or Muse, it's important to understand the concept. 

Here's the syntax:

```
@media only screen and (min-width: 480px) {
    /*Some CSS properties */
}
```

EMBED CODEPEN: https://codepen.io/BenFictional/pen/jwxGXv

Resize the window to see the new CSS properties kick in and change the color and size of the square.

The @media object has a variety of options that you can declare. It will still work if you omit  `only screen and`, but it's standard practice to include those because:

* `screen `prevents extra styles from applying to printed pages and other media types.
* `only` prevents older browsers from loading the media query and getting confused. 

You can write a media query to kick in at a min-width \(when the browser is at least 480px wide\) or a max-width \(when the browser is smaller than 480px\). Since we want to create websites mobile-first, the best way to include media queries is:

```
/* Default mobile styles */

@media only screen and (min-width: 480px) {
    /* Tablet styles */
}

@media only screen and (min-width: 768px) {
    /* Desktop styles */
}
```

The widths that trigger new media queries are called **Breakpoints **and you can have as many of them as your design requires \(though limiting it to 3 makes your life easier\). A good approach is to start with your mobile design, and then gradually increase the browser width until it starts to look weird.  

**Check out the online tool **[**Ish 2.0**](http://bradfrost.com/demo/ish/) — enter any URL at the top of the screen and hit the "DISCO" button to start stretching the website in all sorts of sizes; it's a good way to find bugs in your design or just see how real-world sites deal with media queries. 







