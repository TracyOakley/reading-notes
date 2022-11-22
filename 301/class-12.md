# Class 12 Notes - CRUD

[Back to Home](../README.md)

## [Status Codes Based on REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)

In your own words, describe what each group of status code represents:

100’s = information status about header info

200’s = success codes (not that it will process, just it met validation requirements)

300’s = redirection (what you want is not here no more)

400’s =These are the client error codes. They are all about invalid requests a client sent to a server. There are several causes to this, timeouts, wrong URI, missing authentication, etc

500’s = Server side problems

What is a status code 202?

+ 202 Accepted - Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future. The response body should include an URL to the finished resource with some information about when it will be available, or an URL to some monitoring endpoint that tells the client when the resource is available.

What is a status code 308?

+ 308 Permanent Redirect - This is the right code if the resource will now be available at a new URL and the client should directly access it via the new URL in the future. The current endpoint can’t control the clients’ behavior after the request and a subsequent redirect if the resource URL changes again have to be issued from the new URL.


What code would you use if an update didn’t return data to a client?

+ 204 No Content - A proper code for updates that don’t return data to the client, for example when just saving a currently edited document.

What code would you use if a resource used to exist but no longer does?

+ 410 Gone - This is like 404 but we know that the resource existed in the past, but it got deleted or somehow moved, and we don’t know where.

What is the ‘Forbidden’ status code?

+ 403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.


## [Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes](https://www.youtube.com/channel/UCFbNIlppjAuEX4znoulh0Cw)

Why do we need to pull our MongoDB database string out of our server and put it into our .env?

+ So that whomever is using our code can use their own db and not our database.

What is middleware?

+ code that runs when the server gets a request but before routes.

What does app.use(express.json()) do?

+ lets server accepts json as a body inside a post or get

What does the /:id mean in a route?

+ it is a parameter and you can access with req.params.id

What is the difference between PUT and PATCH?

+ Patch only updates the info that is passed and not all the info about the subscriber

How do you make a default value in a schema?

+ just include in the model in the object value a "default: valuewhatever"

What does a 500 error status code mean?

+ error on the server

What is the difference between a status 200 and a status 201?

+ 201 is more specific success created object and 200 is just it was successful
