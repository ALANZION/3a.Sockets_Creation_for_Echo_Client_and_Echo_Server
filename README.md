# EX.NO:3a            CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS

## NAME:ALAN ZION H
## REG NO:212223240004

## AIM:
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.

## ALGORITHM:
1. Import the necessary modules in python</br>
2. Create a socket connection to using the socket module.</br>
3. Send message to the client and receive the message from the client using the Socket module in
 server.</br>
4. Send and receive the message using the send function in socket.</br>

## PROGRAM:
### Client

### NAME:ALAN ZION H
### REG NO:212223240004
```
import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
 msg=input("Client > ")
 s.send(msg.encode())
 print("Server > ",s.recv(1024).decode())
```
### Server
```
import socket
s=socket.socket()
s.bind(('localhost',8000))
s.listen(5)
c,addr=s.accept()
while True:
 ClientMessage=c.recv(1024).decode()
 c.send(ClientMessage.encode())
```
## OUPUT:
![image](https://github.com/user-attachments/assets/1f2de386-1b78-4ec7-b420-175e60d89cc1)

## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
