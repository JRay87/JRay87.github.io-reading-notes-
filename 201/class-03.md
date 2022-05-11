# Lists, Boxes, Review, and New

## ***Chapter 3 - Lists***

HTML has three different types of lists.

***Ordered lists*** display information with a numbered list. These are great for recipes, step by step directions, or ranking NL East baseball teams by wins (CAO 10May22)...

`<ol>`

  `<li> NYM 21-10`

  `<li> ATL 14-16`

  `<li> MIA 13-16`

  `<li> PHI 13-16`

  `<li> WSH 10-21`

`</ol>`


Ordered lists live within `<ol> </ol>` tags utilizing `<li>` tags for each item.

***Unordered lists*** display information with bullets, but give no numbering to the items. This is better for lists that require no ranking of value or placement of order.

**Mets Facts**

`<ul>`

  `<li> Founded in 1962, the NY Mets replaced the Dodgers and Giants who moved to California.`

  `<li> Mets have won two World Series (so far). 1969 and 1986.`

  `<li> The broadcast booth of Gary, Keith, and Ron are consistently considered the best team in baseball.`

  `<li> The Mets mascot, Mr. Met, was introduced in 1963 and is believed to be the first 'live' mascot.`

  `<li> The Mets play at Citi Field in Flushing, Queens, New York.`

`</ul>`

Unordered lists live within `<ul> </ul>` tags, again utilizing the `<li>` tags for each item.

Finally, the last type of lists are ***definition lists***. They are used to 

`<dl>`

  `<dt>Mets</dt>`

  `<dd>Short for Metropolitans, Mets means <strong>city dwellers</strong></dd>`

`</dl>`

('*Mets*' definitely sounds better in my opinion.)

Final note - lists can be nested within lists forming sublists and you can bounce between the two types. 

## ***Chapter 13 - Boxes***

If we think back to previous chapters regarding CSS we will remember that it works off the mindset that all elements within HTML are in a box. CSS can then manipulate the boxes with color and size rules that change the way the browser displays it to the user.

The boxes around these elements also allow CSS to manipulate margin, borders, padding, and the content itself. It can alter the height or width (specific size or ratio of screen), it can give a minimum height/width. We can add shading the border or round the edges.

CSS can manipulate these elements to add color, or affect the placement on the page. Remembering block v inline elements we can manipulate the flow of the content.

CSS elements can be done in three different ways, but in exterior CSS a rule might look something like this:

` art {`

  `height: 30%;`

  `min-width: 400px;`

  `margin-left: 10px;`

  `padding-top: 5px;`

   `border: 5px solid blue;`

`}`

The CSS rule above is for the Article element. It sets the height to be 30% of the browser. The width will not go lower than 400 pixels. There is a margin on the left, a padding on the top, and then a solid blue border around the whole article.

## ***JavaScript Chapter 2 review - Arrays***

Arrays are a tool used by developers to store multiple values that are related to eachother. 

Example array:

  `var colors;`

   ` colors=['White', 'Blue', 'Orange'];`

This has given the variable 'colors' as any of those colors. Quick note that due to computer numbering programming the first value is considered '0' for counting purposes. This numbering can then be used if you are trying to access or change the value, as we see below.

  `colors[0] = 'Black';`

## ***JavaScript Chapter 4 cont'd - from Switch elements***

Switch elements - I need more explanation. I understand that it decalres the variable/sets levels for the variable and that it runs a script based off the level...but I feel like I'm not wrapping my head around it. 

Loops checks the value of a condition. If the condition value is true it runs the code block. When it finishes it checks the condition again and if still true, runs the code block. Rinse and repeat. There are a few different types of loops with their own contexts. 

'for loop' - runs the loop a set number of times. 

<sub>(My attempt based on ex. p175)</sub> This code, when summoned, would display the grades received for three tests. <sub>The code will run ***for*** the amount of values in the grades array</sub>

   `var grades = [95, 76, 97];`

   `var arrayTests = grades.tests;`

   `var testNumber = 0;`

   `var msg = '';`

   `var i;`
      
`for(i = 0; i < arrayTests; i++) {`

  `testNumber = (i + 1);`

   ` msg += 'On test ' + testNumber + 'you scored:';`

   `msg += grades[i] + '<br />;`

`}`

while loop - run as long as the condition is true. Example p 176 displays multiplications table. ***While*** the condition "value of variable 'i' is less than 10" is true it will run the computation code and display the message giving the expression and sum.

`var i = 1;`

  `var msg = '';`

  `while (i < 10) {`

  `msg += i + ' x 5 = ' + (i * 5) + '<br />';`

  `i++;`

`}`  

do while - simlar to while loop, but runs the code at least once even if the condition = false. 

 This code will only display the message once because the condition "value of variable 'i' is less than 1" is false. It will always run the code at least once. 

`var i = 1;`

   `var msg = '';`

  `do {`

  `msg += i + ' x 5 = ' + (i * 5) + '<br />';`

  `i++;`

`} while (i < 1);`


<sub>example from p177</sub>