# Authentication


## Securing Passwords



1. Explain to a non-technical friend how you would safely hash and store a password.

***We usually use  an algorithim like MD5, SHA1, SHA256, SHA512, SHA-3 or another algorithim which hash the password and this algorithim designed to calculate a digest of huge amounts of data in as short a time as possible.***  

2. What is Bcrypt?

***Bcrypt is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor (also known as security factor), which allows you to determine how expensive the hash function will be.***  

3. Why might you use something like Bcrypt?

***Because we need algorithms which can make the brute force attacks slower and minimize the impact. Such algorithms are PBKDF2 and BCrypt, both of these algorithms use a technique called Key Stretching.***

## Basic Auth


1. What is Basic Authentication?

***basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic <credentials>, where credentials is the Base64 encoding of ID and password joined by a single colon :.*** 

2. What properties are necessary in the header of a Basic Auth request?
- ***Authorization***
- ***Credentials***

3. How are username:password in Basic Auth encoded?

***Using the base-64 we can encode the this string (username:password) and the result will be an encoded string.***

## OWASP auth cheatsheet


1. Define the authentication process to a non-technical recruiter.

***Is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.***

2. How should your error messaging respond (both HTTP and HTML)? Why?

 ***An application should respond (both HTTP and HTML) in a generic manner.Incorrectly implemented error messages in the case of authentication functionality can be used for the purposes of user ID and password enumeration***

3. Bookmark this link also and consider OWASP fundamentals any time you interact with authentication. Applications developed with security in mind from inception have fewer vulnerabilities throughout their lifecycle.

***Done***