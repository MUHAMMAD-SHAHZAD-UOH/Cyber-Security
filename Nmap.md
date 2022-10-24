# What is Nmap and How to Use it

* Nmap is the most famous scanning tool used by penetration testers.

# What is Nmap?

Nmap is short for Network Mapper. It is an open-source Linux command-line tool that is used to scan IP addresses and ports in a network and to detect installed applications.

* Nmap allows network admins to find which devices are running on their network, discover open ports and services, and detect vulnerabilities.

**Gordon Lyon (pseudonym Fyodor) wrote Nmap as a tool to help map an entire network easily and to find its open ports and services.**

* Nmap has become hugely popular, being featured in movies like The Matrix and the popular series Mr. Robot.
# Why use Nmap?
There are a number of reasons why security pros prefer Nmap over other scanning tools.

* First, Nmap helps you to quickly map out a network without sophisticated commands or configurations. It also supports simple commands (for example, to check if a host is up) and complex scripting through the Nmap scripting engine.

## Other features of Nmap include:

* Ability to quickly recognize all the devices including servers, routers, switches, mobile devices, etc on single or multiple networks.
* Helps identify services running on a system including web servers, DNS servers, and other common applications. Nmap can also detect application versions with reasonable accuracy to help detect existing vulnerabilities.
* Nmap can find information about the operating system running on devices. It can provide detailed information like OS versions, making it easier to plan additional approaches during penetration testing.
* During security auditing and vulnerability scanning, you can use Nmap to attack systems using existing scripts from the Nmap Scripting Engine.
* Nmap has a graphical user interface called Zenmap. It helps you develop visual mappings of a network for better usability and reporting.

# Basic scans
Scanning the list of active devices on a network is the first step in network mapping. There are two types of scans you can use for that:

Ping scan — Scans the list of devices up and running on a given subnet.
|-----------------|
|nmap -sp 192.168.1.1/24 |
Scan a single host — Scans a single host for 1000 well-known ports. These ports are the ones used by popular services like SQL, SNTP, apache, and others.
|> nmap scanme.nmap.org |

![image](https://user-images.githubusercontent.com/104230071/197577984-5dd25445-7a83-4ffd-9dd0-c4ce19c65f4e.png)
|---------|
| OS Scanning
In addition to the services and their versions, Nmap can provide information about the underlying operating system using TCP/IP fingerprinting. Nmap will also try to find the system uptime during an OS scan. |
|> nmap -sV scanme.nmap.org |
* You can use the additional flags like osscan-limit to limit the search to a few expected targets. Nmap will display the confidence percentage for each OS guess.

* Again, OS detection is not always accurate, but it goes a long way towards helping a pen tester get closer to their target.

![image](https://user-images.githubusercontent.com/104230071/197579798-9ff55d1c-ee29-4b06-869a-b78496ed1a1f.png)

## Aggressive Scanning
Nmap has an aggressive mode that enables OS detection, version detection, script scanning, and traceroute. You can use the -A argument to perform an aggressive scan.

> nmap -A scanme.nmap.org

* Aggressive scans provide far better information than regular scans. However, an aggressive scan also sends out more probes, and it is more likely to be detected during security audits.

![image](https://user-images.githubusercontent.com/104230071/197580363-526d76c6-c2fd-4018-b4de-967116d5a136.png)

# Scanning Multiple Hosts
Nmap has the capability of scanning multiple hosts simultaneously. This feature comes in real handy when you are managing vast network infrastructure.

You can scan multiple hosts through numerous approaches:
* Write all the IP addresses in a single row to scan all of the hosts at the same time.
**> nmap 192.164.1.1 192.164.0.2 192.164.0.2**
* Use the asterisk (*) to scan all of the subnets at once.
**> nmap 192.164.1.**
* Add commas to separate the addresses endings instead of typing the entire domains.
**> nmap 192.164.0.1,2,3,4**
* Use a hyphen to specify a range of IP addresses
**> nmap 192.164.0.0–255**
## Port Scanning
**Port scanning is one of the most fundamental features of Nmap. You can scan for ports in several ways.**

* Using the -p param to scan for a single port
**> nmap -p 973 192.164.0.1**
* If you specify the type of port, you can scan for information about a particular type of connection, for example for a TCP connection.
**> nmap -p T:7777, 973 192.164.0.1**
* A range of ports can be scanned by separating them with a hyphen.
**> nmap -p 76–973 192.164.0.1**
* You can also use the -top-ports flag to specify the top n ports to scan.
**> nmap --top-ports 10 scanme.nmap.org**
## Scanning from a File
If you want to scan a large list of IP addresses, you can do it by importing a file with the list of IP addresses.

**> nmap -iL /input_ips.txt**

* The above command will produce the scan results of all the given domains in the “input_ips.txt” file. Other than simply scanning the IP addresses, you can use additional options and flags as well.

## Verbosity and Exporting Scan Results

* Penetration testing can last days or even weeks. Exporting Nmap results can be useful to avoid redundant work and to help with creating final reports. Let’s look at some ways to export Nmap scan results.

## Verbose Output
**> nmap -v scanme.nmap.org**

* The verbose output provides additional information about the scan being performed. It is useful to monitor step by step actions Nmap performs on a network, especially if you are an outsider scanning a client’s network.

![image](https://user-images.githubusercontent.com/104230071/197580534-f8612407-b6a6-4600-982f-3a22cf1c90cc.png)

# Normal output

* Nmap scans can also be exported to a text file. It will be slightly different from the original command line output, but it will capture all the essential scan results.

**> nmap -oN output.txt scanme.nmap.org**

![image](https://user-images.githubusercontent.com/104230071/197580641-cd1ab747-b754-4cd1-9c14-e7b749a071a8.png)

# Nmap Help

* Nmap has a built-in help command that lists all the flags and options you can use. It is often handy given the number of command-line arguments Nmap comes with.

**> nmap -h**

![image](https://user-images.githubusercontent.com/104230071/197580860-086dda65-5dcf-48be-a2f8-65e20f97beb5.png)

# Nmap Scripting Engine

**Nmap Scripting Engine (NSE) is an incredibly powerful tool that you can use to write scripts and automate numerous networking features.*8

* You can find plenty of scripts distributed across Nmap, or write your own script based on your requirements. You can even modify existing scripts using the Lua programming language.

![image](https://user-images.githubusercontent.com/104230071/197581072-ee7c7ce4-104d-4ca5-b9a3-56265ae7c69f.png)

# Conclusion

* Nmap is clearly the “Swiss Army Knife” of networking, thanks to its inventory of versatile commands.

* It lets you quickly scan and discover essential information about your network, hosts, ports, firewalls, and operating systems.

* Nmap has numerous settings, flags, and preferences that help system administrators analyze a network in detail.



