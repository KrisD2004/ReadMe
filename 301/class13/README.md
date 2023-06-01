# More CRUD

## CRUD Basics

* CRUD stands for Create, Read, Update, and Delete. It represents the four basic operations that can be performed on data in a persistent storage system.

* Create: This operation involves adding new data to the system. It typically corresponds to the HTTP method POST in web development and is used to create new resources.

* Read: The read operation allows retrieving or viewing existing data from the system. It corresponds to the HTTP method GET and is used to fetch resources without modifying them.

* Update: This operation involves modifying existing data in the system. It corresponds to the HTTP method PUT or PATCH and is used to update the content of a resource.

* Delete: The delete operation removes existing data from the system. It corresponds to the HTTP method DELETE and is used to delete resources.

* CRUD operations are fundamental to database applications and are essential for building applications that interact with data.

* In web development, CRUD operations often correspond to HTTP methods, which communicate how you want to interact with a web server.

* When designing and developing applications, considering CRUD operations helps determine the necessary functionality and user actions for working with data.

* Each CRUD operation typically corresponds to a specific route or endpoint in an API. The route structure often includes the resource name and an identifier for the specific item being manipulated.

* Understanding CRUD operations is crucial for developers as they form the foundation for many software applications, ranging from simple to complex systems.

* Remember, CRUD operations provide a basic framework for working with data and are widely used in various domains of software development.

### Question for CRUD Basics

1. Which HTTP method would you use to update a record through an API?

To update a record through an API, the HTTP method commonly used is PUT or PATCH. Both methods can be used to modify an existing resource.

2. Which REST methods require an ID parameter?

Regarding the REST methods that require an ID parameter, typically, the HTTP methods that require an ID parameter are:

GET: When retrieving a specific resource, you would typically include an ID parameter in the URL to identify the specific resource to be fetched. For example, /api/resource/:id would fetch the resource with the corresponding ID.

PUT or PATCH: When updating a specific resource, you would include the ID parameter in the URL to identify the resource to be updated. For example, /api/resource/:id would update the resource with the specified ID.

DELETE: When deleting a specific resource, you would also include the ID parameter in the URL to identify the resource to be deleted. For example, /api/resource/:id would delete the resource with the specified ID.

## Speed COding Building a CRUD API

[Video Link](https://www.youtube.com/watch?v=EzNcBhSv1Wo)

### Questions on Video

1. What’s the relationship between REST and CRUD?

RESTful APIs align with the CRUD concept by utilizing HTTP methods to perform CRUD operations on resources. Each CRUD operation (Create, Read, Update, Delete) corresponds to a specific HTTP method (POST, GET, PUT/PATCH, DELETE). REST emphasizes a resource-oriented design approach, where resources are identified by URLs and CRUD operations are applied to these resources using the appropriate HTTP methods. This relationship between REST and CRUD allows developers to design APIs that follow REST principles while providing CRUD functionality for data manipulation.

2. If you had to describe the process of creating a RESTful API in 5 steps, what would they be?

The process of creating a RESTful API in 5 steps:

Identify Resources: Determine the resources (data entities) that your API will expose. These could be objects, concepts, or entities that your application manages.

Design URLs: Define a URL structure that represents your resources and their relationships. Use meaningful and hierarchical URLs to reflect the resource hierarchy and provide a consistent and intuitive API endpoint structure.

Choose HTTP Methods: Assign the appropriate HTTP methods (GET, POST, PUT, DELETE) to the URL endpoints based on the desired CRUD operations for each resource. Ensure that the chosen methods align with the semantics of each operation.

Define Data Formats: Determine the data format (such as JSON or XML) that your API will use for request and response payloads. Define the structure and schema of the data to ensure consistency and interoperability.

Implement API Handlers: Develop the server-side logic to handle incoming requests and perform the corresponding CRUD operations on the resources. Validate inputs, interact with the database or storage system, and generate appropriate responses for successful and error scenarios.


## Things i want to know 