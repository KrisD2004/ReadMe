# Data Transfer Objects

## How to use Data Transfer Objects in ASP.NET Core 3.1

It seems like you've provided a detailed article from InfoWorld written by Joydip Kanjilal about using Data Transfer Objects (DTOs) in ASP.NET Core 3.1. The article discusses the benefits of using DTOs, why they should be immutable, and how to work with them in ASP.NET Core applications. The article covers various aspects of DTOs, including their advantages, creation of an ASP.NET Core API project, the use of DTOs for abstraction and data hiding, immutability of DTOs, and challenges related to DTO serialization.

## Create Data Transfer Objects (DTOs)


It looks like you've provided an excerpt from a tutorial about creating Data Transfer Objects (DTOs) in a web API using Entity Framework 6. The tutorial explains how to use DTOs to shape the data that is sent over the network, allowing you to customize the data structure that clients receive from your API. DTOs can help with various tasks such as removing circular references, hiding specific properties, reducing payload size, flattening object graphs, and decoupling service and database layers.

In the tutorial, you learn how to define DTO classes for your data. Here's a summary of the key steps:

## Create DTO Classes:

Create two DTO classes, BookDto and BookDetailDto, in the Models folder.
BookDto contains a subset of properties from BookDetailDto.

## Update Controller Methods:

Modify the GetBooks method in the BooksController to return a collection of BookDto objects using LINQ's Select statement.
Modify the GetBook method to return a single BookDetailDto object using LINQ's Select and SingleOrDefaultAsync methods.
Modify the PostBook method to return a BookDto object after saving the new book.

## Optional: Load Author Data

In the PostBook method, use db.Entry(book).Reference(x => x.Author).Load() to load author information for the DTO.

## Note: Consider AutoMapper

The tutorial mentions that you can use a library like AutoMapper to automate the conversion process from entities to DTOs.