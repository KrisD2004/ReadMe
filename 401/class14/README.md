# Navigation Properties and Routing

## ASP.NET MVC Routing Overview (C#)

The article discusses ASP.NET MVC Routing, which is responsible for mapping incoming web requests to specific controller actions in an ASP.NET MVC application. ASP.NET Routing is enabled in the Web.config file and configured in the Global.asax file.

The default route table is created during the application's start event and includes a predefined route structure: "{controller}/{action}/{id}". This route maps URL segments to controller name, action method, and an "id" parameter. The default values for these parameters are set, allowing for flexibility in URL structure.

Examples illustrate how different URL patterns are matched to controller actions. Various scenarios of controller actions are explored, including those with string parameters, no parameters, nullable integer parameters, and non-nullable integer parameters.

In summary, the article provides an introduction to ASP.NET MVC Routing, highlighting the default route table's role in mapping URLs to controller actions and demonstrating how different URL variations can be handled by controller methods with various parameter types.

## Routing in ASP.NET Core

The article provides an in-depth exploration of Routing in ASP.NET Core, which is responsible for matching incoming HTTP requests to executable endpoints within an application. Key concepts and functionalities related to routing are covered extensively:

## Routing Basics:

Routing is responsible for matching incoming HTTP requests to executable endpoints.
Endpoints are units of executable request-handling code defined and configured in the application.
Endpoints can extract values from the request's URL and generate URLs based on endpoint information.
Routing can be configured using controllers, Razor Pages, SignalR, gRPC Services, and more.

## Routing Concepts:

Routing uses a pair of middleware: UseRouting and UseEndpoints.
UseRouting adds route matching to the middleware pipeline.
UseEndpoints adds endpoint execution to the pipeline.
Endpoints can be selected and executed based on URL and HTTP method.
Route templates define how endpoints are matched.

## Route Templates and Constraints:

Route templates define the structure of URLs that an endpoint can match.
Constraints are rules applied to route segments to narrow down matches.
Route templates can include constraints to validate URL segments.

## Integration with Middleware:

Middleware can run before and after routing to influence or react to the endpoint selection.
Middleware can be used to apply authorization policies based on endpoint metadata.

## Endpoint Metadata:

Endpoints can have metadata attached to them.
Middleware can process endpoint metadata to make decisions during request processing.
Metadata can be of any .NET type and can influence middleware behavior.

## URL Matching Phases:

URL matching occurs in several phases, including matching against route templates and applying constraints.
Matches are processed and narrowed down based on route constraints and additional policies.
The EndpointSelector makes the final decision on the matched endpoint.
The article emphasizes that routing in ASP.NET Core is a powerful mechanism for handling incoming requests and executing corresponding endpoint code. It highlights the interaction between routing and middleware, enabling developers to create flexible and maintainable applications.

Overall, the article provides a comprehensive understanding of ASP.NET Core routing, its features, and its integration with other components of the framework.