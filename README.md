# Project_22.02
## Java Chat Application

This project is a simple **multi-client chat application** built in Java using **sockets**.  
It consists of two main components:

- **ChatServer.java** – handles client connections, message broadcasting, and user management.
- **ChatClient.java** – connects to the server and enables real-time chat from the client side.

## Features
- Multi-client support using threads.
- Broadcast messages to all connected clients.
- Usernames for identification.
- Server-side logging of messages and connections.
- Graceful handling of client disconnects.

## How It Works
1. The **server** listens on port `12345` and accepts incoming client connections.
2. Each client is handled in a separate thread, enabling multiple users to chat simultaneously.
3. Messages sent by a client are broadcast to all other connected clients.
4. Clients can see when a user joins or leaves the chat.

## Getting Started

### Prerequisites
- Java 8 or higher installed.
- A terminal/command prompt.

### Running the Server
```bash
javac ChatServer.java
java ChatServer
