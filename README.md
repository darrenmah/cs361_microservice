# cs361_microservice


NOTE: For the microservice to work, please install zeromq in Python using pip -install zmq

NOTE: Make sure microservice must be opened in a separate terminal from the calling application FIRST before main application.

The following program listens for a request for random Gen-Z quotes. Once the microservice receives a socket request via ZMQ, the calling application will send a request
to microservice to generate a random quote and send it back. 

Microservice sends back the quote in byte format and must be decoded using UTF-8. In Python it can be decoded using the decode('utf-8','strict') method to receive data in Python string format. 







UML Diagram:

https://github.com/darrenmah/cs361_microservice/blob/main/Sequence%20diagram.png
