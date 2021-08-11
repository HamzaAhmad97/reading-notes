# APIs

1. REST is short for *Representational State Transfer*, which simply refers to an architecture that is independent of the protocol used to send resources. So for example, we know that the http protocol is used for transferring named resources, however, REST does not rely or is tied to HTTP or any other transfer protocol, in addition, REST is independent of the environment or the client's platform.

2. REST APIs are designed around **resources**, which represents any kind of data.

3. An identifer of a resource is thought of the thing that uniquely identifies or distinguishes a resource, and usually it is the URI (universal resource identifier). This is an example: `https://adventure-works.com/orders/1` which represents a path for a resource on a server.

4. The most common HTTP verbs are GET, POST, PUT, PATCH, and DELETE, and each one of them allows only one unique action.

5. URIs should be based on nouns (resource name) not on actions or verbs like the ones descriped above.

6. An example of a good URI: `htttps://mywebsite.com/clients/history/purchases`

7. *Chatty* APIs are APIs that expose a large number of small resources, and this makes the application send multiple requests which puts load on the app and the server.

8. Successful GET > status code = 200

9. Unsuccessful GET > status code = 404

10. Successful POST > status code = 201

11. Successful DELETE > status code = 204