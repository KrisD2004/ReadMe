# Introduction to Databases and ERDs

## Definition of Data and Database and Data modeling 

* Data is a collection of facts and figures that can be processed to produce information.
* A database is a collection of related data. Data aids in producing information based on facts.

## Characteristics of a Modern DBMS

1. Real-World Entity: A modern DBMS uses real-world entities, their behavior, and attributes to design its architecture.

2. Relation-Based Tables: DBMS organizes data into tables, representing entities and their relationships.

3. Isolation of Data and Application: A database system is distinct from its data. DBMS stores metadata to facilitate its own processes.

4. Less Redundancy: DBMS follows normalization rules to reduce data redundancy and optimize storage.

5. Consistency: DBMS maintains data consistency using methods and techniques to avoid inconsistencies.

6. Query Language: DBMS comes with a query language for efficient data retrieval and manipulation.

7. ACID Properties: DBMS ensures Atomicity, Consistency, Isolation, and Durability for transactional integrity.

8. Multiuser and Concurrent Access: DBMS supports multi-user environments with parallel data access.

9. Multiple Views: DBMS offers different views of the database for various user requirements.

10. Security: DBMS provides security features like access restrictions and data constraints to protect data integrity.

## User Categories:

1. Administrators: Responsible for managing and maintaining the DBMS, creating access profiles, enforcing security, and overseeing resources.
2. Designers: Design the database structure, including entities, relations, constraints, and views.
3. End Users: Benefit from the DBMS by accessing and utilizing data. Ranges from simple viewers to sophisticated business analysts.

DBMS plays a crucial role in organizing and managing data efficiently, providing a structured and secure way to store, retrieve, and manipulate information. It offers features like data consistency, concurrency control, security, and ease of data access through a query language.

## DBMS Questions

1. In a relational database, relationships define the associations or connections between tables (also known as entities) based on shared data. These relationships are crucial for organizing and structuring data in a meaningful and efficient way.

2. One-to-One (1:1) Relationship:
A one-to-one relationship exists between two tables when each record in the first table is associated with at most one record in the second table, and vice versa. 

3. Many-to-Many (M:N) Relationship:
A many-to-many relationship exists between two tables when each record in the first table can be associated with multiple records in the second table, and vice versa. 

4. One-to-Many (1:M) Relationship:
A one-to-many relationship exists when each record in the first table can be associated with multiple records in the second table, but each record in the second table is associated with at most one record in the first table. 

5. Many-to-One (M:1) Relationship:
A many-to-one relationship is essentially the reverse of a one-to-many relationship. 

## Data model

* DataType Attribute:

Specifies a more specific data type than the database intrinsic type.
Enhances semantics of data and enables HTML5 features.
Useful for controlling display format, like showing only dates.

* DisplayFormat Attribute:

Explicitly defines the format for displaying values.
Combined with DataType for improved formatting control.
Supports formatting during editing with ApplyFormatInEditMode.

* StringLength Attribute:

Sets maximum and minimum string lengths for properties.
Provides client-side and server-side validation for data length.

* RegularExpression Attribute:

Applies regex-based restrictions to input values.
Useful for enforcing specific input patterns.

* Column Attribute:

Controls how class properties map to database columns.
Allows customization of column names in the database.

* Database Migrations:

Updates database schema based on model changes.
Utilizes Entity Framework Core CLI (dotnet ef) for creating and applying migrations.
By utilizing these attributes and migration techniques, developers can significantly improve their ASP.NET Core MVC applications by managing data presentation, validation, and database schema modifications effectively.

## Data Models QUESTIONS 

1. Database Schema:

A database schema is a logical blueprint that defines the structure, organization, and relationships among the data stored in a database. It serves as a framework for creating, storing, and managing data in a structured and efficient manner. The schema outlines the tables, columns, data types, constraints, and relationships within a database.

What is a Schema?

A schema is a high-level representation of the database's logical structure, including tables, fields, data types, and relationships. It defines how data is organized and stored in a database.

Why do we use them?

We use database schemas to:

Organize Data: Schemas provide a structured way to organize and categorize data, making it easier to manage and query.

Ensure Data Integrity: By defining constraints and rules within the schema, we can maintain data integrity and prevent inconsistencies.

Improve Query Performance: A well-designed schema can optimize query performance by reducing unnecessary data retrieval and processing.

Facilitate Collaboration: Schemas provide a standardized framework that multiple users and applications can follow, promoting effective collaboration and data sharing.

What do they look like?

A database schema is typically represented using a combination of tables, columns, relationships, and constraints. It is often depicted graphically using entity-relationship diagrams (ERDs) or textual representations.

2. Different Types of Database Keys:

Primary Key: A primary key uniquely identifies each record in a table and ensures data uniqueness and integrity.

Foreign Key: A foreign key establishes a relationship between two tables by referencing the primary key of another table. It enforces referential integrity between related tables.

Composite Key: A composite key is a combination of two or more columns that together uniquely identify a record within a table. It is used when a single column cannot provide unique identification.

Primary Key:

A primary key is a unique identifier for a record in a table. It ensures that each record is distinct and can be used as a reference in other tables. Every table should have a primary key, and it should have the following properties:

Unique: No two records can have the same primary key value.
Not Null: The primary key value cannot be null.
Fixed: The primary key value should not change over time.
Foreign Key:

A foreign key is a column or set of columns in one table that refers to the primary key of another table. It establishes a relationship between the tables and ensures data consistency and integrity. Foreign keys are used to maintain referential integrity and enforce relationships between tables.

Composite Key:

A composite key is a combination of two or more columns that together serve as the primary key of a table. It is used when a single column cannot uniquely identify a record. Composite keys are used to handle situations where the combination of values is unique.

Relationships in a Relational Database:

Relationships in a relational database define how tables are connected or related to each other. There are several types of relationships:

One-to-One (1:1) Relationship: In a one-to-one relationship, one record in a table is associated with only one record in another table, and vice versa.

One-to-Many (1:N) Relationship: In a one-to-many relationship, one record in a table is associated with multiple records in another table, but each record in the second table is associated with only one record in the first table.

Many-to-Many (N:N) Relationship: In a many-to-many relationship, multiple records in one table are associated with multiple records in another table. This relationship is typically implemented using an intermediary table.

Many-to-One (N:1) Relationship: This is the reverse of a one-to-many relationship. Multiple records in one table are associated with a single record in another table.

The choice of relationship type depends on the nature of the data and the business requirements of the database design.






