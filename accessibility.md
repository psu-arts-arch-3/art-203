As students develop their final websites, we need to consider some new aspects of web design. The previous websites we've made have been largely experimental "art websites"—for this final project, students will create professional business-friendly websites. In order to design with the full experience in mind \(UX\) we need to spend some time on accessibility and search engine optimization \(SEO\).

### Accessibility 

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

In HTML you can include metadata for any image, including alt text:` <img src="path-to-image/bunny.jpg" alt="A fuzzy bunny">`

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



### Search Engine Optimization  

SEO might seem like a strange thing to include on the same page as accessibility, but there are some connections between the two, and by making your website accessible you're also making it easier for search engines to analyze... so there's even more incentive to follow these guidelines. 

SEO and accessibility both revolve around an attention to detail and following standards adopted by web designers everywhere. Similar to accessibility, optimizing your site for search engines involves following some guidelines and considering the eventual uses throughout the entire design process—except these users aren't human. 

Once again text is essential. Computers can't tell a JPEG of a bunny from one of a motorcycle—unless they're powered by a powerful machine learning algorithm. You can upload images to Google's [Cloud Vision](https://cloud.google.com/vision/) to test it's image recognition abilities. But it's much easier for algorithms to analyze text, so it's important to include as much descriptive text as possible throughout your sites. 

There are bunch of Lynda videos about SEO—including [The 17 Minute SEO](https://www.lynda.com/Marketing-tutorials/17-minute-SEO/151545/415814-4.html) primer—but this stuff gets pretty advanced, so let's just cover some basics.

Mobile Compatibility

Google's [Mobile-Friendly Test](https://search.google.com/test/mobile-friendly)

Speed

Google's [PageSpeed Insight](https://developers.google.com/speed/pagespeed/insights/)

File naming and URL

Organization

