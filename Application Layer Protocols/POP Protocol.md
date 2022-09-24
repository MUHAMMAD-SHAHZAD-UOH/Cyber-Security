# POP Protocol

* POP is a short form of Post Office Protocol. It is another protocol present at the Application Layer of the OSI reference model.

* POP is mainly a message access protocol.

* POP is basically an internet standard protocol and as we already told you it works on the application layer and is used by the local email software in order to retrieve emails from the remote email server over the TCP/IP connection.

* The Post office Protocol (POP) does not allow any search facility.

* This protocol mainly allows one protocol to be created on the server.

* As this protocol supports offline access to the messages and so less internet usage time is required by this.

* Non-email data is not accessed by this protocol.

* Some of the common clients that make use of POP3 are Gmail, Netscape, Internet Explorer, Eudora.

# History of POP

* The POP(post office protocol) was published in 1984 by Internet Engineering Task Force. After that, it has been updated two times, because the backend developers want to make the layout simple.

* The second version of POP was developed in 1985 and known as POP2 and this version needs the SMTP protocol in order to push the emails.

* Then after the third version of POP was released in 1988 and known as POP3, this version does not require the SMTP protocol. The POP(Post office protocol version 3) is also integrated into famous e-mail software, like Eudora and Outlook Express.

* **And since then(1988) the POP3 is the active version.**
# Working of POP

* All the incoming messages are stored on the POP server until the user login by using an email client and downloads the message to their computer. After the message is downloaded by the user it gets deleted from the server.

* As we know that the SMTP is used to transfer the email message from the server to the server, basically POP is used to collect the email with an email client from the server and it does not include means to send messages.

![image](https://user-images.githubusercontent.com/104230071/192087483-79646994-2fe0-4ba7-b536-68a798265d9f.png)

* If any user tries to check all the recent emails then they will establish a connection with the POP3 at the server-side. The user sends the username and password to the server machine for getting the proper authentication. After getting the connection, users can receive all text-based emails and store them on their local terminal (machine), then finally discard all server copies and then breaks the connection from the server machine.

* In order to retrieve a message from the server following steps are taken;

* Firstly a TCP connection is established by the client using port 110.

* The client identifies itself to the server.

* After that client issues a series of POP3 commands.

![image](https://user-images.githubusercontent.com/104230071/192087527-84143a05-7450-41d8-967d-d4c59a08b568.png)

# Features of POP protocol

* Given below are some of the features provided by the POP protocol:

* The POP protocol uses PORT 110.

* It makes the use of a Persistent TCP connection.
**It is a Pull protocol.**

* It is a connection-oriented protocol.

**The POP protocol is a stateful protocol until the mail is downloaded and across the sessions, it is a stateless protocol.**

