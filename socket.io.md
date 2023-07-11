# Socket.io

## Web Sockets

1. What is a Web Socket?

***WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection***

2. Describe the Web Socket request/response handshake and what happens once the connection is established.

***The handshake starts with an HTTP request/response, allowing servers to handle HTTP connections as well as WebSocket connections on the same port. Once the connection is established, communication switches to a bidirectional binary protocol which does not conform to the HTTP protocol.***

3. Web Sockets provide a standardized way for the server to send content to a client without first receiving a ***request*** from that client.

## Socket.io Tutorial

1. What does the event handler io.on() do?
***io.on() is typically used on the server side to listen for incoming events from connected clients***

2. Describe some possible proof of life or proof that the code works as expected.

- Passing unit tests that cover different scenarios and edge cases.
- Executing the code with sample inputs and verifying the expected outputs.
- Reviewing the code logic and design through code reviews.

3. What does socket.emit() do?

*** socket.emit() method is used to send a specific event and its associated data from the server to a specific client in real-time communication using WebSockets or Socket.IO. ***

## Socket.io vs Web Sockets

1. What is the difference between WebSocket and Socket.IO? (think Git and GitHub, or OAuth and Auth0).

***WebSocket: WebSocket is a standardized communication protocol that provides full-duplex communication channels over a single TCP connection. It is supported by most modern web browsers natively. WebSocket allows for low-latency, real-time, and efficient bidirectional communication between clients and servers. It provides a simple, raw, and low-level interface for sending and receiving messages. However, WebSocket does not handle certain features out of the box, such as automatic reconnection, support for older browsers, and built-in fallback mechanisms.***

***Socket.IO:Socket.IO is a library built on top of WebSocket that provides additional features and cross-browser compatibility. It offers a higher-level abstraction over WebSocket and includes features like automatic reconnection, event-based messaging, broadcasting, namespaces, and room management. Socket.IO transparently falls back to alternative transport mechanisms, such as long polling or WebSockets emulation, to support older browsers or network configurations where WebSocket is not available. It simplifies the development process by providing a consistent API across different environments and browsers.***

2. When would you use Socket.IO?

 ***Use Socket.IO when you need additional features, compatibility with older browsers, and an easier API for real-time applications. ***

3. When would you use WebSockets?
***Use WebSocket when you require a lightweight, low-level, native WebSocket implementation for high-performance, direct communication between clients and servers.***