# ***Reading 1** - Introduction to React and Components*

## Importance

Components are an essential piece of software development that help speed up the process of website/application development. Their portability and adaptability make them an important concept to master for a career Software Development.

Properties (or 'props') are used to pass data from parent components to their child. Understanding what they are and their traffic flow(unilateraly from parent to child) will help master the skill of writing components.

## Questions

### What is a “component”?

 A component is a piece of code that can be moved, replaced, and reused. It is a "set of well defined functionality that encapsulates its implementation and exports it as a higher-level interface." (from the [tutorialspoint.com](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm) article, what does it mean in English though?).

 It can have 3 different views - Object oriented, conventional, or Process-related. In object oriented a component is a set of one or more cooperating classes. It has all attributes and operations explained for its implementation. Conventional views the component as an element/module that integrates the processing logic, the data structures that are required to implement the processing logic and an interface that enables the component to be invoked and data to be passed to it. Finally, in Process-related view, the system builds the component from existing components already in the library. As the architecture is built the components are selected from the library.

### What are the characteristics of a component?

 Reusable, Replaceable (can be freely substituted with similar components), Not context specific (designed to operate in different environments), extensible (can be extended from existing components to provide new behavior), encapsulated (allows the caller to use the functionality, but does not expose the internal processes or variables/state), Independent (minimal dependencies on other components).

### What are the advantages of using component-based architecture?

 Reduced time and development cost because it is reusable. It also has increased reliability because it can be reused. They are easier to deploy and update to newer versions without impacting the other components. Easier to develop and maintain and they are independent of eachother.

### What is “props” short for?

 Props is short for properties. It is used to pass "immutable" (read-only/unchangeable) data down from Parent components to Child components.

### How are props used in React?

Define an attribute and its value.

 `<ChildComponent text={"I'm the 1st child"} />`

Pass it to child components using Props

 `const ChildComponent = (props) => {`

`return <p>I'm the 1st child!</p>`

`};`

Render the Props data.

 `{props}`

### What is the flow of props?

 Unidirectional (one direction) 'parent to child'

## Things I want to know more about

"set of well defined functionality that encapsulates its implementation and exports it as a higher-level interface." - Can I have this explained in different words?

Is there a way to pass props from child to parent components?

The article stated that the data passed from parent to child should not be changed, which leads me to believe that it can be. Is that a misunderstanding on my part or is there a time you would/could/should change data in the props? And if that is the case, when and why would you do this?
