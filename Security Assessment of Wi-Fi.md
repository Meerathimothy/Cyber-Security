1. Learn the basic working of Wi-Fi and its types with various types of attacks on it.

Wi-Fi works by using radio waves to transmit data between devices and a wireless access point, which is connected to the internet or a network. The access point acts as 
a central hub that allows devices to connect to the network and communicate with each other. When a device wants to connect to a Wi-Fi network, it sends a request to the 
access point. The access point then assigns the device an IP address and allows it to communicate with other devices on the network.The data that is transmitted between 
devices and the access point is encrypted using various security protocols, such as WEP, WPA, and WPA2.

Types Of Wifi Attacks

a. Eavesdropping: This attack involves intercepting Wi-Fi traffic to steal sensitive information such as passwords, credit card numbers, or other personal data.

b. Man-in-the-middle (MITM) attack: This attack involves intercepting and modifying Wi-Fi traffic to gain access to sensitive information.

c. Rogue access point: This attack involves setting up a fake Wi-Fi network to trick users into connecting to it and stealing their data.

d. Denial-of-service (DoS) attack: This attack involves overwhelming a Wi-Fi network with traffic to disrupt its normal operation.

e. Password cracking: This attack involves using software to guess or crack the Wi-Fi network's password and gain access to the network.

f. Packet injection: This attack involves injecting malicious packets into a Wi-Fi network to exploit vulnerabilities and gain unauthorized access.

2. Perform Wi-Fi fingerprinting using Wigile, Inssider, and Kismet

Wi-Fi fingerprinting is the process of gathering information about the Wi-Fi access points and their characteristics in a particular area.

 Wigle
 
 Wigile is an open-source tool that can be used to map Wi-Fi networks and their characteristics. It uses a GPS device to collect location information and a wireless 
 adapter
 
 
