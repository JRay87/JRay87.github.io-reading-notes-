# ***Day 14** - Transitions and Animations*

## **Transforms**

`transform` property allows modifying elements into 2D or 3D elements. The support varries between browsers and this means we have to specify all the browsers using the vendor prefixes (`-webkit-transform:`,`-moz-transform:`, `-o-transform:`) when writing the `transform` property.

**2D**

2D transforms the elements on the 2D plain. Examples of what it can do in 2D is: rotate, scale, translate ('flip'), skew. To combine them you would simply put all the desired modifications on the same line separated by spaces. Ex (from art)`transform: rotate(25deg) scale(.75)` . Combining multiple elements together can be used to simulate 3D objects in the browser.

The origin point can be moved with `transform-origin`. This moves the "center" point of the element and all future modifications are made based off the location of the new "center" point.

Perspective moves the "vanishing point" which means it makes the image look like the top of the image is farther away and the bottom of the image is closer to the user than it really is; versus the traditional straight up and down image users are used to. The depth of the perspective shift is placed inside parenthesis `transform: perspective(100px)` which will then stretch or shrink the image along the modified perspective. As with transform, perspective origin can be shifted which would have a similar shifting of the point from where changes are made to the image.

**3D**

3D is similar to 2D in that it has rotate, scale, translate, and skew. They can be combined in one line as well. 3D objects will have a backface (underside) of the element which can be rendered invisible using `backface-visibility: hidden;`. Combining multiple 3D elements into eachother can be used to make 3D animations with the elements.


## Transitions & Animations

**Transitions**

*For an element to have a transition it must have a change in state and different styles must be used for each state.* This can change colors, border-radius, height, width, visibility, or a multitude of other options. You can change the time it takes for the transition to happen with the `transition-timing-function:` this can be `linear`(same pace), `ease-in`(starts slow gets faster), `ease-out`, or `ease-in-out`. Can have the transition delayed as well.

**Animations**

Animations can handle multiple stages in a transition or multiple points of importance within the animation timeline. *Using the `keyframes` rule and the name, any breakpoints, and the properties needing to be animated* you can create animations within your website elements. The timing and speed can be modified as well as how often they would be repeated (`animation-iteration-count`). They can be reversed with `animation-direction: alternate;`


## ***8 Simple CSS3 Transitions that will wow your users***

This article showed how simple it was to make good looking animations on your website. 

'Fade in' made the element opacity increase. (0.5 -> 1)

'Change Color' changed the color from its initial css value to a new designated color. (Blue -> Orange)

'Grow/Shrink' (must have the vendor prefixes) grows or shrinks the element size

'Rotate' rotates the image (using the vendor prefixes) `rotateZ()`putting the desired degrees in the parenthesis

'Square to Circle' transforms the element shape with `border-radius:50%;`

'3D Shadow' gives a `box-shadow` to the element making it appear 3D

'Swing' makes the element shake left and right within parent element

'Inset Border' a border appears within the element box. `box-shadow: inset 0 0 0 25px #53a7ea;`


## Assorted Animations

Other ideas / code for other animations