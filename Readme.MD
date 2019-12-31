# GlobalGiving Assignment

## Overview

This assignment took me 6 hours, most of which was spent referencing the style guide for the utility classes. As I progressed with components, it became quicker. The confusion I had was with what color variants were available for text and buttons. I couldn't find where this was documented, as it seems not all brand colors are applied to element colors.

My first step was to setup my project structure including copying over the provided minimized stylesheet. I didn't end up writing any new external styles. I then ran the assets through imageOptim, and converted any jpg and png files into webP. The two largest images where the benefits of webP would have been the greatest were used as background images, and I didn't have a chance to implement the solution I detailed in `Next steps`.

I created a base HTML file, and copied over the markup from the live GlobalGiving site for the navigation, header, and footer areas. I noticed I needed the styles from the homepage.css file, and added copied over those styles to the end of the minimized CSS file, so as not to create another request for this file.

From here I laid out the content of the middle sections within their own parent div, to keep a modular structure to the markup. I started with the simpler text + button sections, and got familiar with how the grid system works, and where I needed to utilize `grid-padder` vs `grid-lg-padder`.

The parts which took longer were the sections which used a background image. The need to use nested divs with padding felt like it could be improved, and could use more fine tuning for responsiveness.

## Changes made from design

- The logo grid background color was changed from `Primary 2 Light` to `Primary 2` for accessibility against the White logos.

## Next steps

- Defer the loading of the large images on the page.
- Use Modernizr to detect webP support, and create two class options on the background-image styles to use a webP image where possible.
- Use Handlebars to break up the length of this HTML and create a more modular layout.
- Create more responsive steps for the large image in the "Our approach to disaster relief and recovery" section.
- Implement a better solution on mobile for the two sections with background images.
