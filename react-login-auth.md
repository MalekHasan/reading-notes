# Reading: ```<Login />``` and ```<Auth />```


## What is Role Based Access Control (RBAC)?

1. What is Role Based Access Control (RBAC)?

***restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.***  

2. Share some an example of RBAC including all possible CRUD operations and correlating roles.  

- ***Management role scope – it limits what objects the role group is allowed to manage.***  

- ***Management role group – you can add and remove members.***  

- ***Management role – these are the types of tasks that can be performed by a specific role group.***  

- ***Management role assignment – this links a role to a role group.***  

***By adding a user to a role group, the user has access to all the roles in that group. If they are removed, access becomes restricted. Users may also be assigned to multiple groups in the event they need temporary access to certain data or programs and then removed once the project is complete.***
3. What are the Benefits of RBAC? 

***Managing and auditing network access is essential to information security. Access can and should be granted on a need-to-know basis. With hundreds or thousands of employees, security is more easily maintained by limiting unnecessary access to sensitive information based on each user’s established role within the organization. Other advantages include:Reducing administrative work and IT support,Maximizing operational efficiency and Improving compliance.***


Compare and Contrast the following two Libraries and the following questions. Yes, they are similarly named.

***```react-cookie library```***
***```react-cookies component```***

1. Describe some react-cookie features.

- Cookie Management: react-cookie allows you to easily set, get, and remove cookies in your React components.

- Hooks and Components: It provides hooks like useCookies for accessing cookies in functional components and components like CookiesProvider for managing cookies in your application.

- Server-Side Rendering (SSR) Support: react-cookie has support for server-side rendering, ensuring that cookies can be managed both on the client and server sides of your application.

- TypeScript Support: It offers TypeScript support, making it a good choice for projects using TypeScript.

- Well-Maintained: As of my last knowledge update in September 2021, react-cookie was actively maintained and had a significant user base.

2. Describe some react-cookies features. 

- Simple API: react-cookies provides a simple and straightforward API for managing cookies in React applications.

- Get and Set Cookies: You can easily get and set cookies using methods like get, set, and remove.

- No Dependencies: react-cookies doesn't have any external dependencies, which can make it a lightweight choice.

- Cookie Options: You can specify additional options for cookies, such as expiration time and domain.

- No React-Specific Features: Unlike react-cookie, react-cookies doesn't offer React-specific hooks or components. It's a more general-purpose cookie management library.

3. Which library would you prefer would you prefer? Why?
react-cookie,  preferred choice for managing cookies in React due to its seamless integration, support for server-side rendering, TypeScript support, and active community. It simplifies cookie management within the React ecosystem.