<div align="center">

![Logo](/sock.png)

</div>

## Sock Idea
- [Organization](https://github.com/Sock-Net)

Sock is a idea, not a code. "Sock" allows you to connect to channels and communicate with other instances. Everyone can make his own "Sock" and "Sock Client". Or you can use [Lightweight Sock Server](https://github.com/Sock-Net/sock) to host a Sock.

## Why Websockets?
Simple, websocket is easy to use in browser. This allows you to host a "Sock" server and manage sock to communicate between back-end and front-end easily.

## Why Not?
Not recommended for embedded devices. But still, [Lightweight Sock Server](https://github.com/Sock-Net/sock) only uses 2MB ram.

## Making a Sock Server
To make a sock server, you must have these routes:
- `/channel/:channel` (WebSocket): This route is where we connect our clients.
- `/api/channel/:channel/:id` (HTTP): This route allows us to get a instance from channel
- `/api/channel/:channel` (HTTP): This route allows us to get all instances from channel

And you must write-read a object that has:
- `type` (int): Type for the instance. Every client has their own types.
- `data` (string): This key can hold any data.
- `from` (string): For see who sent the message.

If type is less than zero (0), Message is for pinging server to keep connection alive.

Please check [Lightweight Sock Server](https://github.com/Sock-Net/sock) to understand how it works.

## Making a Sock Client
And you can make a sock client that allows anything... For example, you can make a sock client that allows to run a python code in channel and send output to other instances.

We made a client that uses "Sock" to send files and data between instances. Check it [here](https://github.com/Sock-Net/sockc)

Please check [Sockc](https://github.com/Sock-Net/sockc) to understand how it works.

## Finishing
You can star project if you liked it!
Sock is a idea, not a code. "Sock" allows you to connect to channels and communicate with other instances. Everyone can make his own "Sock" and "Sock Client". Or you can use [Lightweight Sock Server](https://github.com/Sock-Net/sock) to host a Sock.

## Why Websockets?
Simple, websocket is easy to use in browser. This allows you to host a "Sock" server and manage sock to communicate between back-end and front-end easily.

## Making a Sock Server
To make a sock server, you must have these routes:
- `/channel/:channel` (WebSocket): This route is where we connect our clients.
- `/api/channel/:channel/:id` (HTTP): This route allows us to get a instance from channel
- `/api/channel/:channel` (HTTP): This route allows us to get all instances from channel

And you must write-read a object that has:
- `type` (int): Type for the instance. Every client has their own types.
- `data` (string): This key can hold any data.
- `from` (string): For see who sent the message.

If type is less than zero (0), Message is for pinging server to keep connection alive.

Please check [Lightweight Sock Server](https://github.com/Sock-Net/sock) to understand how it works.

## Making a Sock Client
And you can make a sock client that allows anything... For example, you can make a sock client that allows to run a python code in channel and send output to other instances.

Please check [Sockc](https://github.com/Sock-Net/sockc) to understand how it works.