# Reading 7 

## ***Domain Modeling***

*Domain modeling is the process of creating a conceptual model in code for a specific problem.*

Defining a constructor function allows you to define the same properties for many different objects. A constructor function is when a variable is assigned a function that stores values inside its properties. (storing the data makes it accessable later in your code by other objects.)

The objects are then instantiatated (keyword - new) and initialized (given variables using 'this') before stored within the variables.

Constructor methods can have prototypes created that run the function by multiple objects without taxing the memory of the computer.

*Tips to follow when building your own domain models.* (from article)

> When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
>
> Model its attributes with a constructor function that defines and initializes properties.
>
> Model its behaviors with small methods that focus on doing one job well.
>
> Create instances using the `new` keyword followed by a call to a constructor function.
>
> Store the newly created object in a variable so you can access its properties and methods from outside.
>
> Use the `this` variable within methods so you can access the object's properties and methods from inside.


## HTML ***Chapter 6** - Tables*

The `<table>` element is used to add tables to a web page. Tables will present information to the user in a grid format. The syntax needed for table elements are:

- `<table>` - creates the table

- `<tr>` - creates new row

- `<td>` - table data

- `<th>` - table heading

If you are building a larger table other elements used are:

`<thead>` - table headings label columns

`<tbody>` - the table body (main content)

`<tfoot>` - used to display totals

## ***JS Chapter 3 (106-144)** - Functions, Methods, and Objects*

`new` keyword and Object Constructors create a blank object that can then have properties added to it. `var hotel = new Object();` 

To update the values use dot notatioon or square brackets. `hotel.name = 'Park'` ~or~ `hotel['name'] = 'Park';` (brackets do not work on methods). 

`delete hotel.name;`- deletes the name property from the hotel object. To clear the value, give it a blank string.

By using a constructor function you can build multiple objects using the same piece of code. This is less demanding on the memory of the computer and will run smoother.

### The three built-in objects

Browser Object Model - This represents the current window, contains objects that describe the browser, and is the topmost object in the model.

Document Object Model - This represents the current webpage loaded in the browser

Global JavaScript Objects - This list includes strings, number, boolean, undefined, null, and objects. Working with these valuables allows you to write methods with the values of the data types.

