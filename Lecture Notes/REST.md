## API 

- Kitchen -> Interface, Menu -> Functions, Waiter -> Instance 
- System.out.print()

## Story for API:
You have an amazon site.
        * get All products is available.
        * Your friend wants to use it

        1. Create a JAR and give it to him
        2. It won’t work since he doesn’t have DB.
        3. Updating
        * Again JAR and give it to him

Export it as web service.
        * Your friend can use it  
Webservice: Service delivered over the web

consumer -> interface -> implementation 

—————————————————————
Private APIs => Companies
Partner => Insta, Facebook
Public => github

- Swiggy -> Interface, 
—————————————————————
Talk about Internet (TCP connection)
What happens when google.com is typed ?
DNS -> Returns Google.com


## HTTP Methods

| HTTP Methods 	| CRUD Operation 	| Description                  	|
|--------------	|----------------	|------------------------------	|
| POST         	| INSERT         	| Adds to an existing resource 	|
| PUT          	| UPDATE         	| Overrides existing resource  	|
| GET          	| READ           	| Fetches a resource           	|
| DELETE       	| DELETE         	| Delete a resource.           	|

## Status Codes

1xx - Informational codes
2xx	- Successful codes
3xx - Redirection codes
4xx	- Client Error codes
5xx	- Server Error codes

* Mark wants to do an TODO app and integrate with FB
* Webservlet returns HTML (cannot use for other devices)
* need to produce the output in the format that the consumers can understand. Then facebook can call my web service and integrate it.Â 
Web services:
* machine-to-machine (or application-to-application) interaction
* interoperable - Not platform dependent
* should allow communication over a network

consumer -> interface(wont work for different lang) -> WS 

consumer -> XML (Web service description lang) -> WS

Client App UDDI (Universal dependent discovery & integration)
Client Protocol WS

They should be standard formats so that they can be used with varied kind of platforms.Â 
- JSON and XML are quite popular Data Exchange formats.Â 

Not really types but a broad classificationÂ 
- SOAP
- REST


SOAP => Simple Object Access Protocol.Â 
In SOAP, req & res => XML format.Â Â 

WSDL (Web Service Definition Language) to define the format of request xml and the response xml.
Now lets say Facebook wants to know how to call the TODO Service? 
What should I give to the Facebook developer? I will give him a WSDL.
It will explain -
What are the different services (operations) exposed by the server?
How can a service (operation) be called?
What url to use? (also called End Point)
What should the structure of request xml?Â Â 
What should be the structure of response xml?

WSDL methods, args, return type (swagger alike document)

——————————————————

Independence of Language and platform
Based on XML , yet simple and extensible 
Better way to communicate through HTTP that is supported by all internet browsers and serversÂ 

UNIX RPC :
Like a function call, when an RPC is made, the calling arguments are passed to the remote procedure and the caller waits for a response to be returned from the remote procedure.Â  The client makes a procedure call that sends a request to the server and waits.
	requires binary-compatible UNIX implementations at each endpoint
CORBA: 
In distributed computing, an object request broker is a middleware which allows program calls to be made from one computer to another via a computer network, providing location transparency through remote procedure calls.
requires compatible ORBs
RMI:
an API that provides a mechanism to create distributed application in java. The RMI allows an object to invoke methods on an object running in another JVM.
requires JAVA at each end points
DCOM:
programming construct that allows a computer to run programs over the network on a different computer as if the program was running locally.Â 
- requires Windows at each endpointÂ 

envelope indicates the start and the end of the message so that the receiver knows when an entire message has been received.
The SOAP envelope solves the problem of knowing when you are done receiving a message and are ready to process it.

REST:
- Cacheable 
* HTTP responses must be cacheable by the clientsÂ 
* Importance for performance
* If a new request for the resources comes within a while, then the cached response will be returned.

REST vs SOAP are not really comparable.

REST is an architectural style.
Let's compare the popular implementations of REST and SOAP styles.
- RESTful Sample Implementation : JSON over HTTP
- REST is built over simple HTTP protocol.
- REST has better performance and scalability.
- REST reads can be cached.
- REST permits many different data formats (JSON is the most popular choice) where as SOAP only permits XML.

SOAP is a message exchange format.
- SOAP Sample Implementation : XML over SOAP over HTTP
- SOAP services are more complex to implement and more complex to consume.
- SOAP based reads cannot be cached.
- SOAP services have well defined structure and interface (WSDL) and has a set of well defined standards (WS-Security, WS-AtomicTransaction and WS-ReliableMessaging).

Documentation standards with REST are evolving.
