# ***Day 2** - React Lifecycle and its 'state' vs 'props'*

## React: Component Lifecycle Events - [Joshua Blankenship](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

### This reading taught the lifecycle of the react component, broke it down into its three phases. Understanding these phases and what events coincide with them will help remember when you can and can't update the User Interface and the application states.

Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? 

- Render

What is the very first thing to happen in the lifecycle of React? 

- Mounting phase; constructor > "is called before it is mounted...can be used to assign state or to bind event handle methods to an instance." Blankenship

Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates 

- constructor, render, React Updates, componentDidMount, componentWillUnmount

What does componentDidMount do?

- This is for loading anything using a network request or initializing the DOM. Can also by used to set up subscriptions.

## React State Vs Props [Web Dev Simplified](https://www.youtube.com/watch?v=IYvD9oBCuJI)

### The React State vs Props video taught the differences between state and React. Props can be modified outside the component and then passed down to the state. Mastering these are important to writing dry code for your web application/pages.

What types of things can you pass in the props?

- arguments that modiy the component/state

What is the big difference between props and state?

- Props pass into a component and are handled/updated outside the component where state is handled inside the component and is handled/updated inside the component.

When do we re-render our application?

- Whenever the state changes

What are some examples of things that we could store in state?

- values being updated in a form, any information that is being handled/updated in the component.

### Things I want to know more about

Are the three phases of the React lifecycle run consecutively or concurrently?