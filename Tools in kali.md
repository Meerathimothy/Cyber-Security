Meera E Thimothy
                                           
                                        Analyzing Tools in Kali  
                                           
CB.EN.P2CYS22002                                                             


1) Information Gathering

a) DNS Analysis

i) dnsenum(domain nameserver enumeration)

   It easily gathers DNS information. It will sca and get all information related to DNS server.It will give 
   Host address
   name server
   mail record
   subdomain search
   Alternate for this tool is dmirty
  
  ii) dnsrecon
  
   This script written in python. It is used to perform a variety of function ranging from security enumeration to basic network         troubleshooting. It is used for Zone transfering(transfering DNS from one server to another) , domain and host bruteforce.
  
iii) fierce

   It is a scanner that helps to locate non-contagious space and hostname against specific domains.it does not perform the    exploitation and do not scan whole network.it is used to locate the target and is a preferred tool for vulnerability check in large networks. 
     
 b) IDS/IPS Identification
 
 i) lbd
 
   Tool is to check whether domain has load balancing enabled or not. Load balancing is technique used in different services for    balancing load among different server. If million of requests coming then it should be splitted to different computer clusters because a single host cannot manage it . So lbd check wheteher load balancing is enable.
 
ii) wafwoof

   This python tool identifies and finger web application firewall products. It automate set of procedure used in finding WAF.
   
C) Live Host Identification

   i) arping
   
   Tool for searching / examining host. It operates at datalink layer. It uses ARP by sending ARP request to destination host and  waiting for ARP replies. Basically Arping sends brocast message first. If an Arp reply received , switch to unicast.
      
  ii) fping(fast ping)
  
   It is used to send icmp request to network hosts. Similar to ping but we are pinging multiple hosts. It will not wait for one ping to complete. It gives you the ability to scan list of hosts and gives which one is alive.

iii) Hping3

Allows to send custom TCP/IP and get replies like that of ping. It is like generator and analyzer for Tcp/Ip
operations performed like 
advance port scanning
Test firewall rule

d) Network And Port scanner

Network scanning detects all active hosts on a network and maps to their IP addresses. Port scanning is sending packets to specific 
ports on a host and analyzing the responses.

i) masscan

masscan is a network port scanner. It scans large area of network so quickly. It is designed defensive and offensive investigation.

ii) nmap

nmap is used to find host and services for sending packets and analysing response. It is mainly used for auditing the security of a device.

e) Osint Analysis

open source intelligence 
collection and analysis of data from open source to produce some intelligence. It is used in business intelligence, national securities, law enforcement.

i) spiderfoot

spiderfoot is a tool that automatically queries over 100 public data sources to gather intelligence on IP addresses, domain names, e-mail addresses, names and more. We will specify the target you want to investigate then SpiderFoot will collect data.

ii) spiderfoot-cli

It show you how to run a scan, view the logs and browse the data all from the comfort of a keyboard.

iii) Theharvester

It is wrapper of different search engines and is used to find out email account, open ports , subdomains etc. It is open source tool. 
It is developed using python. theharvester is used to gather open source intelligence on a company or domain.

f) Route Analysis

It determines the best route from one network location to one or more other locations. It can also calculate the quickest or shortest 
route

i) Netdiscover

A tool used to gather all the information of network like IP address , MAC address . It also give information about clients connected and router. It is quick and simplest tool to use.

ii) Netmask

It is used in computer networks. It gives the class and range of IP address. It provides a method to create subnetworks from large network. Netmask length is defined in up to 24-bit format. The greater the length of netmask the more networks it can accommodate.

 g) SMTP Analysis

swaks

It deals with mail server and administration. This tool make it easy find the unverified mails from lists. Swaks has the ability to create subject and body content.

h) Snmp Analysis

i) Onesixtyone(161)

This tool contain a snmp agent that takes request on UDP. It is a very simple SNMP scanner that only requests the system description value for any specified IP address. It is also used to bruteforce snmp.

2) Vulnerablity Analysis

i) Voip Tool

It is used for the transmission of voice and the multimedia over the internet.

ii) Nikto

It is a free software command-line vulnerability scanner. It is used to scan for dangerous files. It captures and print any cookie received.

ii) Legion

It is an open source tool. It is a testing tool that aids in discovery and exploitation of information systems. It is used to execute vulnerabilities assessment tasks.

3) Web Application Analysis

i) Burpsuite

It is used to perform security testing of web application. It has the ability to intercept and modify HTTP and HTTPS traffic between the browser and web application. It is also used to identify vulnerabilities such as SQL injection, cross-site scripting (XSS) and other web application attacks.

ii) Skipfish

