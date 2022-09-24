# Simple Mail Transfer Protocol (SMTP)

* Email is emerging as one of the most valuable services on the internet today. Most internet systems use SMTP as a method to transfer mail from one user to another. SMTP is a push protocol and is used to send the mail whereas POP (post office protocol) or IMAP (internet message access protocol) are used to retrieve those emails at the receiver’s side. 

# SMTP Fundamentals 

* SMTP is an application layer protocol. The client who wants to send the mail opens a TCP connection to the SMTP server and then sends the mail across the connection. The SMTP server is an always-on listening mode. As soon as it listens for a TCP connection from any client, the SMTP process initiates a connection through port 25. After successfully establishing a TCP connection the client process sends the mail instantly. 

# SMTP Protocol 

## The SMTP model is of two types:
* End-to-end method
* Store-and- forward method

* The end-to-end model is used to communicate between different organizations whereas the store and forward method is used within an organization. An SMTP client who wants to send the mail will contact the destination’s host SMTP directly, in order to send the mail to the destination. The SMTP server will keep the mail to itself until it is successfully copied to the receiver’s SMTP. 
* The client SMTP is the one that initiates the session so let us call it client- SMTP and the server SMTP is the one that responds to the session request so let us call it receiver-SMTP. The client- SMTP will start the session and the receiver-SMTP will respond to the request. 

## Model of SMTP system 

* In the SMTP model user deals with the user agent (UA), for example, Microsoft Outlook, Netscape, Mozilla, etc. In order to exchange the mail using TCP, MTA is used. The user sending the mail doesn’t have to deal with MTA as it is the responsibility of the system admin to set up a local MTA. The MTA maintains a small queue of mails so that it can schedule repeat delivery of mails in case the receiver is not available. The MTA delivers the mail to the mailboxes and the information can later be downloaded by the user agents.

![image](https://user-images.githubusercontent.com/104230071/192087166-7f0bf749-f559-42c8-b487-82024d49ad14.png)

# Both the SMTP-client and SMTP-server should have 2 components:

* User-agent (UA)
* Local MTA
* Communication between sender and the receiver : 
**The sender’s user agent prepares the message and sends it to the MTA. The MTA’s responsibility is to transfer the mail across the network to the receiver’s MTA. To send mails, a system must have a client MTA, and to receive mails, a system must have a server MTA.** 

## SENDING EMAIL: 
* Mail is sent by a series of request and response messages between the client and the server. The message which is sent across consists of a header and a body. A null line is used to terminate the mail header and everything after the null line is considered as the body of the message, which is a sequence of ASCII characters. The message body contains the actual information read by the receipt. 

## RECEIVING EMAIL: 
* The user agent at the server-side checks the mailboxes at a particular time of intervals. If any information is received, it informs the user about the mail. When the user tries to read the mail it displays a list of emails with a short description of each mail in the mailbox. By selecting any of the mail users can view its contents on the terminal.

## Some SMTP Commands: 

* HELO – Identifies the client to the server, fully qualified domain name, only sent once per session
* MAIL – Initiate a message transfer, fully qualified domain of originator
* RCPT – Follows MAIL, identifies an addressee, typically the fully qualified name of the addressee, and for multiple addressees use one RCPT for each addressee
* DATA – send data line by line
