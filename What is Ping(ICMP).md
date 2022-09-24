# What is a ping?
* **A ping (Packet Internet or Inter-Network Groper) is a basic Internet program that allows a user to test and verify if a particular destination IP address exists and can accept requests in computer network administration. The acronym was contrived to match the submariners' term for the sound of a returned sonar pulse.**

Ping is also used diagnostically to ensure that a host computer the user is trying to reach is operating. Any operating system (OS) with networking capability, including most embedded network administration software, can use ping.

## For example:
* **To find the dot address, such as 205.245.172.72, for any given domain name, Windows users can go to the command prompt screen (start/run/cmd) and enter ping xxxxx.yyy, where xxxxx is the second-level domain name, like "whatis," and yyy is the top-level domain name, like "com."**
# Example:
![070219_SWS_ping-test](https://user-images.githubusercontent.com/104230071/189478116-75201887-16d0-4821-9e02-45825c9e3e15.png)
# Ping on a speed test
* The term is also used to test and determine how fast a data signal travels from one place, like a computer, to another, like a website. Ping is also used to troubleshoot and test connectivity and determine response time.

# How does ping work?
* Ping works by sending an Internet Control Message Protocol (ICMP) Echo Request to a specified interface on the network and waiting for a reply. When a ping command is issued, a ping signal is sent to a specified address. When the target host receives the echo request, it responds by sending an echo reply packet.
# How does ICMP work?
* ICMP is used by a device, like a router, to communicate with the source of a data packet about transmission issues. For example, if a datagram is not delivered, ICMP might report this back to the host with details to help discern where the transmission went wrong. It's a protocol that believes in direct communication in the workplace.
# ICMP and Ping
* Ping is a utility which uses ICMP messages to report back information on network connectivity and the speed of data relay between a host and a destination computer. It's one of the few instances where a user can interact directly with ICMP, which typically only functions to allow networked computers to communicate with one another automatically.
