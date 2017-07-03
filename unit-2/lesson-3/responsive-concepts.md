You've probably heard the terms "responsive," "fluid," or "mobile-first" used in refernece to web design, but let's take a look at exactly what they mean and how to best utilize responsive practices in your own projects.

### Screen Sizes

In our CSS Crash Course, a number of different units were provided, including "px," "em," and "%." Recall that these units specify the size of any elements in a website. For a long time the most popular unit was "px" \(pixel\) because it was most familiar unit for many designers. 

An "em" is equal to the height of the current font-size. For most browsers, the base font-size is 18px high, but that will change if you're working with a header element \(which is much taller than a regular paragraph\).

"Em" and "px" are both fixed units, and the problem with using them for the overall layout of a site is illustrated by the following Codepen—try resizing your browser window and watch what happens:

EMBED CODEPEN https://codepen.io/BenFictional/pen/WOJEwv

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

### Mobile-first

In addition to screen size, the popularity of smartphones means that websites need to load _fast_. Users frequently access websites over cellular networks with limited bandwidth, so including data-heavy assets like images, videos, and plugins can really slow down a site's performance. 

In order to deliver content as fast as possible, most websites aim to deliver optimized content specifically for mobile users... and then if a user is on a larger screen \(usually signifying that they're on a computer and a proper WIFI connection, then the website will serve up larger images and extra content. This approach is called **mobile-first**, and also implies that the design for the website begins with mobile-users in mind, and then expands—as opposed to beginning a design with desktop site, and then removing elements to make it fit on a smartphone. 

One of the main ways that designers restrict content depending on screen size is by using **media-queries**—which we'll get to in a second—but a website might also present different content depending on a user's browser, location, or installed applications. 

For a terrifically weird example of what a website can detect from its users, check out [clickclickclick.click.](https://clickclickclick.click/#0ceb8962712a9ca28de290b4264c72da)

### Media Queries 





