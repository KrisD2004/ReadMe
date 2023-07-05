# Which HTTP Status Code to Use for Every CRUD App

* HTTP status codes are part of the HTTP response and provide information about the status of a request.
* Status codes are divided into classes based on their first digit: informational (100-199), success (200-299), redirection (300-399), client error (400-499), and server error (500-599).
* Custom status codes above 599 are not permitted but may be encountered in practice.
* The CRUD model (Create, Read, Update, Delete) is commonly used in API design for persistent storage operations.
* For the Create operation, common status codes are 200 OK, 201 Created, 202 Accepted, and 303 See Other.
* For the Read operation, common status codes are 200 OK, 206 Partial Content, 300 Multiple Choices, 308 Permanent Redirect, and 304 Not Modified.
* For the Update operation, common status codes are 200 OK, 204 No Content, and 202 Accepted.
* For the Delete operation, common status codes are 200 OK, 204 No Content, and 202 Accepted.
* API changes can be handled using status codes such as 307 Temporary Redirect and 308 Permanent Redirect.
* Multiple endpoints for one resource can be managed using 308 Permanent Redirect.
* Error handling can utilize status codes such as 500 Internal Server Error, 404 Not Found, 405 Method Not Allowed, 501 Not Implemented, 406 Not Acceptable, 410 Gone, 414 Request-URI Too Long, 308 Permanent Redirect, and 307 Temporary Redirect.
* Status codes like 401 Unauthorized and 403 Forbidden can be used for indicating permission issues.
* Consistency in the usage of status codes across the entire API surface is important for clarity and developer experience.

## Questions on Status Code

1. 100 -  Informational codes that indicate that the server has received the client's request and will continue processing it. These codes are used to provide feedback during the early stages of a request.
200 - Success codes that indicate that the client's request was successfully received, understood, and processed by the server. These codes inform the client that everything went well.
300- Redirection codes that indicate that the requested resource is not available at the expected location and the client needs to take further action, such as making a new request to a different location.
400- Client error codes that indicate that the client's request was invalid or could not be fulfilled by the server. These codes typically indicate issues like incorrect input, missing authentication, or a timeout.
500-Something is wrong in the server. Server error codes that indicate that the server encountered an error while processing the client's request. These codes usually indicate temporary or permanent issues with the server, such as being overloaded or unreachable.

2. Status code 202: This status code, "Accepted," is typically used for asynchronous processing. It indicates that the client's request was valid and has been accepted by the server, but the processing of the request will happen at a later time.

3. Status code 308: This status code, "Permanent Redirect," is used to inform the client that the requested resource has permanently moved to a new URL. The client should update its request to use the new URL for future access to the resource.

4. If an update doesn't return data to a client, the appropriate code to use is 204 No Content. This status code indicates that the server successfully processed the request, but there is no content to return in the response.

5. If a resource used to exist but no longer does, the appropriate code to use is 410 Gone. This status code indicates that the resource is gone and will not be available again in the future.

6. The 'Forbidden' status code, 403 Forbidden, indicates that the client does not have the necessary permissions to access the requested resource. It is different from a 401 Unauthorized status code, which indicates that the client needs to provide valid credentials for access.

## build a rest api with nodejs and express and mongodb

[Video Link](https://www.youtube.com/results?search_query=build+a+rest+api+with+nodejs+and+express+and+mongodb)

### Questions

1. Why do we need to pull our MongoDB database string out of our server and put it into our .env?

It is considered a best practice to store sensitive information, such as database connection strings, passwords, and API keys, in environment variables rather than hard-coding them into the source code. By storing the MongoDB database string in the .env file, you separate the configuration from the code, making it easier to manage and maintain. This approach also helps to protect sensitive information from being exposed if the source code is accidentally shared or if the project is hosted on a version control system.

2. What is middleware?

Middleware refers to a piece of code that sits between the request and response objects in an application. It acts as a bridge, intercepting incoming requests, performing certain actions or transformations, and passing the request along to the next middleware or final request handler.

Middleware can be used for various purposes, such as logging, authentication, authorization, error handling, data parsing, and more. It allows developers to modularize their application logic and apply common functionalities across multiple routes or endpoints without duplicating code.

3. What does app.use(express.json()) do?

In the context of an Express.js application, app.use(express.json()) is middleware that parses incoming request bodies containing JSON data. It enables the server to handle JSON payloads sent by clients and transforms them into JavaScript objects, making it easier to work with the data within the application.

By including app.use(express.json()) in the application setup, you ensure that the middleware is applied to all routes, allowing the server to automatically parse JSON data in the request body.

4. What does the /:id mean in a route?
In the context of a route definition in Express.js, /:id represents a route parameter. The colon (:) indicates that it's a variable segment in the URL, and id is the name of the parameter.

For example, if you have a route defined as /users/:id, it means that the route expects a URL like /users/123, where 123 can be any value, and it will be captured and accessible within the route handler as req.params.id. This allows you to dynamically handle requests for specific resources based on their identifiers, such as retrieving a user with a specific ID from a database.

5. What is the difference between PUT and PATCH?
Both PUT and PATCH are HTTP methods used for updating resources in a RESTful API. However, they differ in their semantics and how they handle updates:

PUT: The PUT method is used to completely replace an existing resource with a new representation. When sending a PUT request, the entire resource is typically included in the request payload, and the server replaces the existing resource with the provided data. If a resource with the same identifier already exists, it is overwritten. PUT is considered an idempotent operation, meaning that sending the same request multiple times should have the same effect as sending it once.

PATCH: The PATCH method is used to partially update an existing resource. Unlike PUT, which replaces the entire resource, PATCH allows you to send only the changes or updates that need to be applied. The server then applies the provided changes to the resource, modifying only the specified fields or properties. PATCH requests are not necessarily idempotent, as multiple identical requests may have different effects depending on the initial state of the resource.

6. How do you make a default value in a schema?

The default property

7. What does a 500 error status code mean?

Something is wrong with the internal server. 
8. What is the difference between a status 200 and a status 201?

200 means successful request, 201 means successful creation.

### Things i want to know 


