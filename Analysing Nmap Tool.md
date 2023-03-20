 Meera E Thimothy    
                              Analysis Of Nmap Tool
  CB.EN.P2CYS22002
                              
a) Explain the subnet and use the NMAP Command to scan the services for the whole subnet.

Subnet is a segmented piece of a larger network. It falls within the class A, B or C range. Ip address are used for subnetting. Systems can communicate within subnetwork but not with other subnetworks. That's why it is more secured.
class A  has ip address ranging from 0.0.0.0 to 127.255.255.255 with subnet mask 255.0.0.0.
class B  has ip address ranging from 128.0.0.0 to 191.255.255.255 with subnet mask 255.255.0.0.
class C  has ip address ranging from 0.0.0.0 to 192.255.255.255 with subnet mask 255.255.255.0.

Nmap allows to scan network and discover everything connected to it. It also give information about what's connected, what services each host is operating, and so on. It gives detail of open ports , live host etc.

![image](https://user-images.githubusercontent.com/57287429/226362565-91eaf040-25e4-4a23-8acd-70fdf054baa1.png)

b) What is a firewall and mention its types. Use the NMAP command to detect that a firewall protects the host.

Firewalls monitor incoming and outgoing network traffic and allow/prohibit data packets based on a set of rules. Firewalls protect networks from external and malicious traffic and data packets while allowing legitimate traffic to pass through.

Types Of Firewalls

i)    packet-filtering Firewalls
ii)   Circuit-level Gateways
iii)  Application-level Gateways (Proxy Firewalls)
iv)   Stateful Multi-layer Inspection (SMLI) Firewalls
v)    Next-generation Firewalls (NGFW)
vi)   Threat-focused NGFW
vii)  Network Address Translation (NAT) Firewalls
viii) Cloud Firewalls
ix)   Unified Threat Management (UTM) Firewalls

![image](https://user-images.githubusercontent.com/57287429/226338668-7b224299-98cf-47a6-85ce-aa51e92af971.png)

c)  Use the NMAP command to scan a network and determinewhich devices are up and running

![image](https://user-images.githubusercontent.com/57287429/226363906-45ff12dd-12db-414c-b03a-648c5e583ea2.png)

d)  What are vertical and horizontal scanning?

Horizontal scanning or network scanning sends requests to the same port on different hosts. Attackers use horizontal scanning to prepare for a mass attack. It is also scanning a group of IPs for a single ports.

Vertical scanning sends requests to different ports on the same host. Attackers use vertical scanning to look for vulnerabilities in a preselected target. It is also scanning single IP being scanned for multiple ports.

f) Use NMAP commands to export the output in XML format

![image](https://user-images.githubusercontent.com/57287429/226341034-f4280861-cf93-4862-87eb-14b33eb56f45.png)

g)  Use the NMAP command to get OS information about a host

![image](https://user-images.githubusercontent.com/57287429/226364878-08d8529b-4c5c-4327-beae-01a09de4cd8b.png)

h) Explain ping sweeping and Perform ping sweeping using Nmap
   
   Ping sweep is a method that establish a range of IP addresses which map to live hosts. The classic tool used for ping sweeps is fping. it is series of pings that are automatically sent to a range of IP addresses instead of manually entering the individual address. Ping sweep can be done using Nmap.
   
   ![image](https://user-images.githubusercontent.com/57287429/226366220-b5d7a299-257f-432e-88fc-ce3e8a5a98b4.png)
 
   1) What is a web application firewall? How do you use Nmap to detect a WAF? Perform WAF fingerprint detection using NMAP?

   A WAF or web application firewall helps protect web applications by filtering and monitoring HTTP traffic between a web application and the Internet. It protects web applications from variety of application layer attacks such as cross-site scripting (XSS), SQL injection, cookie poisoning.
   
   To detect a WAF, we used nmap -sV --script=http-waf-detect <target> command
   
![image](https://user-images.githubusercontent.com/57287429/226403474-4a79d9dc-c7c4-4971-9754-1d70727614ab.png)
   
   To perform WAF fingerprint detection nmap -sV --script=http-waf-fingerprint <target>.
   
   ![image](https://user-images.githubusercontent.com/57287429/226403892-096d564c-baad-4181-a98a-4b2069bccd05.png)

   2) What is EXIF data? Tryto find EXIF data of images on a website using NMAP NSE. 
   
      EXIF (Exchangeable Image File Format) files store important data about photographs. An EXIF file holds all the information about the image itself such as the   exposure level where the photo was taken and settings used. It represents the metadata that is embedded in photos by digital camera manufacturers.
   
 ![image](https://user-images.githubusercontent.com/57287429/226405384-964d0f99-8feb-4195-b677-2a1b6cd25d64.png)
 ![image](https://user-images.githubusercontent.com/57287429/226406162-f9e72000-a5be-42f3-85fa-0f60a508ef07.png)
 
  3) Use NMAP NSE to find all subdomains of the website. 
   
   ![image](https://user-images.githubusercontent.com/57287429/226406775-955950cb-494f-4bb3-981e-7d006b2886d5.png)
   
  4) Perform a vulnerability scan on the target host using NMAP NSE.
   
   ![image](https://user-images.githubusercontent.com/57287429/226402501-1e28fbd1-6d88-472a-83b8-cf666cd10f7f.png)

   
