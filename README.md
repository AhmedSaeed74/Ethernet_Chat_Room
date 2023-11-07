# Ethernet Chat Room

## Overview

The Ethernet Communication Simulator is a Python-based project that allows you to emulate Ethernet communication between devices. It is designed to simulate the exchange of data packets over an Ethernet network, making it a valuable tool for educational and testing purposes.

## Server

### Configuration

- Server listens on all available network interfaces (`0.0.0.0`).
- Default port: 12345.
- Buffer size for message transmission: 1024 bytes.

### Functionality

- The server handles multiple client connections concurrently.
- It broadcasts messages received from one client to all connected clients.
- The server thread waits for incoming connections and creates client threads to handle them.

## Client

### Configuration

- Client connects to the server's IP address and port (`192.168.1.3:12345` by default).
- Buffer size for message transmission: 1024 bytes.

### Functionality

- The client allows users to send and receive messages.
- Separate threads manage sending and receiving messages.
- User input is sent to the server for broadcasting.
- Received messages are displayed in the client's console.

## Usage

1. Start the server script on a machine that will serve as the central server.

2. Start one or more client scripts on different machines to connect to the server.

3. Follow the on-screen prompts to join the chat group, send messages, and communicate with other clients.

4. Enjoy real-time communication with other users in the chat group.

## Implementation Details

- The server listens on a specified IP address and port for incoming connections.
- Clients connect to the server and create threads for sending and receiving messages.
- Messages are broadcast to all connected clients except the sender.
- User input is sent to the server, which then broadcasts it to all clients.
- Real-time messaging is achieved through multi-threading.


Please click the link to make sure everything works perfectly and passes all tests without any problems.

https://drive.google.com/file/d/1wcakvPO9Axfsf9PYHEjMUZC3I0WykRzn/view?usp=drive_link
