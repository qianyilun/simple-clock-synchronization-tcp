# Java Socket Programming with TCP

## Introduction 
TCP socket is a communication mechanism via stream. A client program can create a TCP socket to connect to the socket of a server.

When the connection is made, the server creates a socket object on its end of the communication. The client and the server can now communicate by writing to and reading an object (or stream) from the socket.

The `java.net.Socket` class represents a socket, and the `java.net.ServerSocket` class provides a mechanism for the server program to listen for clients and establish connections with them.

TCP is a two-way communication protocol. Data can be sent across both streams at the same time.

### Steps

1. The server instantiates a `ServerSocket` object, denoting which `port number` communication is to occur on
2. The server invokes the `accept()` method of the `ServerSocket` class. This method waits until a client connects to the server on the given port
3. After the server is waiting, a client instantiates a `Socket` object, specifying the server name and the `port number` to connect to



## Screenshot

#### Server

Server’s time is what we get from the system time

![server with explain](https://ws4.sinaimg.cn/large/006tKfTcly1g0f02d7m52j31c00u07ih.jpg)

#### Client

Time from server is not the same as the local machine's time. It means clock is synced successfully.

![client with explain](https://ws1.sinaimg.cn/large/006tKfTcly1g0f04yq39zj31c00u01a3.jpg)

## Reference

* https://www.tutorialspoint.com/java/java_networking.htm
* https://www.pegaxchange.com/2017/12/07/simple-tcp-ip-server-client-java/
* http://cs.lmu.edu/~ray/notes/javanetexamples/#date
* https://systembash.com/a-simple-java-tcp-server-and-tcp-client/
