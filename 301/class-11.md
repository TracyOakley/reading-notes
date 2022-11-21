# Class 11 Notes - MongoDB and Mongoose

[Back to Home](../README.md)

## [SQL vs NoSQL](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

Fill in the chart below with five differences between SQL and NoSQL databases:

        SQL vs NoSQL

 	1. SQL databases are primarily called as Relational Databases (RDBMS); whereas NoSQL database are primarily called as non-relational or distributed database.
  2. SQL databases are table based databases whereas NoSQL databases are document based, key-value pairs, graph databases or wide-column stores. This means that SQL databases represent data in form of tables which consists of n number of rows of data whereas NoSQL databases are the collection of key-value pair, documents, graph databases or wide-column stores which do not have standard schema definitions which it needs to adhered to.
  3. SQL databases have predefined schema whereas NoSQL databases have dynamic schema for unstructured data.
  4. SQL databases are vertically scalable whereas the NoSQL databases are horizontally scalable. SQL databases are scaled by increasing the horse-power of the hardware. NoSQL databases are scaled by increasing the databases servers in the pool of resources to reduce the load.
  5. SQL databases uses SQL ( structured query language ) for defining and manipulating the data, which is very powerful. In NoSQL database, queries are focused on collection of documents. Sometimes it is also called as UnQL (Unstructured Query Language). The syntax of using UnQL varies from database to database.

SQL database examples: MySql, Oracle, Sqlite, Postgres and MS-SQL. NoSQL database examples: MongoDB, BigTable, Redis, RavenDb, Cassandra, Hbase, Neo4j and CouchDb
 	  
What kind of data is a good fit for an SQL database?

+ For complex queries: SQL databases are good fit for the complex query intensive environment whereas NoSQL databases are not good fit for complex queries. On a high-level, NoSQL don’t have standard interfaces to perform complex queries, and the queries themselves in NoSQL are not as powerful as SQL query language.

Give a real world example.

+ MySQL
+ SQL databases are best fit for heavy duty transactional type applications, as it is more stable and promises the atomicity as well as integrity of the data.

What kind of data is a good fit a NoSQL database?

+ NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data. 

Give a real world example.

+ NoSQL database are highly preferred for large data set (i.e for big data). Hbase is an example for this purpose.

Which type of database is best for hierarchical data storage?

+ NoSQL database fits better for the hierarchical data storage as it follows the key-value pair way of storing data similar to JSON data.

Which type of database is best for scalability?

+ For scalability: In most typical situations, SQL databases are vertically scalable. You can manage increasing load by increasing the CPU, RAM, SSD, etc, on a single server. On the other hand, NoSQL databases are horizontally scalable. You can just add few more servers easily in your NoSQL database infrastructure to handle the large traffic.

## [SQL vs NoSQL Video](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)

What does SQL stand for?

+ **Structured Query Language**

What is a relational database?

+ database Structure makes assumptions about how the query language works and is strict

What type of structure does a relational database work with?

+ tables (multiple) and fields

What is a ‘schema’?

+ specific defined data that can go into a table and all records have to follow the schema

What is a NoSQL database?

+  collections filled with documents

How does it work?

+ like json because no schema is enforced

What is inside of a MongoDB database?

+ lots of (unrelated) documents but also probably duplicate data

Which is more flexible - SQL or MongoDB? and why.

+ MongoDB because no schema is enforced

What is the disadvantage of a NoSQL database?

+ Because no schema is enforced you may not get back exactly what you thought 


## Bookmark and Review

+ [Mongoose API](https://mongoosejs.com/docs/api.html#Model)
+ [React Router](https://v5.reactrouter.com/web/api/BrowserRouter)
