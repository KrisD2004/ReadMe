# Nosql v sql

### SQL Databases

* Also known as Relational Databases (RDBMS).
* Data is stored in tables with predefined schemas.
* Use structured query language (SQL) for defining and manipulating data.
* Vertically scalable by increasing hardware resources.
* Good for complex query-intensive environments and heavy-duty transactional applications.
* Examples: MySQL, Oracle, SQLite, PostgreSQL, MS-SQL.

### NoSQL Databases

* Also known as non-relational or distributed databases.
* Data is stored in various formats like key-value pairs, documents, graph structures, or wide-column stores.
* Dynamic schema allows for unstructured data.
* Horizontally scalable by adding more database servers.
* Queries are focused on collections of documents, with various query languages.
* Preferred for hierarchical data storage and large datasets.
* Examples: MongoDB, BigTable, Redis, RavenDB, Cassandra, HBase, Neo4j, CouchDB.

### SQL Database Examples

1. MySQL Community Edition:
Popular open-source database, often used with Apache and PHP.
Features replication, sharding, and Memcached for performance.
Available for multiple platforms and languages.
Cost-effective and stable.

2. MS-SQL Server Express Edition:
Powerful and user-friendly database with Microsoft support.
Integrated development environment (IDE) for developers.
Offers disaster recovery mechanisms and cloud backup.

3. Oracle Express Edition:
Free limited edition of Oracle Enterprise Edition.
Easy to upgrade and supports multiple platforms.
Reliable, secure, and easily manageable.

### NoSQL Database Examples

1. MongoDB:

* Document-based NoSQL database storing data in JSON-like documents.
* High performance for simple queries and scalability through horizontal scaling.
* Easy to use for developers and administrators, with dynamic schema support.

2. CouchDB:

* Document-based NoSQL database storing data in JSON documents.
* Schema-less and accessible through HTTP queries.
* Automatic conflict resolution and straightforward replication.

3. Redis:

* Open-source NoSQL database known for its speed.
* Provides efficient data structures and can be used as a cache.
* Works with in-memory datasets and considered one of the fastest NoSQL servers.

### Nosql v Sql Questions

1. An SQL database is a good fit for structured data that adheres to a predefined schema. It works well for applications where the data has a consistent structure and relationships between entities are clearly defined. A real-world example of data suitable for an SQL database is an e-commerce website.
2. A NoSQL database is a good fit for unstructured or semi-structured data that does not follow a rigid schema. It is suitable for scenarios where data is evolving, and the structure may vary between different documents or entities. A real-world example of data suitable for a NoSQL database is a social media platform.
3. For hierarchical data storage, NoSQL databases are generally considered a better fit. NoSQL databases, such as document-based or graph databases, can handle hierarchical data structures more naturally.
4. When it comes to scalability, NoSQL databases are typically preferred. NoSQL databases are designed to scale horizontally by distributing data across multiple servers, making them well-suited for handling large amounts of data and high traffic loads.

## Video Questions

1. What does SQL stand for?

SQL stands for "Structured Query Language". It's a programming language used to communicate with and manipulate databases.

2. What is a relational database?

A relational database is a type of database that organizes data into tables, and these tables (also called 'relations') can be linked to each other based on their common data. Each table consists of rows (records) and columns (fields).

3. What type of structure does a relational database work with?

A relational database works with a structured, table-based format. Each table has a fixed structure with a set number of columns (fields) that define the data to be stored, and each row in the table represents a single record.

4. What is a ‘schema’?

A schema in a database is like a blueprint. It defines how data is organized and how the relations among them are associated. It outlines how data is stored in the database in terms of tables, fields, relationships, constraints, and indexes.

5. What is a NoSQL database?

A NoSQL database is a type of database designed to handle data that doesn't fit well in a rigid, table-like structure that SQL databases use. They can handle unstructured data and can scale horizontally across servers.

6. How does it work?

NoSQL databases work by storing data in a format that is either key-value pairs, wide-column stores, a graph format or document-oriented. They don't require a fixed schema and can handle large volumes of data.

7. What is inside of a MongoDB database?

Inside a MongoDB database, data is stored in a format called BSON, which is similar to JSON. Data is organized into 'collections' (similar to tables in SQL), and each individual data point is a 'document' (similar to a row in SQL), which can contain various 'fields' (like columns in SQL). But unlike SQL, each document can have a different structure and different types of data.

8. Which is more flexible - SQL or MongoDB? And why?

MongoDB is generally more flexible than SQL. This is because MongoDB does not require a fixed schema, so data can be stored in various formats and structures. In contrast, SQL requires a predefined schema and the data must fit into this structure.

9. What is the disadvantage of a NoSQL database?

One disadvantage of NoSQL databases is that they lack the standardization that SQL databases have. This means different NoSQL databases can have different query languages and APIs, which can create a steeper learning curve.

Also, while NoSQL databases can handle unstructured data and scale horizontally, they generally don't support complex queries and transactions as well as SQL databases do. This makes them less suitable for applications where data integrity and consistency is crucial.
