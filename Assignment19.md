# Read19

## WebSockets
**WebSocket is a communications protocol. It is useful for opening persistent two-way connections between web client and server.**

## Why do you need WebSockets?
- the server needs to be able to approach the client with the message as soon as someone sends it to them.
- WebSocket protocol seeks to fix these issues. The whole purpose of it is to allow for one persistent two-way connection.

## A high-level overview of the WebSocket protocol
- The client first sends a special request called a handshake. 
- You can think of the handshake as the client asking the server to talk via WebSocket. 
- If the response is successful then the server opens up the WebSocket connection for as long as they need it. 
- With the connection open, the client and server send messages to URL endpoints just like HTTP.

## STOMP protocol
**STOMP (simple text orientated messaging protocol) is a sub-protocol much like HTTP. Each time either party sends data, they must send it in the form of a frame. A frame takes a structure like an HTTP request.**

## Implementing WebSockets in Spring
First, we need to create a new Spring Boot project from the Spring initializer. The only dependency we will need for now is the spring-boot-starter-websocket dependency. Next, you need to create a configuration class to register our STOMP endpoints and to allow us to use an extra tool called sockjs.

What sockjs does is it allows for backup plans in case the client cannot connect via WebSocket. If this happens it will try to connect using another protocol to try to mimic a WebSocket connection. This is particularly useful if we want to allow the use of older browsers that do not support WebSockets.