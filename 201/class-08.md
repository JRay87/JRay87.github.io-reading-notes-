# ***CSS 2**- The Re-designing*

This day's readings are mainly review from previous lessons on CSS, but there was still important imformation I was able to pull out of them. 

## Article - Layout
Originally released in 1996 CSS has had 3 official named updates and 6 updated feature releases inbetween 1996 and 2021.

There was a reminder of the box around elements with margin, padding, etc.,

There are two layout mechanisms in CSS *'flexbox'* and *'grid'*.

***Flexbox*** put elements in one dimension (either horizontal or vertical.Defaults to inline.) The elements will stay on the same axis and not wrap. Converts its child elements to flex items (*behavior can be changed in the container*).

***Grid*** controls elements in multiple dimensions. Groups elements together and can create grids.

Other layouts include:

***Inline block*** - displays content in a box with some characteristics of block-level, but still flows inline with the text.

***Float*** - Tells the element to float in the specified area and content wraps around it.

***Multicolumn*** - Splits long columns into multiple columns to help with layout.

***Position*** - *changes how an element behaves in the normal flow of the document, and how it relates to other elements* (relative, absolute, fixed, sticky, static)

## HTML Chapter 15 - Layout

Elements in HTML live within an invisible box that can be manipulateded by the developer to change the browser's presentation to the user. These blocks can have different types of positioning:

 Normal(block elements start content on new lines)
 
 Relative(shifts content to desired side of the box)
 
 Absolute(stays in place while content moves during mouse scroll)
 
 Fixed(combines relative and absolute)
 
 Floating(fixes an element to a side and the other content flow around it)

 Child elements will inherit the parent element rules.

 Layouts can be *fixed* (use pixel values to state size) or *liquid* (uses percentages to scale content to size of browser window)

 link style sheets to your html to have the browser display the desired formatting rules