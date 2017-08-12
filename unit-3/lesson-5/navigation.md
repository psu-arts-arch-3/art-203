![](blob:https://www.gitbook.com/769d4130-a6b8-4c1a-bded-728a8f6e7e54)

If you watched Lynda's Muse Essential Training, you got a glimpse of how Muse handles site navigation. We'll eventually build our final sites in Muse, so you'll return to this screen, but it's also a nice visualization of how any site is laid out. This "roadmap" shows the **top level pages**\(featured in the **navigation menu **at the top of each page\), with **children pages **nested below.

You're probably familiar with this layout from a lifetime browsing the web. But it's important to plan out the content of your site efficiently, and avoid having too many pages. Make sure that the content is laid out in a logical way, so users don't have any trouble finding information.

Here's a sample hierarchy of pages:

* About
* Store
  * Shirts
  * Pants
  * Shoes
    * Boots
    * Sneakers
* Contact
* Support
  * FAQ
  * Contact

The design of children pages could be identical or unique. In this example, the children pages below "Store" would probably look identical expect for**metadata**like the item's name, cost, description, and an image. However the children pages below Support might look different... "FAQ" would probably have a big list of questions that users can click on, while "Contact" would have some sort of web form that users could fill out.

With a Content Management System \(CMS\) like Wordpress, you can just design a single page for "Store items" and let Wordpress dynamically fill in the metadata. Since Muse only makes static websites, you'll have to manually copy and paste the page and type in the metadata for items like this.

Some navigation menus also show children pages in a submenu when you hover over the relevant parent page. This helps users go directly to the page they want without having to load interstitial pages, but it can be unwieldy if you have a lot of pages.

![](blob:https://www.gitbook.com/30b0a91b-ec0a-4e01-bb49-0e68670dcfe5)

This chaotic**flyout**submenu has some glitchy behavior, but the sheer number of pages is overwhelming and certainly doesn't make it easy for Pennsylvania residents to file their taxes.

### Navigation Menus

Some quick thoughts on navigation menus, which we haven't talked about much yet, because we've focused on one-page websites. "Nav" menus are pretty self-explanatory, but you'll have to make a few decisions as you imagine your site layouts:

**Horizontal or vertical?**

* Most sites arrange navigation links in a horizontal row at the top of the page, but you will also see sites stack the links in a vertical column, usually located on the left side of the screen.
* Vertical nav menus make it easier to add more links in the future
* Most people scan websites from top to bottom, and are less likely to look at side navigation menus.
* Here's an interesting article from
  [Smashing Magazine](https://www.gitbook.com/book/psu-arts-arch/dart-203/edit#)
  on the debate, that argues for horizontal menus but still identifies some effective uses of vertical menus.

![](blob:https://www.gitbook.com/36ad2e9f-f01b-4a6e-a3cf-b1b693fc07c9)

**Static or fixed?**

* The default behavior of any HTML element is to sit in the document flow and allow the user to scroll up and down \(or left and right\).
* Elements like nav menus can be "fixed" in place, so they remain visible as the user scrolls through the page.
* This is accomplished with the CSS property
  `position: fixed;`

**Top or bottom?**

* Almost all sites put their nav menus at the top, for the reason mentioned above, that people scan websites from top to bottom.
* Some sites put the menu at the bottom for a unique effect. This forces users to look at your content before they even consider going to another page.

**Mobile behavior?**

* Unless a site only has a few top level pages, the nav menu will need to adapt to fit on smaller screens.
* The typical solution is to use an icon \(three horizontal lines a.k.a. a "hamburger"\) to show/hide the nav menu.
* Here are some
  [alternative methods](https://www.gitbook.com/book/psu-arts-arch/dart-203/edit#)
  for mobile nav menus, and some reasons to
  [consider hamburger alternatives](https://www.gitbook.com/book/psu-arts-arch/dart-203/edit#)
  .

![](blob:https://www.gitbook.com/496732b6-fd03-4d23-8aca-69630f8650bc)

