# Day 5 - Thinking in React and Higher-Order Functions

## [Thinking in React](https://reactjs.org/docs/thinking-in-react.html)


### What is the single responsibility principle and how does it apply to components?

A component should only do one thing; if the component starts to handle multiple facets it should be broken down into smaller pieces.

### What does it mean to build a ‘static’ version of your application?

Building a static version of your website means to build one with the structure and user interface but without the functionality. When building a static version pass data down through props as state dentoes interactivity. 

### Once you have a static application, what do you need to add?

After you have built the static version of your application then you begin to add data through `state`

### What are the three questions you can ask to determine if something is state?

1) Is it passed down from a parent element?

2) Does it change in value?

3) Can you use any other state or props to get this piece of data?

(If the answer to any of these questions is yes, it isn't state.)

### How can you identify where state needs to live?

To identify where state needs to live, find all the components that render something based on the state value. Then find a common parent component to store the value. This is so all the children components can have this data accessable. 

## [Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)


### What is a “higher-order function”?

A higher-order function is one that 'operates' on other functions. These can create or make changes to other functions.

### Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

Line 2 is telling the greaterThan function to return values of m that are greater than n.

### Explain how either map or reduce operates, with regards to higher-order functions.

map operates on another function by taking in an array of data and modifying each value in the array through an expression that is passed through the map arguments. Adding + 2 to all the numbers or placing a message/characters before or after each string value.

reduce operates by taking in the data and creating a new value that has each of the values from the array added together one by one. `arr = [1,2,3,4]` passed through reduce would be 1 + 2 = 3 + 3 = 6 + 4 = 10.

## Things I want to know more about
When reduce builds the new value does it create a new data key like (using the example above) `newArr = 10` or does it just change `arr = [10]`. I'm assuming it isn't pushing the data into `arr=[1,2,3,4,10]` or am I mistaken?