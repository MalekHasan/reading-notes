# Express REST API

## Review: ES6 Classes
1. Classes are a template for creating ____.

***Classes are a template for creating Objects***  

2. Can a class declaration be hoisted?  

***No, class declarations are not hoisted.***

3. How would you describe a constructor and contextual “this” to a non-technical friend?

***Constructor is like a blueprin or prototype for creating objects. "this" refers to the object itself, allowing access to its properties and methods within its own code.***

## Using Express Routing

1. Within Express, what does routing refer to?

***Routing refers to how an application’s endpoints (URIs) respond to client requests***  

2. What is the difference between a route path and a route method? 

***A route method is derived from one of the HTTP methods, and is attached to an instance of the express class. Route path define the endpoints at which requests can be made.***


3. When is it appropriate to add **next** as a parameter to a route handler and what must you do if **next** has been passed to your middleware as a parameter?

***It is appropriate to add next as a parameter to a route handler or middleware function when you want to delegate the handling of the current request to the next function in the middleware chain.However,when next is passed as a parameter to your middleware function, you should invoke it to pass control to the next middleware function in the chain. This allows the request to proceed to the next matching route handler or middleware function.***

## Express Routing

1. What is an Express Router?
***It is a mini express application without all the bells and whistles of an express application, just the routing stuff.***  

2. By what mean do we initialize express.Router() in an express server?  
***We will call instance of express.Router() first by requiring the express module then pulling the Router() from the express object.***

3. What do we use route middleware for? 

***Middlewares are functions to access the request and respose and do some proccess on them. we use middleware route to handle a speecifc route or group or routes and perform some procces or operation like authentication,logging or implemnt a custom operation.***
