# State and Props

![](https://scriptverse.academy/img/tutorials/reactjs-components-props.png)

# What types of things can you pass in the props?

When you have a React component who received some props (“properties”) from its parent component, and you want to pass all of those props on to this component’s child, then you need to pass the entire props object.
If you happen to know all of the props, then you could pass them all by just listing them out individually as the new props for the child component.
Let’s look at a code example of a ParentComponent that passes all of its props to two child components, DisplayAllProps and ChildComponent.

View raw code as a GitHub Gist
If you don’t know what the props are or don’t want to type them all out, then instead use the ... spread operator to pass all props simultaneously.
Here’s that same ParentComponent, except now it passes all of its props to its two child components without specifying the props individually:

View the raw code as a GitHub Gist
Here is the resulting React app, where ParentComponent has sent all of its props to its two child components, DisplayAllProps and ChildComponent:

View the CodeSandbox live demo (Screenshot by 
Dr. Derek Austin
)
For reference, here is the code for the ChildComponent:

View the raw code as a GitHub Gist
And to display the props as a table, I made a DisplayAllProps component, which uses Object.entries() to take a look at the React props object:

View the raw code as a GitHub Gist
As you can see, I use the ... spread operator repeatedly in order to pass all of the React props together from each parent component to its child.
Live Demo: How to Pass All React Props
If you’d like to play around with passing all props in a real React app, I used the above JSX code to make this live demo over at CodeSandbox:


# What are the differences between props and state?
Finally, let’s recap and see the main differences between props and state:

Components receive data from outside with props, whereas they can create and manage their own data with state
Props are used to pass data, whereas state is for managing data
Data from props is read-only, and cannot be modified by a component that is receiving it from outside
State data can be modified by its own component, but is private (cannot be accessed from outside)
Props can only be passed from parent component to child (unidirectional flow)
Modifying state should happen with the setState ( ) method
React.js is one today's of the most widely used JavaScript libraries that every front-end developer should know.

# When do we re-render our application?

React components automatically re-render whenever there is a change in their state or props. A simple update of the state, from anywhere in the code, causes all the User Interface (UI) elements to be re-rendered automatically.

However, there may be cases where the render() method depends on some other data. After the initial mounting of components, a re-render will occur when:

A component’s setState() method is called.

A component’s forceUpdate() method is called.

# What are some examples of things that we could store in state?
In React, whenever we are working with any data, we always use state for storing that data which may be a string, number or any complex object.
This is fine if you are using that state while rendering the component or If you want to do something when the state value changes but If you are using that state just for storing data and not using it for rendering or not passed as prop to other components then you should not use state.
Because whenever the state value changes, React will re-render the component and also all its child components will get re-rendered.
