# Reading 6
## Article 1 - *Understanding the Problem Domain*

John Sonmez's article was important for any new or veteran developer. This writing was a reminder to the reader that to write the best code you need to fully understand what the problem is that this software is needed to solve.

This means speaking with the person/company you are writing code for to fully understand what it is that they are needing the software to do. Rushing into writing code causes extra stress and increases the time needed. If you fully understand what the problem is this software needs to solve, you can break it down into smaller and easier to code sections.

If you are having difficuly understanding the problem in its entirety, breaking the entire problem down piece by piece can also help lessen the time and headaches. 


## Article 2 - *Primative Values v. Object References*

Primative values (*Boolean, Null, Undefined, Number, BigInt, String, and Symbol*) are values that are set directly to a value and cannot be mutated

Object references (*Arrays, Functions, and Dates*) - Can be mutated. Object references are variables that serve as a reference (*memory address*) for property with changeable values. 
<hr />

### Creating a new variable and Mutating object (*'Object.assign'* - code supplied from article) example:

>`let lead = {`
>
 > `name: 'John Lennon'`
>
 >`group: 'The Beatles'`
>
>`}`

This first step creates the variable 'lead',  makes it an object reference for the properties (keys) 'name' and 'group', and gives those *keys* the value 'John Lennon' and 'The Beatles'

>`let coLead = Object.assign ({}, lead, {`
  >
  >`name:'Paul McCartney'`
>
>`})`

This second step creates a new variable "coLead", assigns it the same properties (*keys and values*) of 'lead', and mutates the value for object 'name' to 'Paul McCartney'

>`console.log(lead, coLead)`

This final step will log the values stored within the lead/coLead references.

<hr />

Equality checks (`===`/`!==`) can be problematic with object references because the variables have different *memory addresses*. In order to check check the contents of these objects you must go through and check that each key + value match ***OR*** you must convert the object to a *suitable* primative value before doing the check.


## JS Chapter 3 - *Object Literals* (100-105)

***Objects are everything inside the curly brackets of a variable.***

In objects, 'properties' are comprised of keys and values. (Remember the values in objects can be mutated.)

'Functions' are called 'methods' when nested inside an object. and when they are utilizing the values within their object they use the keyword 'this.'before calling for the values.
<hr />

To access an object the developer can use *dot notation.*

>*Example from book*:

>- `var hotelname = hotel.name;` - This creates the variable 'hotelname' and assigns it the value of:

The 'property value' of the 'key - name' in the 'object - hotel'. (There has to be a better way to word this.)

The developer can also use the bracket syntax:
>- 'var hotelName = hotel['name'];`

Bracket syntax is usually used when:
- Property name or method contains a special character
- Property name is a number
- A variable is being used instead of a property name
<hr />

## JS Chapter 5 - *Document Object Model* (183-242)

When a browser recieves the webpage document it builds a DOM tree which is a visual representation of the entire page. It breaks down the webpage into:
- Document Node - top of tree, represents the entire page
- Element Nodes - show the structure of the html in the page
- Attribute Nodes - This lives in the element and represents the/can change the attribute of the carrier element
- Text nodes - the text of the element node

Working within the DOM tree involves two steps; accessing the elemenent and then working with it.

Dom queries find elements within the DOM tree.
- Inidividual - `getElementById()`, `querySelector()`
- Multiple nodes - `getElementsById()`, `getElementsByTagName()`, `querySelectorAll()`

These tell the browser (*interpreter*) to locate any elements with those ids/tags/etc.,

If your query returns a node list (multiple elements) you can select individual elements and store them withtin a variable. This can be completed one of two ways: The Item Method or through Array Syntax.

- The Item Method

    `var elements = document.getElementsByClassName('hot')`

    `if (elements.length >= 1){ `

    `var firstItem = elements.item(0);`

    `}`

    This creates the variable elements and queries the DOM for any elements with class "hot". If the list contains one or more node it creates a variable "firstItem" and stores the value of index 0. 

- Array Syntax
    
    `var elements = document.getElementsByClassName('hot)`

    `if (elements.length >=1){`

    `var firstItem = elements[0];`

    `}`

  This style creates a node list containing elements that have class atrributes with the value 'hot' and stores them in the variable(/array?) elements. If the length of the node list elements is greater than or equal to 1 it creates a variable firstItem and it's value is index 1 of elements.

  Other ways to select elements are: class attribute(className), tagName, and css selectors.

  If the selection gathers a node list you can repeat the actions or loop through a nodelist. This targets the elements one by one using the index length to determine the amount of times it will repeat the action. "*When the value of the counter...no longer returns true...the loop ends. The script then continues to the first line of code after the loop.*"(p207) 

  Traversing the DOM allows you to target elements nested outside (parent element), inside (first/last Child element), or near (previous/next sibling).

  To change the content of a text node you have to access the text by traversing through the nodes and use the `.replace('orig', 'new')` syntax to replace the original text with the new.

  To add or remove HTML developers can use innerHTML property where you create the new variable containing the markup, select the element you're wanting to update, and then update it with the new markup. (*Be aware that one missing closing tag could throw out the design of the entire page.*p 220)

  You can also use DOM manipulation methods by creating new text and new element nodes, add the text node to the element node, select the fragment you are wanting to add the new element to, and add the new fragment to it.

  You can also remove elements using DOM manipulation. Select the element you wish to remove and store it in a variable, locate and store the parent element in a variable, and then remove the element using `removeChild()`.

  document.write() - easy way to add content to HTML but it has many issues and is usually not the best option.

  element.innerHTML - lets the developer modify the entire content of an element. Should not be used wo add content from users as it poses a security risk. 

  DOM Manipulation - using methods and properties to manipulate the node. Can only access one element at a time so it takes more time and code to complete tasks compared to innerHTML.
  
    > innerHTML can cause "Cross-Site Scripting (XSS) Attacks" giving malicious users access to the DOM and user tokens, giving them the capability to make purchases etc., (if the site is a storefront or contains payment info).
    
    To defend against XSS you need to validate the input is the desired datatype (validation), not allow markup/script from untrusted sources, and make sure all data going in or out of databases that any and all harmful html or characters.