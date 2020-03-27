# SMACSS and Responsive Web Design

- Responsive web design is the practice of building a website suitable to work on every device and every screen size, no matter how large or small, mobile or desktop. - Responsive web design is focused around providing an intuitive and gratifying experience for everyone. Desktop computer and cell phone users alike all benefit from   responsive websites.

## Responsive vs. Adaptive vs. Mobile
Responsive generally means to react quickly and positively to any change, while adaptive means to be easily modified for a new purpose or situation, such as change.
Mobile, on the other hand, generally means to build a separate website commonly on a new domain solely for mobile users

Responsive web design is broken down into three main components, including flexible layouts, media queries, and flexible media

- target ÷ context = result (relative width of the target element.)

- To use media queries, using the @media rule inside of an existing style sheet, importing a new style sheet using the @import rule, or by linking to a separate style sheet from within the HTML document (@media recommended :@media all and (min-width: 320px) and (max-width: 780px) {...})



## Viewport
 it is recommend that you use the device defaults by applying the device-height and device-width values. (<meta name="viewport" content="width=device-width">)

- One of the recommended viewport values is outlined below, using both the width and initial-scale properties.(<meta name="viewport" content="width=device-width, initial-scale=1">)

- The previously recommended viewport meta tag would look like the following @viewport rule in CSS.
- @viewport {
  width: device-width;
  zoom: 1;
}


## Flexible Media

img, video, canvas {
  max-width: 100%;
}


# Float

Float is a CSS positioning property, that makes other elemnts flow around the floated element.

 **Techniques for Clearing Floats:**
- The Easy Clearing Method
- The Overflow Method 
- The Empty Div Method



# SMACSS

It is a flexible style guide, the core of it is categorizing CSS rules.
There are five types of categories:Base,Layout,Module,State, and Theme.

**Base rules** are the defaults. They are almost exclusively single element selectors but it could include attribute selectors, pseudo-class selectors, child selectors or sibling selectors. Essentially, a base style says that wherever this element is on the page, it should look like this.

**Layout rules** divide the page into sections. Layouts hold one or more modules together.

**Modules** are the reusable, modular parts of our design. They are the callouts, the sidebar sections, the product lists and so on.

**State rules** are ways to describe how our modules or layouts will look when in a particular state. Is it hidden or expanded? Is it active or inactive? They are about describing how a module or layout looks on screens that are smaller or bigger. They are also about describing how a module might look in different views like the home page or the inside page.

Finally, **Theme rules** are similar to state rules in that they describe how modules or layouts might look. Most sites don’t require a layer of theming but it is good to be aware of it.
