# 3b.CREATION FOR CHAT USING TCP SOCKETS
## AIM
To write a python program for creating Chat using TCP Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server
4. Send and receive the message using the send function in socket.
## PROGRAM
```
client.py
import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
    msg=input("Client > ")
    s.send(msg.encode())
    print("Server > ",s.recv(1024).decode())
```
```
server.py
import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
    msg=input("Client > ")
    s.send(msg.encode())
    print("Server > ",s.recv(1024).decode())
```
## OUPUT
<img width="500" height="358" alt="image" src="https://github.com/user-attachments/assets/997a22d3-1155-4914-a632-0bb7435a3d57" />
 <img width="508" height="281" alt="image" src="https://github.com/user-attachments/assets/47cc612e-931f-4c99-85d1-eb482294f817" />


## RESULT
Thus, the python program for creating Chat using TCP Sockets Links was successfully 
created and executed.
