# cs361_microservice


NOTE: For the microservice to work, please install zeromq in Python using pip -install zmq

NOTE: Make sure microservice must be opened in a separate terminal from the calling application FIRST before main application.

TO REQUEST DATA:
First ensure that client and server are connected to the same socket and TCP Port Numbers. To send out a request we can use the socket.send_string() method 
Any data / string will be received via the socket.recv() and must be decoded using UTF-8.

For example:
*Main Application connects to tcp://localhost:5555
*Microservice should be bind to socket tcp://*:5555



TO SEND DATA:
To send out a request we can use the socket.send_string() method 
Any data / string will be received via the socket.recv() and must be decoded using UTF-8.

The following program listens for a request for random Gen-Z quotes. Once the microservice receives a socket request via ZMQ, the calling application will send a request
to microservice to generate a random quote and send it back. 

Microservice sends back the quote in byte format and must be decoded using UTF-8. In Python it can be decoded using the decode('utf-8','strict') method to receive data in Python string format. 







UML Diagram:
![alt text](https://github.com/darrenmah/cs361_microservice/blob/main/Sequence%20diagram.png)

