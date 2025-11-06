Is an Application Programming interface (API). that follows the design principles of the REST architectural style. REST is short for Representational State Transfer, and is a set of rules and guidelines about how you should build a web API.

What's an API?
An API is a set of definition and protocols for building and integrating application sofware. It's sometimes reffered to as a contract between an information provider and an Information user - establishing the content required from the consumer (the call) and the content require by the producer (the response).

What's REST ?
Is a set of architectural constraints, not a protocol or a standart. API developers can implement REST in a variety of ways.

When a client request is a made via a RESTfull API, it transfers a representation of the state of the resource to the requester or endpoint. This informatio, or representation, is delivered in one of several formats via HTTP : 

- JSON (Javascript Object Notation) / most popular format
- HTML
- XLT
- Python
- PHP
- Plain text

In order for an API to be considered RESTful. it has to conform to these criteria:
- A client-server architecture made up of clients, servers, and resources, with request managed through HTTP
- Statelss client-server communication, meaning no client information stored between get requests and each request is separated and unconnected
- Cacheable data that steamlines client-server interactions.
- A uniform interface between components so that information is transferred in a standart form. This requires that:
	- Resources requested are identifiable and separate from the representations sent to the client
	- Resources can be manipulated by the client vie the representation they receive because the representation contains enogh information to do so
	- Self-descriptive messages returned to the client have enough information to describe how the client shoul process it.
	- Hypertext/hypermedia is avalaible, meaning that after accessing a resource the client should be able to use hyperlinks to find all other currently avalaible actions they can take.
- A layered system that organizes each type of server (those responsible for security, load - balancing,etc.) involved the retrieval of request information into hierarchies, invisible to the client
- Code-on-demand (optional): the ability to send executable code from the server to the client when requested, extending client functionality