Skipfish is a free, open-source Automated Penetration Testing tool available on GitHub made for security researchers. Skipfish is used for information gathering and testing security of website or webserver. It gives us all the security check that are active and generate report of further security assessment to be done.

4) Database Assessment

i) Sqlmap

It is a free tool that gives of database vulnerability. It will detect and exploit SQLi flaws

5) Password Attacks
 
 i) Cewl 
 
 It is a ruby based tool. It is used to generate custom wordlists. It will crawl a specific URL to defined path and returns a list of wordlist. These wordlist can be used as password cracker. It is preinstalled in kali.
 
 ii) John The Ripper
 
 It help sysyem administrators to find out the weak passwords. It is the most powerful password cracking tool. It does brute forcing a list of password. If the password is short and/or weak, John the Ripper can crack such data quickly.
 
 iii) Wordlists
 
 Wordlist can be referred to as a password dictionary since it is a collection of passwords which is stored as plain text. Wordlists are derived from data breaches.
 
 6) Wireless Attacks

i) Bully

It is a new implementation of WPS bruteforce attack. It is written in c. It exploit the design flaw in wps specification. It will break wps pin to get password.

ii) Aircrack-ng

It is a tool to asses wifi networksecurity. It is used to crack wifi passwords. It is command line based tool. They perform monitoring of packet capturing , attacking, Testing wifi cards and drives and cracking of passwords.

iii) Reaver

Reaver performs a brute force attack against an access point’s WPS pin number. a robust and practical attack against WPS.

7) Reverse Engineering

i) clang

The Clang tool is a open source front end compiler that is used to compile programming languages such as C++, C, Objective C++ and Objective C into machine code. Clang is also used as a compiler for frameworks like OpenMP, OpenCL, RenderScript, CUDA and HIP. 
 Clang works in three different stages:-
The first stage is the front end that is used for parsing source code.
The second stage is the optimizer that is used for optimizing that was generated by the frontend.
The third and final stage is the back end. This is responsible for generating the final code to be executed.

ii) clang++

clang++ compiles code as C++.

iii) NASMshell

Netwide Assembler
It is used to write short assembly code.

8) Exploitation Tools

i) Metasploit Framework

The Metasploit Framework is an open source platform that supports vulnerability research, exploit development and creation of custom security tools. The Metasploit framework is a very powerful tool which can be used by cybercriminals as well as ethical hackers to explore/examine systematic vulnerabilities on networks and servers.

ii) Searchsploit

it is a CLI search tool that allows to make a copy of exploit DB. It also perform detailed offline searches for exploits in the saved Exploit-DB.

iii) Social Engineering Toolkit

The Social-Engineer Toolkit is an open-source penetration testing framework designed for social engineering. SET has number of custom attacks that allows to make quick attack. This is only for testing purposes and can only be used where strict consent has been given.

9) Sniffing And Spoofing

i) Dnschef

Itis a highly configurable DNS proxy for Penetration Testers and Malware Analysts. This application developed in Python. It can modify or proxy the dns configuration.

ii) netsniff-ng

netsniff-ng is a fast, minimal tool to analyze network packets, capture pcap files, replay pcap files, and redirect traffic. netsniff-ng is Linux specific.

iii) Responder

Responder is a python tool. It is capable of collecting credentials through Man in the Middle (MiTM) attack within the Windows networks. It will answer to specific NetBIOS Name Service queries based on their name suffix.

10) Forensic Tool

i) Autopsy

It is used by law enforcement, military corporate examiners to investigate what happened on a computer. It gives all the vulnerabilities , malicious activity etc. we can even use it to recover photos from camera's memory card.

ii) Binwalk

Binwalk is a fast and easy-to-use tool for analyzing, reverse engineering and extracting firmware images. Binwalk can scan files and filesystem images to find different built-in filetypes etc. It is also used for searching a given binary image for embedded files and executable code

11) Reporting Tools

i) cutycapt

It is a tool which capture webkit's styling of webpage into a variety of formats including SVG, PDF, PNG, JPEG, GIF and BMP.

ii) Pipal

Pipal is an open source tool built in Ruby for password analysis. This will give stats and information that will help to analyze password

iii) Recordmydesktop

Recordmydesktop is a program that captures audio-video data of a linux desktop session. recordMyDesktop tries to be as unnoticed as possible by proccessing only regions of the screen that have changed
 
 
12) Social Engineering Toolkit
 
 Socialengineeringtoolkit(root)
 
Socialengineertoolkit is an open-source penetration testing framework designed for social engineering. SET has number of custom attacks that allows to make quick attack. This is only for testing purposes and can only be used where strict consent has been given.

