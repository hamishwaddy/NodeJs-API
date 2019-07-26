# API's & GRAPHQL

## **REST CONCEPTS & IDEAS**

- REST API's are all about data, no UI logic is exchanged
- REST API's are normal Node servers which expose different endpoints (HTTP method & path) for clients to send requests to
- JSON is the common data format that is used both for requests and responses
- REST API's are decoupled from the clients that use them
- Most of the server-side code doesn't change from a 'classic' Node app - only request & response data is affected
- The REST API server doesn't care about the client, all requests are handled in isolation, therefore there is no need for 'sessions'
- _Example:_ Build a Complete RESTful API from Scratch: https://academind.com/learn/node-js/building-a-restful-api-with/

---

## **REQUESTS & RESPONSES**

- Attach data in JSON format and let the other end know by setting the 'Content-Type' header
- CORS errors occur when using an API that does not set CORS headers

---

## **AUTHENTICATION**

- Due to no use of 'sessions', authentication is handled differently
- Each request needs to send some data that proves that the request is authenticated
- JSON web tokens (jwt) are a common way of storing authentication info on the client and proving authentication status
- JWT's are signed by the server and can only be validated by the server

---

## **WEB SOCKETS**

- Enables multiple clients to be informed (in realtime) of changes on the server.
- Is a protocol that is built up on top of http - is used as well as, not instead of.
- Http uses 'request, response' to communicate between client & server whereas websockets uses 'push data' to communicate from server to client.
- Socket.io Official Docs: https://socket.io/get-started/chat/
- Alternative Websocket Library: https://www.npmjs.com/package/express-ws

---

## **GRAPHQL**

- Is a stateless, client-independent API
- Higher flexibility that REST API's doue to custom query language that is exposed to the client.
- Queries, Mutations & Subscriptions can be used to exchange and manage data.
- All GraphQl requests are directed thru only one endpoint (POST/graphql).
- The server parses the incoming query expression and calls the appropriate resolvers.
- Detailed Guide on GraphQL: https://graphql.org

## **GraphQL vs REST**

- REST API's great for stati data requirements (e.g. file upload, scenarios where you need same data all the time).
- GraphQL gives higher flexibility by exposing a full query language to the client.
- Both REST & GrpahQL can be implemented with any framework/server-side language

---
