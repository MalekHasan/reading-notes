# Advanced State with Reducers

## Extracting State Logic into a Reducer

1. What is the motivation for adding a reducer?  
***Components with many state updates spread across many event handlers can get overwhelming. For these cases, you can consolidate all the state update logic outside your component in a single function, called a reducer.***    
 
2. What are actions in the context of a reducer? How are they different than setting state directly?  

***The actions here is an JavaScript object sonsist of two things (type and payload),type describes the type of action being performed and the payload is optional data that provides additional information about the action. Managing state with reducers is slightly different from directly setting state. Instead of telling React “what to do” by setting state, you specify “what the user just did” by dispatching “actions” from your event handlers. (The state update logic will live elsewhere!) So instead of “setting state via an event handler, you’re dispatching an “added/changed/deleted a task” action. This is more descriptive of the user’s intent.***  

3. What common list operation is useReduce named for, and why?  
***The reduce() operation lets you take an array and “accumulate” a single value out of many***  

4. When should you switch from useState to useReducer?  

***useReducer is often chosen over useState when you need to manage more complex state or when your state updates depend on previous states and actions. It's about choosing the right tool for the job based on the complexity of your state management needs.***
