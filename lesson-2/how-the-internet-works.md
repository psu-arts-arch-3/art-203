Are you the kind of person who knows every component of a modern computer or smartphone, or do you just accept that your devices work "by magic" and just use them instinctually. What about cars? Refrigerators? Cellular networks? With the ever expanding scope of technology, the challenge of understanding how it all works is an existential dilemma for today's society.

So, how does the Internet work?

...

Got an answer? If you're going to be creating content for the web, it's a good idea to have at least a basic grasp of what's happening behind the scenes.

**The Internet** \(derived from "internetwork"\) is a global network of networks that facilitates the transfer of data. The **World Wide Web \(WWW\)** is a public information space that relies on the infrastructure of the Internet to share content. This means that while most people use the terms interchangeably, the Internet and the Web are not the same thing. Think of the Web as a portion of content that is transferred over the infrastructure of the Internet; email, file-sharing, and mobile apps also transfer data through the Internet, but the do not constitute parts of the Web \(i.e. websites\).

In 2016 the Associated Press and New York Times [updated their style guides](https://www.nytimes.com/2016/06/02/insider/now-it-is-official-the-internet-is-over.html) to spell Internet with a lowercase "i" as more and more people refer to it colloquially and not as a proper noun—but either is acceptable.

### HTTP & HTML

Like most computer programs, webpages can be completely reduced to text \(i.e. code\), which is how content is transferred online. **Web browsers** like Chrome, Firefox, Safari, and Edge render those text files as webpages to create the visually compelling experiences you're used to seeing online. If you want to see what the raw text version of a web page looks like, try to following on any website:

Right-click on an empty portion of the web page \(not on text or images\), and select View Page Source \(Chrome or Firefox\) or Show Page Source \(Safari\).

Go ahead and try it.

...

Back now? Okay. In order to take that code and render it consistently on any device, anywhere in the world, webpages are built and shared within a set framework called **HyperText Transfer Protocol \(HTTP\)**. HyperText refers to interconnected content that can be linked together via [hyperlinks,](https://en.wikipedia.org/wiki/Hyperlink) but let's not get too technical.

The actual content that is transferred via HTTP over the Internet are typically text files written in **HyperText Markup Language \(HTML\)**, although some websites use a different coding language \(PHP or Java\) to create web pages, the end product is HTML.

Web browsers can read other types of files too, for example, you can open a JPEG in your web browser. You should try this too.

1. Right-click on an image file anywhere on your computer.
2. Choose "Open with", and choose a web browser like Chrome or Firefox. Alternatively you can drag it onto the icon in the doc if you're on a Mac.

If you need an image file, you can download the image below of the first web browser with a graphical interface  \([Mosaic, from 1993](https://en.wikipedia.org/wiki/Mosaic_%28web_browser%29)\).

**Consider: **Does Mosaic look similar or different from your current web browser? What are some of the design details that have stuck around for 20+ years?

![](/assets/lesson-2/Mosaic.png)

Once you've opened a JPEG or PNG in your web browser, take a look at the URL bar at the top of the screen.

Instead of the traditional "[http://www](http://www)..." you should see something like the following:

![](/assets/lesson-2/local-file.png)

This is the **path** for whatever file you opened. The slashes denote folders, meaning that my file "Mosaic.png" is located in my Documents folder, within my user folder, within a folder called "Users", which is at the root level folder of my computer's hard drive.

If you haven't done any sort of coding before, this might blow your mind, but any URL you type into your web browser is the same sort of file path—except the files you're opening are usually HTML files \(e.g. "http://some-website.com/some-file.html"\) and not JPEG's. So when you go to [http://www.worldcampus.psu.edu/about-us/mission](http://www.worldcampus.psu.edu/about-us/mission) you're accessing a file called "mission" within a folder called "about-us." Sometimes the file extension will be hidden by the browser, but oftentimes you will see URL's ending in ".html"

Unlike the image you opened earlier, webpages are not saved on your local computer; they're saved on a computer somewhere else on the planet. These computers are called **servers,** and they're built specifically to host files and make them accessible over the Internet. Here's a giant server center depicted on the show _Silicon Valley_:

![](/assets/lesson-2/silicon valley.png)

We'll get into the details of how to upload files to and from a remote server soon, but for now just appreciate the fact that every page you visit online is a portal into a computer somewhere else in the world.

It's entirely possible to create HTML files on your local computer and view them in a web browser.

In fact, that's what we're going to do in this lesson.

