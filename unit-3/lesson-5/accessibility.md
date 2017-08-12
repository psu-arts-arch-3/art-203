As students develop their final websites, we need to consider some new aspects of web design. The previous websites we've made have been largely experimental "art websites"—for this final project, students will create professional business-friendly websites. In order to design with the full experience in mind \(UX\) we need to spend some time on accessibility and search engine optimization \(SEO\).

## Accessibility

Every user who encounters your site will have a unique perspective. We've talked about responsive design concepts, and how websites need to account for a variety of devices, but designers also need to account for different browsers, languages, and disabilities.

[Accessibility](https://www.w3.org/standards/webdesign/accessibility) usually refers to making content accessible to people with disabilities, but it's really part of the overall design process. Considering how your site will be understood by different users will force you to consider the overall user experience and think critically about your initial ideas.

The World Wide Web Consortium \(W3C\) has some good information about accessibility, highlighting that the access to information and communication technology is a basic human right as guaranteed by the United Nations. These concerns become very important for large websites and business who become liable for legal action if they fail to make their websites sufficiently accessible.

The following Lynda videos provide a great introduction to accessible design, and provides some nice case studies of specific websites.

#### **Lynda Course**:[ UX Foundations: Accessibility ](https://www.lynda.com/Accessibility-tutorials/Foundations-UX-Accessibility/435008-2.html)

**Required videos:**

* Ch.1 What is Accessibility?
* Ch.2  Accessibility by Example?
* Ch 5. Integrating Accessibility into your UX Work and Process

After watching the videos above, let's review some of the essential ways to make your websites accessible.

#### **Alternative text \(a.k.a. alt text\)**

In HTML you can include metadata for any image, including alt text:`<img src="path-to-image/bunny.jpg" alt="A fuzzy bunny">`

Alt text will be displayed if the image can't be loaded for any reason, or if users sets their browser to not load images \(potentially to save data\). But for the purposes of accessibility, a user with impaired vision might use a text-to-speech program \(called a **screen reader**\) to read the text of a web page aloud—if you don't set alt text, they won't get the full experience of your design and could miss vital information.

#### Image Use

Because some users might not see your image files, you should avoid including vital information in images. Rather than inserting a JPEG image of a button...

![](/assets/lesson-5/submit-button.png)it would be better to create a `<div>` with a text element and add the color and decoration with CSS. Muse makes this process easy, and this also applies to things like logos and site names. Text is much more versatile than images.

#### Color Use

There are various color deficiencies that could impact the accessibility of a website. One of the most common types of color blindness is the inability to distinguish red and green... which also happen to be the colors most commonly used to denote success/failure. If your website has a submission form or other input feedback, make sure that your success/failure messages include text or images besides color.

#### Keyboard Input

Some people cannot use a mouse or trackpad, instead relying on the keyboard for navigation. You may not have experimented with this, but try using the tab, enter, and arrow keys to navigate a website \(Pro Tip: Shift+Tab is also useful\). Most browsers and development platforms will include some level of keyboard support automatically, but keep this in mind if you're considering any  UI inputs that require unique cursor action.

#### Transcripts

More text! If you have audio or video elements, make sure to include full transcripts or enough text to guide through the experience.

## Search Engine Optimization

SEO might seem like a strange thing to include on the same page as accessibility, but there are some connections between the two, and by making your website accessible you're also making it easier for search engines to analyze... so there's even more incentive to follow these guidelines.

SEO and accessibility both revolve around an attention to detail and following standards adopted by web designers everywhere. Similar to accessibility, optimizing your site for search engines involves following some guidelines and considering the eventual uses throughout the entire design process—except these users aren't human.

Once again text is essential. Computers can't tell a JPEG of a bunny from one of a motorcycle—unless they're powered by a powerful machine learning algorithm. You can upload images to Google's [Cloud Vision](https://cloud.google.com/vision/) to test it's image recognition abilities. But it's much easier for algorithms to analyze text, so it's important to include as much descriptive text as possible throughout your sites.

There are bunch of Lynda videos about SEO—including [The 17 Minute SEO](https://www.lynda.com/Marketing-tutorials/17-minute-SEO/151545/415814-4.html) primer—but this stuff gets pretty advanced, so let's just cover some basics.

#### Good Content

Google has pretty sophisticated page-ranking algorithms at this point, and the best way to get your site to show up in search results is to publish original and unique content, and to keep publishing things to give the impression of an active site. An original name helps; if your business and website are called "John's Barbecue" is going to be tough to beat out the hundreds of similar websites, but it's possible if your content is the best. An easier route would be to call it something more unique.

Add descriptive text too, even if it seems redundant or obvious. Make sure important keywords related to your site actually appear in the text.

#### Mobile Compatibility

In it's quest to serve up the best websites, Google gives advantages to sites that are mobile friendly. We've previously covered  good approaches to responsive design, but if you're ever unsure, you can submit your URL to Google's [Mobile-Friendly Test](https://search.google.com/test/mobile-friendly) and receive feedback on how to improve your design. It's also always a good idea to test the site out on a mobile device yourself!

#### Speed

Google also favors sites that load fast. You can check Google's [PageSpeed Insight](https://developers.google.com/speed/pagespeed/insights/) for a rating of your site's performance and suggestions for improvement. Some of the fixes are going to be more useful to a developer who is coding their own site, but it still might reveal some insights. But test the site yourself, and if its loading speed doesn't bother you, you're probably okay for now.

#### Optimization

This is a big component of making your site load quickly. Text takes up much, much less memory than images or videos.

For images, if you're using a vector image created in Illustrator, the best solution is to save it as an SVG for use in web design. SVG's take up very little memory, but are best for simple artwork with flat colors. If you need to make your SVG's even smaller, you can upload them to[ SVGOMG ](https://jakearchibald.github.io/svgomg/)and download a compressed version.

If you're working with photos, you'll have to save iamges as JPEG's. The best approach is to take a trip through Photoshop. Use "File &gt;&gt;&gt; Export &gt;&gt;&gt; Save for Web" to compress raster images, and adjust the "quality" setting as low as you can go without sacrificing the too much image quality \(I usually set the quality to 60\). You can watch a tutorial about this in the Lynda course: Photoshop CC for Web Design, Ch. 8, [Optimizing individual images](https://www.lynda.com/Photoshop-tutorials/Optimizing-individual-images/145211/166635-4.html?autoplay=true).

For raster images \(JPEG's and PNG's\) you should also check the image dimensions, as this can make a \_huge \_impact in the size of your file. If your image is 1920px wide but it's only displayed at 400px in your website, you can resize it in Photoshop \(Image &gt;&gt;&gt; Image Size\) to optimize your file size. For example, an image straight out of your camera might be 4000px wide and take up 4MB but an optimized web version could be 1000px wide and only take up 200kB \(that's twenty times smaller\).

#### Alt Text

Remember alt text? It helps Google know what your images are showing! If your site has a bunch of pictures of coffee, but doesn't use the word "coffee" in enough of the site's text, you won't be ranked highly in searches for your favorite caffeinated beverage.

#### File naming

Hopefully you've been keeping your files organized all semester and using descriptive file names without any spaces—but if you haven't, know that it will hurt your SEO. This is important for images... make sure you use descriptive file names like "bunny-drinking-coffee.jpg" instead of "IMG\_07120417."

Also make sure to use descriptive names for your actual web pages. If the contact page isn't called "contact.html" or something similar, it might not turn up when people search for it.

