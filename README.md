[![General Assembly Logo](https://camo.githubusercontent.com/1a91b05b8f4d44b5bbfb83abac2b0996d8e26c92/687474703a2f2f692e696d6775722e636f6d2f6b6538555354712e706e67)](https://generalassemb.ly/education/web-development-immersive)

# HTML-CSS Portfolio Lab

In this lab, you'll be building a personal website to share with your peers.

We will be using the following mockup to build out our website:

<img src="https://media.git.generalassemb.ly/user/16103/files/652cef80-3f2e-11e9-80cb-480c79b47682" alt="portfolio mockup" width="400"/>

## Installation

1. Fork and clone this repository.
2. Change into the new directory.
1. Install dependencies with `npm install`.
2. Create and checkout a new branch, named `development`.
3. Follow the directions below.
4. When finished, push to your fork.

## Best Practices: UI / Accessibility

Many website users have various disabilities and are neurodiverse. There are
many easy decisions you can make about your HTML and CSS that will help people
use your website, and these tips will also create a website that is easy to use
for everyone.

- Use HTML5 elements - not just divs!
- Use high contrast between backgrounds and text.
- Caption your images in a relevant way.
- Don't use color or sound alone to show what an element does.
- Organize content with headings and subheadings.

## Debugging CSS

The best way to debug anything is to be _methodical_. This includes CSS! If your
elements are not behaving as you expect, here are the first steps. More
information about debugging CSS is in the additional resources section below.

- Make sure your class names are exactly the same in HTML and CSS.
- Double check that your selectors are selecting the correct element.
- Do not ADD MORE to things that aren't working. Take out the code that doesn't
work before adding something else.

## Browser Template

At this point, it is probably helpful to introduce you to the Browser Template
that you will be using in many of your projects. There may be a few things
happening in here that you're not familiar with (and that's okay), but the most
important thing to understand about the Browser Template is how it is
structured in order to add styles to your HTML.

I know we just showed you three distinct ways to add CSS to a page, but things
are done a little bit differently in the Browser Template. This repo actually
relies on said template, so let's take a look at how we would add styling to
the example HTML page within. (Note, we will have to use `grunt serve` in order
to view this page in our browser). `grunt serve` spins up a local server via
Grunt. This local server allows us to work in a 'Development' environment
to replicate what the 'Deployed' environment will be like.

## Instructions

### Developing Content

For this assignment, you'll be writing about yourself, so there's no starter
text. Don't worry, you only need to create the following:

- A headline for your webpage.
- A brief introduction of 2 - 3 sentences about yourself.
- A short description of what you do at work. Again, 2 - 3 sentences is fine.
- A short introduction and list of your favorite pastimes.

If you don't know what you want to say quite yet - don't worry! Developers
and designers often use things like [lorum ipsem](http://www.lipsum.com/) as
content placeholders.

There are also image versions like [picsum](https://picsum.photos/).

### Structuring Your Content

#### Semantic Page Structure

Once you have your content prepared, you'll need to add it to your html page.

1. Start by sectioning off the page with the `header`, `main` and `footer`
sections in the page body.

Here we are focused on using semantic html elements to separate out our content.

#### Header Section

2. Add your headline to the `header` section and wrap it in an appropriate tag
(you'll want this to be the largest one on the page).

3. Add your introductory paragraph to the `header` (it's a paragraph, so use
the appropriate tag).

4. Next, add your `nav` tags in the `header`.

5. Inside the `nav`, add an anchor tag for each of our main sections: work,
hobbies, gallery. We'll be using ids with the same names, so go ahead and
add the href attributes for them (remember that the name of the id is
preceeded by a `#`).

#### Main Section

Our main content needs to be broken down into 3 sections, each with an id
corresponding to the links above. Use an appropriate tag for each section 😉.

6. Inside the work section, add your _heading_ (this should be smaller than the
one used previously for your headline), followed by the _paragraph_ you
wrote about what you do for work.

7. You'll want to wrap this heading and paragraph inside a single `div` so that
you can set the work section in columns later and keep these elements together
in one column.

8. Add an image that represents you at work. This could be a logo from your
company website. Do you remember how to get an image from a website with
the right-click?

9. Do the same for the hobbies section, adding a heading, intro paragraph and a
list of your hobbies. Remember to wrap them all in a `div`.

10. Finally, use what you learned about adding content images with the `img` tag
and insert all of your pictures into the gallery section.

#### Footer Section

The footer section is simple.

11. Just add a paragraph that reads: "Get in touch!" and follow it with a `nav`.

12. Inside the `nav`, create an anchor tag for an email address (you can make a
fake one if you're concerned about privacy) and one other for your linkedin
page.

### STYLING YOUR WEBSITE

Find the `index.scss` file in `assets/styles`.

#### Base Styles

13. Then, go to [fonts.google.com](https://fonts.google.com) and search for
and add the 'Raleway' font you like in the weights of 200, 500, and 900.

14. Inside your style file, add the universal selector and set the box-sizing to
border-box and remove all of the margins.

We're going to set some base styles that will apply to the whole page.
That means we want to use the `html` element as the selector.

15. Set the page background to `#343434`.
16. Set the color of the font to `#16b1b5`.
17. Set the font family for the page to `'Raleway', sans-serif`.
18. Set the font weight to 200.
19. Increase the base font size to 24px.
20. Give our page smooth scrolling.

#### Header Styles

21. Give the header `40px` of padding.

22. Set the line-height for your headline to `.8`.

23. Add `1em` of margin to the top and bottom of the paragraphs since we removed
all margins before.

24. We need to add some padding to the nav element to address a special
phenomenon called margin collapse, which you'll be reading about next week.
So give the nav `1em` of top and bottom padding. Also, decrease the font-size
for the nav elements to `16px` and center them.

25. Finally, to style our links, change the color to white. Add `20px` of margin
and padding. Transform the case to uppercase. Remove the underline. Add a `1px`
solid border.

#### Main Section

26. Give the work section a background-color of `#16b1b5`, padding of `40px`
and set the font color to white. We also need to set the column-count on
this one to 2 columns.

27. The hobbies section needs padding of `40px` too.

28. Our gallery is going to get a column count of 3 and we're going to remove
the column gap by setting it to 0. Set the background color on the gallery
to `#16b1b5` like the work section.

29. We used divs to wrap our column contents so that we can use the special
break-inside: avoid, to keep the div contents together in one column.

30. Lastly, to keep our images in check, we need to set them to width 100%.
Also, if you want to remove the space below each image, you can add a property
to the img of display: block;. We'll be talking about this next week.

#### Footer

31. Set the footer to center its text (inline) elements. The nav is
already receiving the styles from the nav in the header!

### Final Form

Congratulations! You now have a beautifully designed website all about you!

You can use all of the tools at your disposal to expand on this website,
maybe even deploy it for all the world to see.

Hopefully your website looks something like the following:

<img src="https://media.git.generalassemb.ly/user/16103/files/20ee1f00-3f2f-11e9-86f9-b13a6ef7352c" alt="portfolio website example" width="400"/>

There is more information below about the structure of this repo do you choose
to build on this lab.

----

## Structure

### Styles

Developers should store styles in [`assets/styles`](assets/styles) and load them
from [`assets/styles/index.scss`](assets/styles/index.scss). Bootstrap version 3 is
included in this template.

## Adding Images

To add images to your project, you must store them in the `public` directory.
To use the image in HTML or CSS, write the path to the image like this:

```html
<img src="public/cat.jpg">
```
or
```css
#my-cool-div {
  background-image: url('public/cat.jpg')
}
```

Note that there's no `./` or `/` in front of `public/filename.jpg`.

## Adding Fonts

To add custom fonts to your app, you can either use a CDN like Google Fonts, or
you can download the fonts and save them in the `public` directory. If you use
the former method, follow the directions on the website providing the fonts.

For local fonts, put the files in `public`, and then import and use them in a
`.scss` file like this:

```scss
@font-face {
  font-family: 'Nature Beauty';
  src: url('public/Nature-Beauty.ttf') format('truetype');
}

.element-with-custom-font {
  font-family: 'Nature Beauty';
}
```

## Tasks

Developers should run these often!

- `grunt nag` or just `grunt`: runs code quality analysis tools on your code
    and complains
- `grunt make-standard`: reformats all your code in the JavaScript Standard Style
- `grunt <server|serve|s>`: generates bundles, watches, and livereloads
- `grunt build`: place bundled styles and scripts where `index.html` can find
    them
- `grunt deploy`: builds and deploys master branch

## Additional Resources

Here are some sites you might want to bookmark, if you haven't already.

- [HTML5 Element Flowchart](http://html5doctor.com/lets-talk-about-semantics/)
- [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [CSS-Tricks](https://css-tricks.com)
- [Using the browser to debug CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS/Debugging_CSS)

## [License](LICENSE)

1. All content is licensed under a CC­BY­NC­SA 4.0 license.
1. All software code is licensed under GNU GPLv3. For commercial use or
    alternative licensing, please contact legal@ga.co.
