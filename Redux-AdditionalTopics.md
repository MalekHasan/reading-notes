# Redux - Additional Topics

## Redux Toolkit (RTK)

1. What concerns are addressed by Redux Toolkit?

- "Configuring a Redux store is too complicated"
- "I have to add a lot of packages to get Redux to do anything useful"
- "Redux requires too much boilerplate code"

2. What does configureStore() do?

***```configureStore()```: wraps createStore to provide simplified configuration options and good defaults. It can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes redux-thunk by default, and enables use of the Redux DevTools Extension.***

3. How would I use createSlice()?

 ***```createSlice()``` accepts an object of reducer functions, a slice name, and an initial state value, and automatically generates a slice reducer with corresponding action creators and action types.***

## MobX

1. What is Mobx?
***MobX is a simple, scalable and battle tested state management solution. This tutorial will teach you all the important concepts of MobX in ten minutes. MobX is a standalone library, but most people are using it with React and this tutorial focuses on that combination.***

2. How does MobX make it “impossible” to produce an inconsistent state?

***Make sure that everything that can be derived from the application state, will be derived. Automatically.***

3. How would we build a reactive user interface?

- Create an Observable State: Define the state of your application using observables. An observable is a special MobX data structure that can be observed for changes.

- Modify State with Actions: To change the state, create actions that modify the observable data. These actions should be wrapped in @action decorators to ensure they can modify the state.

- Create Components: Build your user interface components using libraries like React. These components can access and observe the observable state using the observer higher-order component.

- Render Components: Finally, render your components in your application, and MobX will automatically track changes to the state and re-render components as needed.

## Tutorial

What take-away(s) did this tutorial provide?