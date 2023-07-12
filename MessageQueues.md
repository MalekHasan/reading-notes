# Message Queues

## Socket.io Chat Example

1. Explain to a non-technical recruiter what the Chat Example (above) does.
The Chat is an application allows to comunicate betwwen the server and the user in real time communication without any latency or lagging in data.


2. What proof of life are we getting on the backend from the above app?
Once we connect in the server there is an event called connection which is already run and in this application we log in console 'a user connected' to check if the connection was established.

3. Socket.IO gives us the i0.emit() method to send an event to everyone. What flag would you use if you want to send a message to everyone except for a certain emitting socket?
***broadcast***like this:
i0.***broadcast***.emit()

## Rooms

1. What is a room and how might a room be useful?

A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of client.

2. How do you join a room?
You can call a method inside the socket called join and you sholud pass the room ID to this method to join the room.
3. How do you leave a room?

You can call a method inside the socket called leave and you sholud pass the room ID to this method to leave the room.

## Namespaces

1. What is a Namespace and what does it allow you to do?

A Namespace is a communication channel that allows you to split the logic of your application over a single shared connection (also called "multiplexing").

2. Each namespace potentially has its own what? (hint: 3 things)

- event handlers
- rooms
- middlewares

3. Discuss a possible use case for separate namespaces.

we can say like a notification for a different department in organization system we need some  department to know a few something and others not so we by creating a seprate a namespaces for this departments we can send the notification for a specifc department and we avoiding the others depatments users to see all notification for everything.