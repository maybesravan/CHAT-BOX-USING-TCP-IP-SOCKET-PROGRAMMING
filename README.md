# CHAT BOX USING TCP/IP SOCKET PROGRAMMING

## Objective:
- Here the objective is to implement a chat application to allow two persons to chat over a network,
- i.e., CLIENT1 and CLIENT2, with the help of socket programming by using TCP protocols.

## Features:
- **Client-Server Architecture**: The application follows a client-server model where multiple clients can connect to a central server to exchange messages.
- **TCP/IP Protocol**: Communication between the server and clients is facilitated using the TCP/IP protocol, ensuring reliable and ordered delivery of messages.
- **Real-Time Messaging**: Users can send and receive messages in real-time, enabling synchronous communication.
- **Basic Command Line Interface (CLI)**: The chat box provides a simple command-line interface for users to interact with the application.

## Procedure:
- Here client1 and client2 cannot communicate directly, so we need a server to handle client1 and client2.
- There are three versions that can be possible: simplex, half duplex, and full duplex.
- Consider FULL DUPLEX, where Client1 will send messages to the server, and the server will send received messages to Client2 and vice versa.

## Requirements:
- C Compiler.
- Operating System that supports TCP/IP networking (e.g., Linux, Windows)

## How to Use:
- **Compile the Source Code**: Use a C compiler to compile both the server and client source files.
    ```bash
    gcc server.c -o server
    gcc client.c -o client
    ```
- **Run the Server**: Start the server application by executing the compiled server binary.
    ```bash
    ./server <port_number>
    ```
- **Connect Clients**: Launch multiple client instances and connect them to the server using the provided IP address and port number.
    ```bash
    ./client <port_number> <server_ip_address>
    ```
- **Start Chatting**: Once connected, users can start sending and receiving messages through the chat box.

## Important Notes:
- By default, the server listens on a specified port for incoming client connections.
- Clients need to provide the server's IP address and port number to establish a connection.
- Ensure that the firewall settings allow communication on the specified port to avoid connection issues.

## Block Diagram
![image](https://github.com/maybesravan/CHAT-BOX-USING-TCP-IP-SOCKET-PROGRAMMING/assets/81691560/337eeca8-3fc3-4cae-a8b1-d61b421ab73d)
