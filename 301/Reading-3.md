# ***Day 3** - DAY 3 TITLE*

## ***React Docs** - [lists and keys](https://reactjs.org/docs/lists-and-keys.html)*

### Utilizing listItems will be important for displaying arrays through React (which can be done with the `map()` function). Keys are used to stabilize the id's of the values. These are important concepts to understand when working with React and JSX

### What does .map() return?

`.map()` returns an array of the data passed to it, which can be modified/displayed etc.,.

### If I want to loop through an array and display each value in JSX, how do I do that in React? 

Using the `map()` function and curly braces `{ }` we can then assign the values in the array to **list items.**

### Each list item needs a unique _____

Key. ("a special string attribute you need to include when creating lists of elements" - from article). Keys must be unique within their array, not necessary to make globally unique keys.

### What is the purpose of a key?

Keys help React keep track of when/how items have been modified or deleted. This gives the elements "a stable identity"(from the article)

## ***How to use the Spread Operator** - Dr. Derek Austin*

### Understanding how spread can be used to modify multiple arrays can be used to take smaller pieces of code and data to build your website through components, and can also be used to keep track of the data within the arrays.

### What is the spread operator?

`...` this piece of code is used to "spread" the array into seperate arguments (values). This can be useful for many reasons.

### List 4 things that the spread operator can do

After the spread function spreads the arguments of the array these values can be used to 1) Copy the array, 2) Use Math functions, 3) combining objects, 4) adding an item to a list, and many more.

### Give an example of using the spread operator to combine two arrays

`const startingRotation = ['deGrom','Scherzer','Bassitt','Carrasco','Walker','Megill']`

`const bullpen = ['Peterson','Williams','Reed','Holderman','Shreve','Rodriguez','Smith','May','Ottavino','Lugo','Diaz']`

`const metsPitchingDepth = [...startingRotation,...bullpen]`

`console.log(...metsPitchingDepth)`

This example uses the spread operator to combine the array 'startingRotation' and 'bullpen' in the 'metsPitchingDepth' array.

### Give an example of using the spread operator to add a new item to an array

`const oldStartingRotation = ['deGrom','Carrasco','Walker','Megill']`

`const newStartingRotation = ['Scherzer','Bassitt',...oldStartingRotation]`

`console.log(newStartingRotation)`

This example takes the array 'oldStartingRotation' and adds it to the array 'newStartingRotation' using the spread operator

### Give an example of using the spread operator to combine two objects into one

`const objMets = {mets: "rule"}`

`const objYankees = {yankees: "drool"}`

`const baseball = {...mets,...yankees}`

`console.log(baseball)` --> logs Object{mets: "rule", yankees: "drool"}

## How to Pass Functions Between Components

### Understanding how functions can be passed and called in new objects/components can help build efficient dry code and helps speed up the development process.

### In the video, what is the first step that the developer does to pass functions between components?

To pass functions between components the developer initially created an element in the object that is accessed in the new component. Then it is called in the child component.

### In your own words, what does the increment function do?

The increment function takes the value of the state and adds one to the value of the state.

### How can you pass a method from a parent component into a child component?

Create an reference to the function within the object that is accessed by the new component. Then in the new object you can use `referencedFunction={this.referencedFunction}` (using whatever name you want, just make sure to remember your naming scheme)

### How does the child component invoke a method that was passed to it from a parent component?

it calls is using `this.props.referencedFunction(this.props.anyPassedArguments)`

## Things I want to know more about

What is the purpose of using spread when simply combining two arrays? I know it is faster than parsing, pushing, etc., but if we simply are combining the data is it necessary to break them down into their individual values?
