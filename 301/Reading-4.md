# Day 4 - *Controlled Components and Ternary Operators*

## [React Docs - Forms](https://reactjs.org/docs/forms.html)

***Controlled Components are built and have the state controlled by React. These controlled components allow the input to update with the state and vice versa.*** 

### What is a ‘Controlled Component’?

A controlled component is 'an input form element (`<input>``<textarea>``<select>`) whose created by and whose value is controlled by React making it a single form of truth'. This means that react creates and controls in the `form` element.

### Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

Updates by the user should be updated as the user is inputting as it gives the code more control over the input. You can then target other elements like unlocking the submit button only after the input meets certain specifications.

### How do we target what the user is entering if we have an event handler on an input field?

`event.target.name` this, when placed in an event handler tells the the code what to target.

## [The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

***Ternary operators are used to write conditional if statements in javascript. Understanding the syntax of the ternary operator can speed up development time over writing out if else statements in the code.***

### Why would we use a ternary operator?

 A ternary operator is used to shorten a conditional, or 'if' statement. This takes multiple lines of code and shrinks it down to one line. 

### Rewrite the following statement using a ternary statement:

if(x===y){
  console.log(true);
} else {
  console.log(false);
}

Rewritten -> `console.log = (x===y) ? 'true' : 'false'`

### Things I want to know more about

Would the password strength images or 'strength value' and how they display/hide when you are putting in a new password be controlled component?
