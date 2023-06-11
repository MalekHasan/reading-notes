# Data Modeling 
## nosql vs sql

1. What type of database is the best fit for the complex query intensive environment?
***SQL databases***  
2. What type of database is the best fit for hierarchical data storage?
***SQL databases***
3. Describe the differences in scalability between a SQl and NoSQL database as though you were speaking to a non-technical friend.
***Scalability means if we neet to improve our performance we should do something in SQL we need to upgrade the server (Computer) component ( CPU,RAM,SSD...etc) whereas in NoSQL we can do the same in SQL or we can add a new servers as much as we need.***


## sql modeling techniques

1. Among data tables, what is a one-to-many relationship and how do we “relate” them?
***The entry in one table can be related to more than one entry in another.We connect lines between tables to show relationships***
2. Prior to designing your relational database, it might be useful to ___ a ___ of the database tables and their relationships.
Prior to designing your relational database, it might be useful to ***create*** a ***diagrams*** of the database tables and their relationships.
3. Explain the difference between a primary and foreign key.
- Primary keys uniquely identify each row in a table.  A table typically has one primary key, but can have more.
- Foreign Key is a column or set of columns which match a primary key in another table.  

## sql vs nosql

1. How do we treat keywords and parameters differently in SQL syntax?

In SQL syntax, keywords are reserved words that have specific meanings and functionalities within the language. They are used to define commands, clauses, and data manipulation operations. Keywords cannot be used as identifiers or variable names.

On the other hand, parameters in SQL are placeholders used to pass values into queries or stored procedures.

2. Define normalization within the context of schemas and data.


Normalization, in the context of schemas and data, refers to the process of organizing and structuring data in a relational database to eliminate redundancy and improve data integrity and efficiency. It involves breaking down data into smaller, more manageable tables and applying certain rules, known as normalization forms, to ensure that each piece of data is stored in the most appropriate and efficient manner. Normalization helps eliminate data anomalies, such as update anomalies and data inconsistencies, and promotes data consistency and accuracy within the database.  

3. Explain the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter.

one-to-one :
Let's say you have a database for employee records in a company. Each employee has a unique employee ID. In this case, there can be a one-to-one relationship between the employee and their office location. Each employee is assigned to a specific office location, and that office location is dedicated to that employee only.

one-to-many :

Let's say you have a customers and orders here each customer have one or more orders but each order is ordering by one customer.

many-to-many :
Let's say you have a students and courses each student have one or more courses and each course taken by one or more student.
