# Entity Framework Core

Entity Framework (EF) Core Overview:

EF Core is a lightweight, extensible, open source, and cross-platform version of the Entity Framework data access technology.
It serves as an Object-Relational Mapper (O/RM), allowing .NET developers to work with databases using .NET objects.
EF Core eliminates the need for writing much of the data access code that would typically be required.

## Model in EF Core:

Data access in EF Core is based on a model, which consists of entity classes and a context object representing a database session.
The context object facilitates querying and saving data.
The article mentions two model development approaches: generating a model from an existing database and hand coding a model to match the database structure.

## Example Model and DbContext:

The provided C# code demonstrates a sample DbContext class, BloggingContext, with DbSet properties for Blog and Post entities.
The OnConfiguring method configures the database connection (in this case, a SQL Server connection).
The Blog and Post classes define entity properties and their relationships.

## Querying Data:

Instances of entity classes are retrieved from the database using Language Integrated Query (LINQ).
The example code illustrates querying blogs with a rating greater than 3, ordering them by URL, and converting the result to a list.

## Saving Data:

Data manipulation in the database involves creating, deleting, and modifying instances of entity classes.
The provided code snippet demonstrates creating a new Blog entity, adding it to the context, and then saving changes to the database.

## EF O/RM Considerations:

Best practices for using EF Core in production applications include having intermediate-level knowledge of the underlying database, testing, performance considerations, security review, logging, error recovery, and application deployment/migration strategies.
Next Steps:

# Data Seeding 

This content discusses data seeding in Entity Framework Core (EF Core), which involves adding initial data to a database. Three methods of data seeding are covered: model seed data, manual migration customization, and custom initialization logic.

## Model Seed Data:

EF Core allows seeding data associated with entity types as part of model configuration.
Migrations compute necessary database operations for upgrading when the model changes.
Example: Seed a Blog entity with its properties using HasData().

## Relationships and Seed Data:

For related entities, provide foreign key values when seeding.
Example: Seed a Post entity linked to a Blog.

## Seeding Owned Entity Types:

Owned entity types can be seeded similarly using the OwnsOne method.

## Using Migrations for Applying Changes:

After adding data to the model, apply changes using migrations.

## Limitations of Model Seed Data:

Best for static data not changing outside migrations and not dependent on other data.
Specify primary key values, and changing primary key may remove previous seed data.

## Manual Migration Customization:

Migrations convert seed data using HasData to InsertData, UpdateData, and DeleteData calls.
Customize by adding these calls or custom operations to migrations.

## Custom Initialization Logic:

Use DbContext.SaveChanges() for seeding before main app logic.
Ensure database creation, add data if absent, and save changes.
Avoid running seeding code as part of normal app execution to prevent concurrency issues and schema modifications.

## Execution of Initialization Code:

Run initialization code locally or deploy with the main app.
Automation possible using publish profiles.

These methods provide ways to populate a database with initial data in EF Core applications.


# How to add User Secrets to .NET Core through Visual Studio

User Secrets in .NET Core is a secure method to store private information like API keys and connection strings without exposing them in source code or version control. It involves enabling User Secrets, creating a secrets.json file for configuration, and modifying the project's .csproj file. The information is accessed via the IConfiguration API, injected into controllers, and used in code. For deployment to Azure, secrets are added as environment variables in the application settings. This ensures data confidentiality and facilitates safe deployment of .NET Core projects.