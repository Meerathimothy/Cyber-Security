
 Meera E Thimothy
 
                                        LAN Based Insider Attack
 
 CB.EN.P2CYS22002
 

1) Perform Password stealing (over plaintext) using ARP Cache Poisoning attacks.

   Ettercap is being used as tool. Host is scaned and target is set from the host list . Now arp-poisioning is done. Now  a website is open in target and login with username and password. Now this    username and password is shown in ettercap.
    
    
    ![arp poisioning](https://user-images.githubusercontent.com/57287429/227922818-789e7886-5ac5-47f3-9302-ff0d5ec81878.png)
    
    
2) Perform Denial of Service (DoS) attacks using ARP Cache Poisoning attacks 
   
   It is a cyberattack that makes a computer or other device unavailable to its intended users. Ettercap is being used as tool. Host is scaned and target is set from the host list. Now arp-poisioning is done. Now dos-attack plugin is selected and activated. The victim Ip address is given and an unused ip which is not there in host   list is also given. Now when a browser is opened in target, it will not connect to any site
   
   ![image](https://user-images.githubusercontent.com/57287429/227930716-115da1c2-1067-43c9-83e4-54b07e60f731.png)
 
 ![image](https://user-images.githubusercontent.com/57287429/228022401-bb38ef43-1975-4bd0-a18f-a30920de0444.png)

3) Perform DNS Spoofing attack using ARP Cache Poisoning attacks 

    DNS Attack is any attack targeting the availability or stability of a network's DNS service.
    
    ![image](https://user-images.githubusercontent.com/57287429/227962843-900e4efc-9426-431a-a507-13df4b603db3.png)

    Here I have tried to get the page which we have created instead of the original login page.
    Here  I have created an html page for our ip address in the HTML folder. I have entered the     corresponding website and its spoof ip in the dns page.
    
    ![image](https://user-images.githubusercontent.com/57287429/227964010-8c90aec8-9e23-4a90-bd6f-f4be45fa2b5a.png)

![image](https://user-images.githubusercontent.com/57287429/227964079-5b662a1b-bc6c-4660-af3d-65dd45dc8bce.png)

![image](https://user-images.githubusercontent.com/57287429/227964175-1a57d7c1-de11-4f77-a830-d1c5957cc2bb.png)
    
![image](https://user-images.githubusercontent.com/57287429/227964223-72a7faeb-d0ee-4699-b33d-c57b7ebd4ed7.png)
    
![image](https://user-images.githubusercontent.com/57287429/227964364-9729c171-89a6-4ec4-8313-c3c516e8e61b.png)

4) Invoke ‘sslstrip tool’ for stealing passwordsfrom any machine that is connected toa LAN by stripping the HTTPSconnection. 

   The sslstrip tool is a tool that can be used to perform a man-in-the-middle attack on HTTPS connections by stripping the encryption from the traffic. This allows an    attacker to intercept and read sensitive information such as usernames and passwords. To use Ettercap and ARP Cache Poisoning to invoke the sslstrip tool, you can      follow these steps:

   Install and configure Ettercap on your machine.
   Identify the IP addresses of the target machines that you want to attack.
   Use the arpspoof tool, which is included with Ettercap, to spoof the ARP tables of the target machines. This will redirect network traffic to your machine.

![image](https://user-images.githubusercontent.com/57287429/228022869-1852c11e-0960-4f48-84a3-fb33c7b20b47.png)

![image](https://user-images.githubusercontent.com/57287429/228026786-c21771c2-2f35-48cd-8723-b8417bbc517d.png)

![image](https://user-images.githubusercontent.com/57287429/228022983-8ff88734-f43b-4b45-b58a-9c0f7c83563d.png)

5) Use arp_cop and scan_poisoner plugins to learn about the detection of ARP attacks.

 arp-cop
 
 Report suspicious arp activity.   
 Here kali is set as attacker and seed as victim . Ettercap is being used as tool. In attacker host is scaned and victim's ip address is set as target from the host
 list . Now arp-poisioning is done. Then arp-cop is done. Parallelly we run vicitim in which attackers ip address is set as target. Then arp poisoning is done. Then
 A suspicious activity in victim.
 
   ![image](https://user-images.githubusercontent.com/57287429/228025404-e6aa27c0-9ec4-4e4d-86f5-bc1730d2d71c.png)

 scan_poisioner

 Actively search other poisioners.
 Ettercap is being used as tool. Host is scaned and target is set from the host list . Now arp-poisioning is done. Scan_poisioner plugin is runed. Here no poisioner is  found.
 
 ![image](https://user-images.githubusercontent.com/57287429/228026309-eedb2e4c-5b59-4ad0-924d-534b3062014d.png)


