# Reading 6
## Article 1 - *Understanding the Problem Domain*

John Sonmez's article was important for any new or veteran developer. This writing was a reminder to the reader that to write the best code you need to fully understand what the problem is that this software is needed to solve.

This means speaking with the person/company you are writing code for to fully understand what it is that they are needing the software to do. Rushing into writing code causes extra stress and increases the time needed. If you fully understand what the problem is this software needs to solve, you can break it down into smaller and easier to code sections.

If you are having difficuly understanding the problem in its entirety, breaking the entire problem down piece by piece can also help lessen the time and headaches. 


## Article 2 - *Primative Values v. Object References*

Primative values (*Boolean, Null, Undefined, Number, BigInt, String, and Symbol*) are values that are set directly to a value and cannot be mutated

Object references (*Arrays, Functions, and Dates*) - Can be mutated. Object references are variables that serve as a reference (*memory address*) for objects with changeable values. 
<hr />

### Creating a new variable and Mutating object (*'Object.assign'* - code supplied from article) example:

>`let lead = {`
>
 > `name: 'John Lennon'`
>
 >`group: 'The Beatles'`
>
>`}`

This first step creates the variable 'lead',  makes it an object reference for the objects name and group, and gives those objects the value 'John Lennon' and 'The Beatles'

>`let coLead = Object.assign ({}, lead, {`
  >
  >`name:'Paul McCartney'`
>
>`})`

This second step creates a new variable "coLead", assigns it the objects and values of 'lead', and mutates the value for object 'name' to 'Paul McCartney'

>`console.log(lead, coLead)`

This final step will log the values stored within the lead/coLead references.

<hr />

Equality checks (`===`/`!==`) can be problematic with object references because the variables have different *memory addresses*. In order to check check the contents of these objects you must go through and check that each key + value match ***OR*** you must convert the object to a *suitable* primative value before doing the check.


## JS Chapter 3 - *Object Literals* (100-105)



## JS Chapter 5 - *Document Object Model* (183-242)


