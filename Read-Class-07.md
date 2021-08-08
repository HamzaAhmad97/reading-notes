## REST

1. Roy Fielding is apparently a smart guy, he helped writing the first web servers which is responsible for sending documents across the internet, he is also one of the authors of the HTTP specification and the originator of the Representational State Transfer architectural style (REST).

2. The techniques that we use today don't work well when we need to be able to talk to all of the machines in the world because we just needed to talk to a small group of machines.

3. There are protocols for sending emails, fetching email, sharing files and so on. HTTP which stands for (hypertext transer protocol) is a protocol for retrieving named resources (chunks of information, like web pages or pictures). It specifies that the side making the request should start with a line like this, naming the resource and the version of the protocol that it is trying to use:

```
GET /index.html HTTP/1.1
```

HTTP treats the network as a streamlike device into which you can put bits and have them arrive at the correct destination in the correct order.

4. GET is the method of the request, it means that we want to get the specified resource.

5. POST -> to send information to the resource.

6. PUT -> to create or replace the resource.

7. PATCH -> considered a set of instructions on how to modify a resource. Contrast this with PUT; which is a complete representation of a resource.

## API Keys

1. yes

2. yes

3. yes

4. yes