![image](https://user-images.githubusercontent.com/123303806/230722300-6af031f5-bfe6-421d-90e5-ca152ba3239a.png)

Inssider

Inssider is a commercial tool that provides a graphical representation of Wi-Fi networks in the area. It uses a wireless adapter to capture information about nearby networks and displays the information in a user-friendly interface.

Kismet

Kismet is an open-source tool that can be used for network discovery, packet sniffing, and intrusion detection. It can be used to capture and analyze wireless traffic in the area and provide detailed information about nearby Wi-Fi networks. Kismet can identify the SSID, MAC address, channel, encryption type, and signal strength of the nearby networks.

![image](https://user-images.githubusercontent.com/123303806/230722246-081410e6-010b-4cb2-b450-4ddf6d6c87da.png)

iwconfig is similar to ifconfig, but is dedicated to wireless networking interfaces.

![image](https://user-images.githubusercontent.com/123303806/230722254-d2388bf6-9be2-4120-bd4d-684aaffb1ed3.png)

Display and modify IP Addresses using ip a command.

![image](https://user-images.githubusercontent.com/123303806/230722259-5c789eed-9b77-4ed6-95c6-254cfc480072.png)


![image](https://user-images.githubusercontent.com/123303806/230722282-41d26708-414f-4e1b-aa68-3a9b7204d9bb.png)

![image](https://user-images.githubusercontent.com/123303806/230722270-07235d26-7379-4b69-94ae-bfca72f17849.png)

The sudo kismet -c wlan0 command is a Linux command that launches the Kismet wireless network detector and sniffer program on the specified wireless network interface wlan0 with root privileges The "-c" option in the command specifies the channel on which the wireless interface should operate.

![image](https://user-images.githubusercontent.com/123303806/230722288-6d3590b5-efd9-4dd1-bb62-a52050792cab.png)

3. Create an Access point with any Wi-Fi encryption standard and start testing the security of that connection using any Wi-Fi security testing tools,which should include (Aircrack-Ng, Wifite, not limited).Try to capture the 4-way handshake using these methods.

Wi-Fi Encryption Standards:

a. Wired Equivalent Privacy (WEP)

b. Wi-Fi Protected Access (WPA)

c. Wi-Fi Protected Access II (WPA2)

d. Wi-Fi Protected Access III (WPA3)

Wi-Fi Security Testing Tools:

a. Aircrack-ng 

A suite of tools used to assess Wi-Fi network security. It includes packet sniffer, a detector for wireless LANs, WEP and WPA/WPA2-PSK cracker, and an analysis tool for 802.11 wireless LANs.

b. Wifite: 

An automated tool used to attack multiple wireless networks encrypted with WEP, WPA/WPA2-PSK.

**c. Reaver: A tool that cracks WPS (Wi-Fi Protected Setup) keys and allows attackers to gain access to a wireless network using a PIN.

**d.** Wireshark: A network protocol analyzer that captures network traffic in real-time and displays it in a human-readable format.

![image](https://user-images.githubusercontent.com/123303806/230722594-acf00776-1bd1-4db3-8327-aee0bcc7802b.png)

Putting a wired adapter into promiscuous mode. It allows us to see all of the wireless traffic that passes by us in the air. 

![image](https://user-images.githubusercontent.com/123303806/230722600-66090f36-daf1-41d8-a22a-6256c0173dd3.png)

 Grab that traffic by simply using the airodump-ng command.
 
![image](https://user-images.githubusercontent.com/123303806/230722606-ced84e51-8951-4235-9527-8b5b560a45c8.png)

Focus Airodump-Ng on One AP on One Channel.We need the BSSID and channel to do this.

![image](https://user-images.githubusercontent.com/123303806/230722614-7537c96e-05eb-4465-acd5-e2807a83a2bf.png)

In order to capture the encrypted password, we need to have the client authenticate against the AP. If they're already authenticated, we can de-authenticate them (kick them off) and their system will automatically re-authenticate, whereby we can grab their encrypted password in the process.

![image](https://user-images.githubusercontent.com/123303806/230725217-f7b6486b-f3de-4ee2-bc11-39920ee36fc9.png)

Capture the Handshake.

![image](https://user-images.githubusercontent.com/123303806/230722632-09caf9f7-4f1a-4745-9c3d-daa47d4defce.png)

Aircrack-Ng That Password.

![image](https://user-images.githubusercontent.com/123303806/230722637-e6a505ca-9582-429b-a820-3bf56fad4447.png)

4. After capturing the required files for testing, use dictionary generation and password cracking tools to crack the Wi-Fi password.

a. You must use an existing word file to crack the password.

b. Also you have to create your dictionary file for cracking the passwords.

c. Keep 3 different types of passwords for your Wi-Fi to test it. Simple, medium,and complex passwords can be used for testing. Simple can be a dictionary word, medium can be of dictionary word with some numbers, and complex can be generated from any password generator online.

Passwords can be brute-forced but it is probably more efficient to use a dictionary. In Kali, wordlists can be found in /usr/share/wordlists. Fasttrack is good for testing weak passwords.

![image](https://user-images.githubusercontent.com/123303806/230725999-725dd0b4-0da3-42dd-92c7-3b0975df9674.png)

![image](https://user-images.githubusercontent.com/123303806/230726005-0d4e1a8e-f8bb-4e83-a5ff-a5f10dc1b9ea.png)

![image](https://user-images.githubusercontent.com/123303806/230726022-141044bf-f25b-493b-ad2d-f2d8560b6792.png)

![image](https://user-images.githubusercontent.com/123303806/230726014-68f059e4-6df5-47c7-a030-da049df68f63.png)

![image](https://user-images.githubusercontent.com/123303806/230726033-8ab72e2a-6143-400a-afe8-5d0a5bbf362b.png)

![image](https://user-images.githubusercontent.com/123303806/230722318-1afe1d29-356c-4001-9a3e-4860efe0128c.png)

![image](https://user-images.githubusercontent.com/123303806/230722308-db3fd608-2204-4d7a-9566-f8ac98cb08f7.png)

5.Use Rouge AP (WifiPhisher) to create an Evil twin, perform a basic phishing attack using this rouge AP,and document the difference between the two attacks you have performed.

Ans : ![image](https://user-images.githubusercontent.com/123303806/230726047-465c2df1-f362-4dbc-b29d-fbd78909faa3.png)

6.Learn the protocol level working of WPA3 and how it differs from WPA2.

WPA3 (Wi-Fi Protected Access 3) is the latest security protocol for Wi-Fi networks, designed to improve upon the previous security standard, WPA2.The WPA3 protocol is designed to address the vulnerabilities and shortcomings of WPA2, which had become increasingly susceptible to attacks due to the hacking techniques.

a. Stronger Encryption: WPA3 uses the more secure encryption protocol, Simultaneous Authentication of Equals (SAE), which is also known as Dragonfly. SAE uses a stronger Diffie-Hellman key exchange algorithm and provides forward secrecy, which makes it much harder for hackers to intercept and decrypt Wi-Fi traffic.

b. Protection Against Offline Attacks: In WPA2, an attacker can capture the Wi-Fi traffic and use offline brute-force techniques to try and guess the Wi-Fi password. WPA3 addresses this vulnerability by implementing a feature called Simultaneous Authentication of Equals (SAE) which uses a key derivation function to protect against offline dictionary attacks.

c. Improved Authentication: WPA3 introduces a new feature called Opportunistic Wireless Encryption (OWE), which provides encrypted connections without requiring authentication from users. OWE is designed to provide a more secure connection for public Wi-Fi networks, where it can be difficult to distribute pre-shared keys (PSKs) to users.

d. Better Protection Against Password Guessing: WPA3 strengthens the protection against password guessing attacks by implementing a feature called Protected Management Frames (PMF). PMF helps to prevent unauthorized devices from connecting to the network by verifying the authenticity of devices before allowing them to connect.

e. Enhanced Protection for IoT Devices: WPA3 also includes a new feature called Wi-Fi Easy Connect, which provides a simpler and more secure method for connecting IoT devices to Wi-Fi networks. Wi-Fi Easy Connect eliminates the need for users to manually enter long and complex passwords by allowing devices to use a QR code to connect to the network.

