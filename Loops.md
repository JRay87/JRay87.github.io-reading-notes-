# ***Operators and Loops***

Assignment operators assign a value to its left and right operand. 
`x=f() -> x= `
`x /=f()-> x=fl/fr`

Comparison Operators compare the operands and returns a logical value based on whether the comparrison is true. In this code the system will be supplied one or multiple variables and will compare the data against the desired outcome. This can then be used for systems such as `if , else , else if , while, for` etc., can come into play. 

Now that we understand the basics of what IS a function, different operators, and how to code and execute functions we should learn about some of the different types of functions you will see during the 102 class. We're not going too into the woods with this class, so we will mainly focus on a For loop and a While loop. A for loop will run a set number of times or until a condition is met. A while loop will run until a condition is met, potentionally forever. The example that stuck in my head was a For loop was saying I was going to run 10 laps unless its raining. A While loop means I am going to run UNTIL the rain shows. (Run Forest, Run!)
 
 A For loop is formatted as such:
    `for ([Initial Expression]; [Conditional Expression]; [IncrementExpression]) statement`
   
   A simple For loop example (provided by our instructor) was:
   
   `let students = 19;`

   `for (let i = 1; i <= students; i = i + 1){`
        `console.log("Hi to student #", i);`
   `}`

   `console.log("We're out of the loop!");`
   
   Broken down this means that we are defining the variable "students" = 19, we start counting at 1, every time invoked the function will log in the console a welcome greeting to the students up until student 19 has logged in. Then we "break out of the loop" and the console outputs a different message.
   
   
   
   A while loop is even simpler. 
   
   `while (condition)`
        
         ` statement`

         Example:
   
    `x=0 while (x<=5) {`
        
        `console log("hi");`
        
        `x = x+1;`
    `}`

    The above code runs a funtion that as long as the value of X is less than 5, the console will log a "Hi" message until the x is valued higher than 5.







    Click [Here](README.md) to return home