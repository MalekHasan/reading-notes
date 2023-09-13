# Redux - Asynchronous Actions

## async actions

1. Why use Redux middleware?

***Redux store doesn't know anything about async logic. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Any asynchronicity has to happen outside the store.***

2. Consider the Redux Async Data Flow Diagram. Describe the flow in your own words.

***we call ```dispatch()```, and pass in something, whether it be a plain action object, a function, or some other value that a middleware can look for.Once that dispatched value reaches a middleware, it can make an async call, and then dispatch a real action object when the async call completes.And  where middleware can run logic like AJAX requests, then dispatch actions.***

3. How are we accommodating async in our Redux app?

## thunk middleware

1. Why would you need redux-thunk middleware?
2. Redux Thunk middleware allows you to write action creators that return a ____ instead of an action.
3. Describe how any return value from the inner thunk function will be made available.