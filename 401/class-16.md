# Class 16 Notes - Serverless Functions

[Back to Home](../README.md)

### [What is Serverless Computing](https://www.ibm.com/topics/serverless)

+ Serverless is a cloud computing application development and execution model that enables developers to build and run application code without provisioning or managing servers or backend infrastructure.
+ Serverless lets developers put all their focus into writing the best front-end application code and business logic they can. All developers need to do is write their application code and deploy it to containers managed by a cloud service provider.
+ Also important: With serverless, developers never pay for idle capacity. The cloud provider spins up and provisions the required computing resources on demand when the code executes, and spins them back down again—called ‘scaling to zero’—when execution stops. The billing starts when execution starts, and ends when execution stops; typically, pricing is based on execution time and resources required.
+ There are not no servers in the serverless model, they are simply abstracted away from the developer.

### Additional Resources

+ [venv - Creation of Virtual Enviroments](https://docs.python.org/3/library/venv.html)
  + The venv module supports creating lightweight “virtual environments”, each with their own independent set of Python packages installed in their site directories. A virtual environment is created on top of an existing Python installation, known as the virtual environment’s “base” Python, and may optionally be isolated from the packages in the base environment, so only those explicitly installed in the virtual environment are available.

+ [Vercel - Get Started](https://vercel.com/docs/concepts/get-started/deploy)
  + Vercel is an end-to-end platform for developers, that allows you to create and deploy your web application. Vercel provides the following features to enable you to serve fast and personalized content to your users:
  + Deployments, CI/CD, Custom Domains, Monitoring your project(Analytics)

+ [http.server](https://pymotw.com/3/http.server/index.html)
  + Base Classes for implementing Web Servers
  + http.server uses classes from socketserver to create base classes for making HTTP servers. HTTPServer can be used directly, but the BaseHTTPRequestHandler is intended to be extended to handle each protocol method (GET, POST, etc.).

+ [Requests: HTTP for Humans](https://requests.readthedocs.io/en/latest/)
  + Requests allows you to send HTTP/1.1 requests extremely easily. There’s no need to manually add query strings to your URLs, or to form-encode your POST data. Keep-alive and HTTP connection pooling are 100% automatic, thanks to urllib3.

+ [Python & APIs](https://realpython.com/python-api/)
  + Knowing how to consume an API is one of those magical skills that, once mastered, will crack open a whole new world of possibilities, and consuming APIs using Python is a great way to learn such a skill.
  + A lot of apps and systems you use on a daily basis are connected to an API. From very simple and mundane things, like checking the weather in the morning, to more addictive and time-consuming actions, such as scrolling through your Instagram, TikTok, or Twitter feed, APIs play a central role.
  + SOAP vs REST vs GraphQL
  + requests and APIs: A match made in heaven

### [What is Serverless? - Video](https://www.youtube.com/watch?v=vxJobGtqKVM)

+ Bare Metal to VM to Containers to Serverless. Interesting view

### Bookmark and Review

+ [Serverless Functions](https://vercel.com/docs/concepts/functions/serverless-functions)
+ [Effective Python Environment](https://realpython.com/effective-python-environment/)
  + This is a great place to start to learn more about shell, setting up your programming environment, etc - there is alot there
