# ***Day 14** - Google's Quest to build the perfect team, Transitions and Animations*

## Google Article

Julia Rozovsky, the protagonist of the article, was a Yale Graduate and her experiences were used to ground the concepts in the article. She was assigned a study group during college that had minimal success and fell apart once the required time was over. She also had experience with an extra curricular group involved in solving business issues for competition. This group had great success as a team and remain in contact. This difference of experiences was the focus of Julia's attention after joining Google's Project Aristotle and tasked to find out: ***What makes for a successful team?***

When Julia joined Project Aristotle they reviewed previous studies and data from prior research but they could not find any specific combination of personality types or skill levels that proved the best. What they did keep coming across was research about "group norms" and this helped determine the behaviors that good teams followed, but even those could differ greatly between successful teams.

Many of the behaviors may change but what researchers from Carnegie Mellon, M.I.T., and Union College were able to determine that signs of a good team included teammates communicating in proportionate amounts ('conversational turn taking') and paid attention to the how their teammates were feeling and had high "social sensitivity". This allowed their teammates to feel safe to discuss ideas or take risks when brainstorming/working on a product. (Important skills = communication and empathy).

The article continues with Project Aristotle's presentation of their findings. At one event the team were met by Matt Sakaguchi, a midlevel manager with Google. He asked to use a survey the team had made for their research and gave it to his team. After recieving the results Mr. Sakaguchi brought his team together off site to discuss the results together. He opened up about Stage-4 Cancer which caused his team to open up about some of their own personal issues which made them more open to discussing some of their work/team issues.

The article spoke to me when it discussed how no one wants to put on a work face or have a separation between their work self and their personal self. People don't want to have to juggle different versions of themselves between work and personal time so the ability to make personal connections with teammates can help boost the success of the team. They feel safe to discuss ideas and discuss any issues which can help solve small issues before they grow into bigger issues.

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