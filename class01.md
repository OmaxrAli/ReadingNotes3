# What is a Component:

A component is a piece of code and modular that fills a functional part in an interface  That is, a software component can be deployed independently and is subject to composition by third parties.
Characteristics of Components so a component is a part of an interface that made out of lines of code to separate to problem into smaller pieces to solve the big problem better.
Here usually the component is basically looking better into the concept of  component reusability

Reusability − Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.

![component](http://www.codingthearchitecture.com/images/20130810-techtribesje-updater-components.png)

# Replaceable − Components may be freely substituted with other similar components.

+ Not context specific − Components are designed to operate in different environments and contexts.
+ Extensible − A component can be extended from existing components to provide new behavior.
+ Encapsulated − A A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.
+ Independent − Components are designed to have minimal dependencies on other components.

# What are the advantages of using component-based architecture?

+ Ease of deployment − As new compatible versions become available, it is easier to replace existing versions with no impact on the other components or the system as a whole.
+ Reduced cost − The use of third-party components allows you to spread the cost of development and maintenance.
+ Ease of development − Components implement well-known interfaces to provide defined functionality, allowing development without impacting other parts of the system.
+ Reusable − The use of reusable components means that they can be used to spread the development and maintenance cost across several applications or systems.
+ Modification of technical complexity − A component modifies the complexity through the use of a component container and its services.
+ Reliability − The overall system reliability increases since the reliability of each individual component enhances the reliability of the whole system via reuse.
+ System maintenance and evolution − Easy to change and update the implementation without affecting the rest of the system.
+Independent − Independency and flexible connectivity of components. Independent development of components by different group in parallel. Productivity for the software development and future software development.

#	What is props short for?
props.
“Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another.
But the important part here is that data with props are being passed in a uni-directional flow. (one way from parent to child)
Furthermore, props data is read-only, which means that data coming from the parent should not be changed by child components.
#	How are props used in React?

1.	Firstly, define an attribute and its value(data)
2.	Then pass it to child component(s) by using Props
3.	Finally, render the Props Data

#	What is the flow of props?
One-Way Data Flow
Props have a one way downward binding between the parent and child component.
When the parent property updates, then the updates are passed into the child via props.
This prevents child components from accidentally mutating the parent’s state.
And this makes our app easier to understand.
We should never mutate props.
If we need to change their value, then we should assign them to a new property first.
For instance, if we need to change the value of an initial value that’s set with the prop’s value, then we should assign that to a state first.
![](https://miro.medium.com/max/700/1*nvQ3jAPwnU7cnlLMPNJnzA.png)
