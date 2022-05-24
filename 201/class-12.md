# ***ChArticles***

## ***Article 1** - Chart.JS - Sara Vieira*

Charts are great ways to display lots of information in small areas. It relies on visual representation of data.

First you create a canvas element, setting the width and height of the canvas. From there you need to code in access to the canvas for your javascript (put it in the footer). Also include chart, line, bar, etc., and the variables. 

Then in JavaScript you access the variable from before and can code in the display properties you are wanting to show.

In a line chart you put the points in an array for the chart to pull from. A Pie chart has each value coded separately for individual variable display control; bar charts have the data points in an array under the desired display style.



## ***Article 2** - Creating a Chart (chart.js)*

This article was a great example of producing a bar chart. Using six values in the 'data' array they coded six bars to visually represent the data on the screen.


## ***Article 3** - Basic Use of Canvas*

The canvas element is a tag which denotes a blank space on the page where tables/videos/charts can be added. The chart tag includes the id, width, and height in the opening tag to determine the size. (Canvas tags require closing tags.)

Canvas tags are signs that the source of the media will be in Javascript and that you will need a window to the DOM in your JavaScript. Includes `getElementById`, and `getContext` for the fallback media.

## ***Article 4** - Drawing Shapes with Canvas*

Canvas elements only support drawing rectangles and paths but this can be accomplished by putting the type of rectangle, its starting coordinates, and the dimensions. Types of rectangles are filled (`.fillrect`), stroke (just the outline of the square with no fill), and clear (makes the specified area transparent).

Paths are *"a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and shape."*(article). These paths can be combined into shapes with some extra coding. `beginPath()` starts the path, `closePath()` draws a straight line from the end of the current subpath to the original path. `stroke` and `fill` are then used to add border and color to the shape. One other useful tip/trick was the `moveTo(x, y)` method which moves the "pen" to a new location without making a line.

Other useful methods were arcs and bezier/quadratic curves which can be used to make more complex shapes and elaborate designs for your page.

## ***Article 5** - Applying Styles and Colors*

This article discussed more CSS color and style options. Opening with `fillStyle` which modified the color inside the element and the `strokeStyle` which is the style for the outline.

Both styles can have equations to fill a gradient of colors within the element adding for extra pop. The developer can also modify the transparency (globalAplha can be used for overlapping elements).

Line visualizations can be modified with different properties including: `lineWidth`, `lineCap`(end of lines), `lineJoin`(for corners of lines that meet but do not intersect(?)), miterLimit (thickness of intersection of lines), and many more. 

Gradients can be used as a line as with `createLinearGradient` (needing the starting and ending coordinates), `createRadialGradient` (needing the starting point, radius 1, end points, radius 2), and `createConicGradient` (simple needs the angle of the cone and the x,y position of the angle)

Patterns - `repeat`, `repeat-x`, `repeat-y` repeats the image along both, only horizontal, and only vertical planes.

## ***Article 6** - Drawing Text*

Canvas also alows the developer to draw text on the element. `fillText(text, x, y, [, maxwidth])`-*from article* draws the text supplied in the 'text' value, starting at the x,y coordinates with a max width of whatever the developer supplies.

`strokeText` does the same but with only the outline of the letter (no fill)

The text can be modified from there with `font = value` value  designating the font used and its size. `textAlign` will align the text within the canvas element. `textBaseline` modifies the baseline of the font. Finally `direction` impacts the directionality of the text.
