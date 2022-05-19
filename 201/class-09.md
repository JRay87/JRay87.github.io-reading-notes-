# Reading 9 - Forms and JS Events

## ***HTML Chapter 7** - Forms*

Forms are a great way for users to supply information to the website to complete a task. Whether that's a search in DuckDuckGo, logging in selecting options from a menu, or buttons to interact with the site. Forms interact with the user and browser when the user fills in a form. It gets sent to the server, which verifies the information and creates a new page to send back to the user. 

Every form tag requires an action statement telling the browser where to send the information.

input tags need the type, text to proceed the window, size of the window, and the max amount of characters the user can input. If the input type is password the input will appear blocked out to the user for security.

Buttons can be used to select things. Radio allows selecting one, checkbox allows for one or more, dropdown list displays a list of values for the user to choose from, and multiple select box allows for multiple from a list.

The labeling function allows the visualy impaired to access your forms.

Form elements live in a fieldset. Creates a "border" in most brosers to show the user the values in the form are related.

HTML5 has made some changes to traditional form elements: browsers complete form validation and input standardization including email and url validation and added a special type of input for single line text boxes.

## ***HTML Chapter 14** - Lists, Tables, and Forms*

Lists can be formatted to have many different markers. Ordered lists can display numbers, letters, numerals, etc., Unordered lists can use discs, circles, squares, small imgs, and you can modify how the bullets are displayed on the screen.

Tables can be modified by row, column, down to individual cells, and has many of the same properties that can be changed.

Individual cells can be modified in many ways. If cells are empty the cell can be hidden in CSS. You can put border spacing or collapse to modify the spacing.

Buttons can be modified for the browser as well.

Forms should be checked to ensure their inputs line up and the float property can help align the input fields.

CSS can change the cursor displayed to the user.

8Forms benefit from styles that make them feel more interactive.

## ***JS Chapter 6** - Events*

Events are when the browser registers an event. This lets your script know it is time to run a script and respond in some way to the event. This list of what events can trigger JS code to run is long, but it can be initiated by any interaction with the site if you code it right.

To trigger an event the developer selects the element they was the script to respond to, indicate which event it will trigger (binding it to the DOM node), and state the code to run.

Binding can be done in three ways:

- HTML event handlers (**BAD PRACTICE**) written directly to HTML opening tag

- DOM event Handlers - written in JS can only attach a single function to an event(`element.event = functionName;`)

- DOM lvl 2 event listeners - can handle multiple fucntions but are not supported by older browsers

Stopped at p 254, will finish 19May

<hr />

## ***Things I want to know more about***

what other types of things can the hidden values do? What is the value of the hidden control?

Does the label function read the word out-loud to the person?