 <h1 align="center"> Representational State Transfer (REST)</h1> 

**"REST stands for Representational State Transfer."** It is a software architectural style that defines some set of principles (constraints)  while developing a web service .The goal of REST is to increase **performance, scalability, simplicity, modifiability, visibility, portability, and reliability**.  So any WebService that follows these REST constraints are known as ***RESTful web services***  and the API’s that follow these constraints are  known as ***REST API***.
<br /><br />The representational state transfer terminology was introduced by **Roy Fielding** in 2000 in his doctoral dissertation.

## Architectural Constraints of REST: 
Six guiding constraints have been defined by the REST architecture, which when followed results in a gain of desired non-functional properties like performance, scalability, simplicity, modifiability, visibility, portability, and reliability.

### The following constraints are listed below:
<ul>
  <li>Client-Server</li>
  <li>Stateless</li>
  <li>Cacheable</li>
  <li>Uniform Interface</li>
  <li>Layered System</li>
   <li>Code on Demand</li>
</ul>

The constraint **"Code on Demand"** is optional in the REST architecture. Other than that, if any other constraint is violated, then those services cannot be referred to as RESTful.

### 1] Client-Server :
This is the first constraint in the REST architecture. It provides a **separation of concerns** so that each component evolves independently, and that's what is important for scalability over the internet. Separating the user interface section from the storage section leads to portability of the user interface over multiple platforms and easy scalability of server components.
>client are one's who requests for the resources.<br />
>server is who has the resources.
### 2] Stateless :
This constraint states that the communication between the client and server should be **stateless**. That means whatever request is made by a client to a server should contain all the necessary information to fulfil those requests. So, there is no requirement for stored context on the server side . That brings out **visibility, reliability,** and **scalability** for the server. Visibility is being improved because the system does not have to rely on other requests to fulfil certain requests. Due to this, partial failures are reduced, and since servers do not have to store the state of a request, it can free up resources, which leads to easy scalability.
<br /><br />One disadvantage is that it reduces network performance because the data cannot be stored on the server in a shared context. The client has to send repetitive request . 
### 3]Cache : 
To improve the efficiency, a cache constraint has been added. So it states that whatever data is sent as a response to the request will be labelled as either cacheable or non-cacheable . So if the data has been labeled as cacheable then a client cache is given the right to reuse that response data for later, equivalent requests.
<br /><br />So this constraint has the advantage of completely or partially eliminating client-server interaction. This leads to improved **performance** and **scalability**.
### 4]Uniform Interface :
It is the most fundamental requirement that sets REST apart from other network-based architectural styles. It suggests that no matter what device or type of application is used to interface with a server, there should be a consistent means of doing so (website, mobile app).

### There are four principles of Uniform Interface :-
 * **Identification of resources:** The interface must uniquely identify each resource involved in the interaction between the client and the server.

 * **Resource manipulation through representations:** The client has a representation of the resource and enough information to edit or remove it from the server, if it has authorization to do so. Example: When a user requests a list of users, they typically receive a user id and then use that id to delete or alter that specific person.

* **Self-descriptive Messages:** Each message contains sufficient information to specify how the message should be processed, allowing the server to quickly analyze the request.

* **Hypermedia as the Engine of Application State (HATEOAS):** It should include links for each response so that the client can readily find additional resources.

### 5] Layered System :
This constraint has been added to improve the Internet-scale requirements.It states that the architectural style can be composed of hierarchical layers, restricting each component to knowing only about the layer immediate to it. By restricting knowledge of the system to a single layer, we place a bound on the overall system complexity and promote independence.Multiple layer architecture helps in separating out infrequently used components from the frequently used components and allowing us to make system availability by enabling load-balancing and providing shared caches .
<br /><br />The drawback is that it can lead to overhead and latency in the processing of requests.
### 6] Code-On-Demand :
This is an optional constraint . This constraint states that the server can also provide executable code to the client in the form of applets or client-side scripts such as JavaScript. It reduces the number of features that are required to be pre-implemented. For example, suppose there is a need for support for Java applets. Then the services can be constructed in such a way that they provide the benefit of enhanced functionality via downloadable Java classes. 

<br />Following are the guidelines need to be followed for developing REST based services and API's.
### Reference Links:
This article was prepared using below references :- 
<br />https://en.wikipedia.org/wiki/Representational_state_transfer
<br />https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm
<br />https://www.geeksforgeeks.org/rest-api-architectural-constraints/
 
 
 
 


