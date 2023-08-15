# ```useState()``` Hook

### Thinking in React

1. Summarize the five steps of thinking in react.  

***Break the UI into a component hierarchy, Build a static version in React, It’s often easier to build the static version first and add interactivity later.Find the minimal but complete representation of UI state, To make the UI interactive, you need to let users change your underlying data model. You will use state for this.Identify where your state should live ,After identifying your app’s minimal state data, you need to identify which component is responsible for changing this state, or owns the state.Add inverse data flow ,to change the state according to user input, you will need to support data flowing the other way: the form components deep in the hierarchy need to update the state.***


### State: A Component’s Memory

1. What is one reason a local variable isn’t sufficient for managing a React component?
***Local variables don’t persist between renders. When React renders this component a second time, it renders it from scratch—it doesn’t consider any changes to the local variables.Changes to local variables won’t trigger renders. React doesn’t realize it needs to render the component again with the new data.***

2. What is the argument to the useState hook, and what are the two parts of its return array?  

The only argument to ```useState``` is the initial value of your state variable.The state variable (index) with the value you stored.
The state setter function (setIndex) which can update the state variable and trigger React to render the component again.

3. How can Component A access state from Component B?  

To have Component A access state from Component B in React:

1. Lift the shared state to a common parent component.
2. Pass the state to both Component A and Component B as props.
3. Component B manages the state and updates it via a prop function.
4. Component A uses the shared state received as a prop.
5. This enables indirect state access between the components.



