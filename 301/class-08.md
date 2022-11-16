# Class 8 Notes - APIs

[Back to Home](../README.md)

## [API Design Best Practices](https://learn.microsoft.com/en-us/azure/architecture/best-practices/api-design)

1. What does REST stand for?

+ Representational State Transfer

2. REST APIs are designed around a __RESOURCES__.

+ REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.
+ an architectural style for building distributed systems based on hypermedia. REST is independent of any underlying protocol and is not necessarily tied to HTTP. However, most common REST API implementations use HTTP as the application protocol, and this guide focuses on designing REST APIs for HTTP.

3. What is an identifier of a resource? Give an example.

+ A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be: https://adventure-works.com/orders/1

4. What are the most common HTTP verbs?

+ GET, POST, PUT, PATCH, and DELETE.

5. What should the URIs be based on?

+ resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource)

6. Give an example of a good URI.

+ https://adventure-works.com/orders // Good
+ https://adventure-works.com/create-order // Avoid

7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

+ Another factor is that all web requests impose a load on the web server. The more requests, the bigger the load. Therefore, try to avoid "chatty" web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires. Instead, you might want to denormalize the data and combine related information into bigger resources that can be retrieved with a single request. However, you need to balance this approach against the overhead of fetching data that the client doesn't need. Retrieving large objects can increase the latency of a request and incur additional bandwidth costs.

8. What status code does a successful GET request return?

+ Returns HTTP status code 200 (OK)

9. What status code does an unsuccessful GET request return?

+ Returns HTTP status code 204 (No Content)

10. What status code does a successful POST request return?

+ Returns HTTP status code 201 (Created)

11. What status code does a successful DELETE request return?

+ HTTP status code 204 (No Content)

Extra(POST, PUT and Patch)

The differences between POST, PUT, and PATCH can be confusing.

A POST request creates a resource. The server assigns a URI for the new resource, and returns that URI to the client. In the REST model, you frequently apply POST requests to collections. The new resource is added to the collection. A POST request can also be used to submit data for processing to an existing resource, without any new resource being created.

A PUT request creates a resource or updates an existing resource. The client specifies the URI for the resource. The request body contains a complete representation of the resource. If a resource with this URI already exists, it is replaced. Otherwise a new resource is created, if the server supports doing so. PUT requests are most frequently applied to resources that are individual items, such as a specific customer, rather than collections. A server might support updates but not creation via PUT. Whether to support creation via PUT depends on whether the client can meaningfully assign a URI to a resource before it exists. If not, then use POST to create resources and PUT or PATCH to update.

A PATCH request performs a partial update to an existing resource. The client specifies the URI for the resource. The request body specifies a set of changes to apply to the resource. This can be more efficient than using PUT, because the client only sends the changes, not the entire representation of the resource. Technically PATCH can also create a new resource (by specifying a set of updates to a "null" resource), if the server supports this.

PUT requests must be idempotent. If a client submits the same PUT request multiple times, the results should always be the same (the same resource will be modified with the same values). POST and PATCH requests are not guaranteed to be idempotent.

## Bookmark and Review

+ [RegExpr](https://regexr.com/)
+ [Regex Tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)
+ [Regex 101](https://regex101.com/)
