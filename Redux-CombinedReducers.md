# Redux - Combined Reducers

## Multiple Reducers Example

1. Why create multiple reducers?

***Reducers are a great concept in Redux, because they allow your react application to have specific pieces of data that all update synchronously.  All reducers run against your Redux store, and then the store triggers a change event and your entire React.js application re-renders.***

2. How would you combine multiple reducers?

***Using function aclled ```combineReducer({})``` that take a object containe the all reducers which bulit by thee developer. ***

3. How will you manage state as an immutable object? why?

*** We must create a new copy of it and do modifications to that copy - which then becomes the new redux state.Immutability of redux state is necessary since it allows detecting redux state changes in an efficient manner. ***

## Redux Docs: Using Combined Reducers

1. combineReducers is a utility function to simplify the most common use case when writing ___ _____ .

***Redux reducers.***

2. Explain how combineReducers assembles the new state tree.

***One frequently asked question is whether Redux "calls all reducers" when dispatching an action. Since there really is only one root reducer function, the default answer is "no, it does not". However, ```combineReducers``` has specific behavior that does work that way. In order to assemble the new state tree, ```combineReducers``` will call each slice reducer with its current slice of state and the current action, giving the slice reducer a chance to respond and update its slice of state if needed. So, in that sense, using ```combineReducers``` does "call all reducers", or at least all of the slice reducers it is wrapping.***

3. How would you define initial state in an app using combineReducers?

***There are two ways to define the initial shape and contents of your store's state. First, the ```createStore``` function can take ```preloadedState``` as its second argument. This is primarily intended for initializing the store with state that was previously persisted elsewhere, such as the browser's localStorage. The other way is for the root reducer to return the initial state value when the state argument is ```undefined```. These two approaches are described in more detail in Initializing State, but there are some additional concerns to be aware of when using ```combineReducers```.***

## Redux Docs: Combined Reducer Syntax

1. Why will you want to split your reducing functions as your app becomes more complex?

***As your app grows more complex, you'll want to split your reducing function into separate functions, each managing independent parts of the state.***

2. The _____ helper function turns an object whose values are different reducing functions into a single reducing function you can pass to ____.

***The ```combineReducers``` helper function turns an object whose values are different reducing functions into a single reducing function you can pass to ```createStore.```.***

3. What is a popular convention when naming reducers?

***A popular convention is to name reducers after the state slices they manage, so you can use ES6 property shorthand notation: ```combineReducers({ counter, todos })```. This is equivalent to writing ```combineReducers({ counter: counter, todos: todos })```.***