![General Assembly Logo](https://camo.githubusercontent.com/1a91b05b8f4d44b5bbfb83abac2b0996d8e26c92/687474703a2f2f692e696d6775722e636f6d2f6b6538555354712e706e67)

# NoSQL Research Lab

## Explainer

Up until now in the cohort we have stored data only in what are known as relational databases (SQL is the most well known type of relational DB querying language). Relational databases structure our data into tables. Today we will learn about a different type of database: a non-relational one. 

## Lab

In this lab you will be researching, either individually or in groups, answer to the following questions about noSQL databases. The intention is for you to spend some time learning about the fundamental differences between the type of databases we have seen before and the new type we will be learning about today. Even more importantly, you will learn about why two types of databases are used, and what situations fit each type of db. 

## Setup

Fork and clone this repository and answer questions as you research directly in the README. You do not have to submit this lab, but you will want to have it on hand for reference in the future. 

## Questions:

1. What does the term noSQL refer to, and what other term is often used synonymously with noSQL?
  - "Not Only SQL" is the synonymous term. noSQL refers to a non-tabular databases and store data differently than relational tables.
2. What are some of the common arguments for using a non-relational versus a relational db?
  - optimization on developer productivity
  - allow developers to store huge amounts of unstructed data, providing felxibility
  - optimized for agile environment - give developers ability to iterate quickly and make changes throughout the software stack all the way down to teh database(faster queries and ease of use)
  - provide capabilities to scale out instead of scale up
3. In this class we will be using the document style of non-relational databases. What are the charecteristics of a document based db? 
  - Document databases store data in documents similar to JSON (JavaScript Object Notation) objects. Each document contains pairs of fields and values. The values can typically be a variety of types including things like strings, numbers, booleans, arrays, or objects.
4. In this class we will be using Mongo specificially as our no-SQL db. Look into Mongo and answer this question: what is the priamry difference between how Mongo is maintained vs SQL?
  - https://www.mongodb.com/nosql-explained/nosql-vs-sql#differences-between-sql-and-nosql
5. Mongo DBs are organized into documents. Describe an example of a table in SQL that contains users, and then describe the equivalent DB setup in Mongo.
  -  SQL: 
``` INSERT INTO users(user_id, age. status)
    Values ('bcd001', 45, "a"): 
```
  - Mongo: 
``` db.users.insert({
user_id:"bcd001"
age: 45
status: "a" 
}) 
```
6. What is an example situation where a Mongo database makes sense versus a non-relational db?
  - makes collaboration easier - developers can own documents or portions of documents and evolve them as needed without intermediation or complex deendency chains between different terms.
7. What are the benefits of SQL databases? NoSQL Databases?
  - SQL Benifits
    - Commonality of the language and lack of complex code needed 
    - Can be used from phone, labtops or PCs
    - Well established and can quickly recieve records from a database
  - noSQL Benifits
    - flexible schema where you can easily make changes to the database
    - uses language common to other dev languages so that developers can store their data the same as in their aplicable code
    - follows the "data that is accessed together should be stored together", makes querying easier by building out not building up and eliminating join tables
8. Explain the differences between ACID and BASE models.
  - ACID; ACID stands for; Atomic, Consistent, Isolated, and Durable
  - BASE stands for Basically Availible, Soft State, Eventually Consistent
  - Some of the differences come the flexibility and structure that you are seaking; banks and financial instatutions use ACID because they need structure and reliablity, Social Media companies use BASE because they need to build out
12. What should you consider when deciding between using a relational database or a non-relational database for your project?
  - Think about what you are looking for in your project; flexibility, structure, association relationships, growth, etc.


## Visual Comparisons

### Structure

![](https://media.git.generalassemb.ly/user/16103/files/65db7f00-afd5-11ea-926a-e51b2fd2be08)

### Relationships

![](https://media.git.generalassemb.ly/user/16103/files/5eb47100-afd5-11ea-8cae-0a65c924be4b)

### Use Cases

![](https://media.git.generalassemb.ly/user/16103/files/7f7cc680-afd5-11ea-82c8-10ed74ee2222)

## Additional Readings

Pick an additional reading to go through with a classmate. Reflect on how the
article changes the discussion. What have you learned?

  _**Note:** You do not have to read about the different types of SQL and NoSQL. We will use PostgreSQL and MongoDB in this course._
- [ACID vs. BASE Explained](https://neo4j.com/blog/acid-vs-base-consistency-models-explained/)
- [PostgreSQL Use Cases](https://www.cybertec-postgresql.com/en/postgresql-overview/solutions-who-uses-postgresql/)
- [MongoDB Use Cases](https://www.mongodb.com/use-cases)
- [What the heck are you actually using NoSQL for?](http://highscalability.com/blog/2010/12/6/what-the-heck-are-you-actually-using-nosql-for.html)
- [A co-Relational Model of Data for Large Shared Data Banks](http://queue.acm.org/detail.cfm?id=1961297&repost)
- [A brief history of databases](http://avant.org/media/history-of-databases)
- [NoSQL Databases: An Overview | ThoughtWorks](http://www.thoughtworks.com/insights/blog/nosql-databases-overview)
- [When to choose CouchDB vs RDBMS?](http://stackoverflow.com/a/2731207/402618)
- [CAP Twelve Years Later: How the "Rules" Have Changed](http://www.infoq.com/articles/cap-twelve-years-later-how-the-rules-have-changed)
