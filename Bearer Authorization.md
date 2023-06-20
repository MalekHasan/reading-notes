# Bearer Authorization

## Intro to JWT

1. What is a JSON Web Token (JWT)?

***Is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.***

2. When should we use JSON Web Tokens?

- ***Authorization***
- ***Information Exchange***

3. Claims are expected in which structural component of a JWT?


***Payload***

## Are JWTs Secure?

1. If I get a JWT and I can decode the payload, how can we call that secure?

***JWTs can be either signed, encrypted or both. If a token is signed, but not encrypted, everyone can read its contents, but when you don't know the private key, you can't change it. Otherwise, the receiver will notice that the signature won't match anymore.***

2. If sending a JWT, what must sender and receiver both know? Hint, it’s appended in the signature.

***They both know some shared secret between them.***

3. Explain how concatenated content and secret can be sent and received securely to a non-technical recruiter.

***The concatenated content will merge to secert(which is a secret message or information between the sender and the receiver they both just know this secret) then we will encrypt this hole things and send it so if someone interface the JWT tokens and he don't know the secret he can't access and change the JWT.***

## JWTs Explained



1. Why use JWT?

***It is used to securely transfer information between any two bodies and two bodies that means any two users any two server any two bodies and it's very usefull in Authorization and Information exchange.***
2. JWT is Compact and self-contained. Describe how this is useful to a non-technical friend.

***Compact means you can send the JWT token via URL, some action like sign in and here we use somthing called method requests(or HTTP method) or when we send data between two bodies we cut the data to something called packets each packet consist of two things also first one called header and the seconde challed body we send this JWT tokens via this header And self-containd means this token hold and containes the information about the user.***

3. What are the three components (the structure) of a JWT signature?

- ***Header***
- ***Payload***
- ***Signature***