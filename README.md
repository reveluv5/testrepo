# <u>**Secure Group Chat Service</u>**

## **Project Description:**
For this coursework, I was required to design and implement a simple multi-user
group chat service using Java secure socket programming.

## **Note:**
I implemented my secure group chat service using JetBrains/IntelliJ IDEA Community
Edition 2022.3.1, so I really recommend using this IDE for your operation of my chat
service as the GUI of this IDE is really helpful in viewing all the clients connected -
thus not making it hard and confusing for you in trying to determine which client you
are testing.

### **How To Run The Chat Service in IntelliJ IDEA:**
1. Import the three classes from the `src` folder in the zipped file - these are
`ChatServer.java`, `ClientHandler.java`, and `ChatClient.java`.
<br> <br>
2. To be able to run the secure chat service, make to change the `KEYSTORE_LOCATION`
and `KEYSTORE_PASSWORD` on lines 22-23 in the [ChatServer](./ChatServer.java) class to
where the location and password is on your computer/laptop. Repeat this for the
`TRUSTSTORE_LOCATION` and `TRUSTSTORE_PASSWORD` on lines 20-21 in the [ChatClient](./ChatClient.java)
class. This will allow the server to authenticate the client(s).
<br> <br>
3. First to run the [ChatServer](./ChatServer.java), simply click on the green play
button next to the declaration of the class, and click on `Run 'ChatServer'`.
<br>
   <img src="C:\Users\salma\IdeaProjects\CS2SNS Coursework\src\images\Step3.png" width="255"/>
<br>![step3b-image](./images/Step3b.png)
<br> <br>
4. Next, to be able to run multiple clients, in the [ChatClient](./ChatClient.java)
class, click on `Edit Configurations` --> `Modify options` --> `Allow multiple instances`,
then click on the green play button next to the declaration of the class and click on
`Run 'ChatClient'`. Then to allow multiple clients to connect, click on the green
play button next to the `Select Run/Debug Configurations` menu; the multiple clients
will be shown in different consoles in the `Run` console window.
<br>
<br><img src="C:\Users\salma\IdeaProjects\CS2SNS Coursework\src\images\Step4.png" width="190"/>
<br><img src="C:\Users\salma\IdeaProjects\CS2SNS Coursework\src\images\Step4e.png" width="170"/>
<br><img src="C:\Users\salma\IdeaProjects\CS2SNS Coursework\src\images\Step4f.png" width="550"/>
<br> <br>
5. Now you can operate the secure group chat service with the number of clients you want. Every
message posted by a client will be encrypted to ensure confidentiality between the client and
server. To simply leave the chat, just click on the `Exit` option on the left hand side of `Run`
console. A message, `SERVER: username has left the chat!` will be broadcast to the other clients
connected on the server. If you are still unsure, you are shown in Step 4 of the following section.

### **EXPECTED OUTPUT:**
1. When a client has connected successfully to the server after entering their username:- 
<br>`ChatClient - salma` console: 
<br><img src="C:\Users\salma\IdeaProjects\CS2SNS Coursework\src\images\output1.png" width="900"/>
<br><br>
`ChatServer` console:
<br><img src="C:\Users\salma\IdeaProjects\CS2SNS Coursework\src\images\output2.png" width="900"/>
<br><br>
2. The first client(s) connected and server are able to see when a new client has joined:-
<br>`ChatClient - bob` console: 
<br><img src="C:\Users\salma\IdeaProjects\CS2SNS Coursework\src\images\output3.png" width="900"/>
<br><br>
`ChatClient - salma` console:
<br><img src="C:\Users\salma\IdeaProjects\CS2SNS Coursework\src\images\output4.png" width="900"/>
<br><br>
`ChatServer` console:
<br><img src="C:\Users\salma\IdeaProjects\CS2SNS Coursework\src\images\output5.png" width="900"/>
<br><br>
3. When a chat member posts a message and the other user(s) are able to view it:-
<br>`ChatClient - salma` console:
<br><img src="C:\Users\salma\IdeaProjects\CS2SNS Coursework\src\images\output6.png" width="900"/>
<br><br>
`ChatClient - bob` console:
<br><img src="C:\Users\salma\IdeaProjects\CS2SNS Coursework\src\images\output7.png" width="900"/>
<br><br>
`ChatServer` console:
<br><img src="C:\Users\salma\IdeaProjects\CS2SNS Coursework\src\images\output8.png" width="900"/>
<br><br>
4. Finally, when a client leaves a chat, the other client(s) connected are notified:-
<br> `ChatClient - salma` console - `bob` leaves the chat:
<br><img src="C:\Users\salma\IdeaProjects\CS2SNS Coursework\src\images\output9.png" width="900"/>
<br><br>
NOTE: HOW TO LEAVE CHAT:-
<br><img src="C:\Users\salma\IdeaProjects\CS2SNS Coursework\src\images\leave-chat.png" width="300"/>
<br><br>






