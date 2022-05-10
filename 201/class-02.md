# Text, CSS, Javascript functions and loops
## Ch 2 - Text
According to chapter 2, HTML elements add basic strucutre to the content of the page. This is known as *Structural Markup*. But it can also do *Semantic Markup* which provides extra information telling the browser how to translate the information and present it to the user.

 Structural tags pointed out by the chapter:

`<h1> - <h6>` These are heading tags. Wrapping these around text impact text simlarly to `#`s in markup. 

`<p> </p>` The p-tag designates paragraphs. (block element - starts content on the next line.)

`<hr />` creates a horizontal line to break up sections of articles.

We see that these designate structure to the document/content held within the tags. 

Semantic tags such as:

`<strong> </strong>` displays text **bold**

`<em> </em>` displays text with *italics*

`<abbr> </abbr>` displays a windowed box over an acronym with the full value. LGM -> Let's Go Mets

These provide more structure information for the browser as to what it is doing in the presentation of the content. 

Now that we've read about building structure with HTML, chapter 10 was about...

## Ch 10 - Introduction to CSS

If HTML is providing structure, CSS provides presentation. This goes beyond the wireframe stucture that HTML sets in place and adds the formatting that makes the webpage look good to the user. If you think of all of your HTML elements living inside an invisible box, you can start to imagine how much influence CSS can have on your project. 

Pages 232-233 described it well with:

> CSS associates style rules with HTML elements (p-tags, h1, etc)

and

> CSS properties affect how elements are displayed

`body {`

  `background-color: blue;`

`}`

CSS can be done in three different "formats" and they have differing levels of precedence. 

External CSS is done in a separate file. It is the default location for coding CSS because it keeps your HTML clean and makes it easier to make changes to individual elements. It is the lowest level of precedence.

Internal CSS is done at the top of the HTML document, within the meta data of the site (head tags). If there is any code that conflicts with the external CSS the internal will win out. 

Inline CSS is done within the opening HTML tag and takes highest precedence, but also provides the most issues with general HTML housekeeping. 

## JavaScript Ch 2 - Basic JavaScript Instructions
<!-- put comments in your code to tell what it's doing. No one will see it...hopefully -->  

Moving on from presentation and into the function, chapter 2 of the JavaScript book talked about *Basic JavaScript Instructions*. JavaScript is full of script that tells your browser how it and the user can interact with the webpage. 

>Script - a series of instructions that a computer can follow one-by-one.

These instructions are called statements. And if you combine a bunch of statements together inside `{ }`then it is called a *code block*. These blocks of code run functions based off of variables which are stored pieces of information that the developer must declare before assigning value (numeric - 3, string, - 'three'/'3', or boolean - true/false).

The book lays out the rules for declaring variables as
- Name must start with a letter, $ , or _
- No . or - in the name
- No keywords or JavaScript reserved words
- Variables are case sensative
- Describe the kind of info stored
- multipleWordNames should capitalize the first letter of every word AFTER the first word.

If your variable has multiple values you should use an array. Arrays are a good thought if you are working with multiple values that are related to eachother. You declare the variable as normal but the values are stored in `[ ]` with commas separating the values. (Note - if utilizing string values with numeric calls the first string value is 0)

Finally the chapter discussed *Expressions* and *Operators*. 

>Expressions 'render' the values into one-single value. This can be done in two ways
    
    1 - assign a value to a variable

      `var color = 'blue';`

    2 - combine multiple values into one value

      `var area = 3*2 ;`

> Operators allow programmers to create a single value from one or more values. 

This can be done through *assignment* which strictly assigns the value, arithmetic which performs basic math and computes the value, or a string which combines two strings and puts them together.

## JavaScript Ch 4 - Decisions and Loops

Finally, Chapter 4 discussed coding a virtual representation of a flow chart. Decision points are a moment in the code where the code sets conditions 'true' and 'false'. 

Decision points have two components; an expression is evaluated returning a value of true or false. They are  followed by if/then/else/else if statements telling the script what to do.

`Set Condition`
  
  - `if true run script1`

  - `else run script2`

Some evaluating conditions include '==' equal to, '===' strict equal to (JS can be considered a weak text), '>' greater than, etc.,

Logical operators include multiple comparison operators. 

- '&&' - both

- '||' - either

- '!' - not

If elements - If condition = true run script

If else - If condition = true, run script. If = false, run other script. 

# ***Things I want to know more about***

Switch elements - I need more explanation. I understand that it sets levels for the variable and that it runs a script based off the level...but I feel like I'm not wrapping my head around it. 

<!--Finally loops check for condition, if the condition is true it runs the code block. Checks the condition again and if still true, runs the code block. Rinse and repeat. There are a few different types of loops with their own contexts. 

for loop - runs the loop a set number of times.

while loop - run as long as the condition is true.

do while - simlar to while loop, but runs the code at least once even if the condition = false.

-->