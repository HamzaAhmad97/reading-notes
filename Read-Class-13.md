# CRUD

## Status Codes Based On REST Methods

1. Status code groups:

* 100's: (informational status codes) > the server will try to comply with a transmission demand of the client, or that the broswer has received the request and is continuing the process, it is temporary.

* 200's: (success codes) > request was accepted.

* 300's: (redirection codes) > the resource is not available for some reason, and the client is being redirected to another domanin that could be having the resource.

* 400's: (client error codes) > invalid requests sent to the server like a worng URL.

* 500's: (server error codes) > could mean that the server is being overloaded, or that it is receiving so many requests it can not handle.

2. 202 meand that the request has been accepted, but it is usually for the case of asynchronous processing, processing may not have started yet.

3. 308: in case of reading requests, this makes the client use another URL since the resource is not in that server anymore, it is useful when we have more than one location or endpoint so the client does not have to access or read from all of them.

4. The code 204 could be used to indicate that the update does not return data to the client.

5. The code 410 could be used to tell the client that the resource used to exist in the past but now it is not avaialable.

6. The forbidden status code is 403, and it is when the client has no permession to access the resouce even if it is authorized.

--------------------------------------------------------

## Build A REST API With Node.js, Express, & MongoDB - Quick 

1. Because when we deploy we will not use the local host, and will use another url instead, so we add the url to the .env file and then we add that variable to the environment variables in the settings of the depolyment platform.

2. A middleware is a code that the server uses or executes when it receives the request but also before it sends the response, like just for processing and modifying the response before it gets sent.

3. `express. json()` is used to make the server recognize the incoming request object as a json object, this is also a middleware software or code.

4. It allows us to access whatever comes after the slash.

5. Patch allows you to modify or update a single piece of information and not the whole instance, for example, if the user changes or modifies his name, this will allow us to do that without the need for modifying the other information related to the user.

6. To make a defuat value in a schema you should pass the attribute 'default' for that value and give it the value you want it to have by default in case it does not get passed or entered.

7. The status code 500 indicates that there is an error at the serve side, and the server could not complete the transaction.

8. 201 status code indicates that the process was successful but also it means that you have created something, whereas 200 only indicates that we everything was successful in general.

