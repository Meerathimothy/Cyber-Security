                                    Snort
                                   
 SNORT is an open-source, rule-based Network Intrusion Detection and Prevention System (NIDS/NIPS). Snort is the foremost Open Source Intrusion Prevention System (IPS) in the world. Snort IPS uses a series of rules that help define malicious network activity and uses those rules to find packets that match against them and generate alerts for users.
 
Task-Exercises folder

There are two sub-folders available;

Config-Sample - Sample configuration and rule files. These files are provided to show what the configuration files look like.Snort's original base files are located under /etc/snort folder.

Exercise-Files - There are separate folders for each task. Each folder contains pcap, log and rule files ready to play with.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/c29c7ab0-db26-47ef-9cc8-818a4cee4e27)

Traffic Generator

Traffic-generator.sh is used to generate traffic on snort interface.

Running the "traffic generator.sh" file by executing it as sudo. Traffic generator script come in action.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/fb266552-1e76-406c-8450-a4cd6596110e)

opening icmp file

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/517e99e2-06ab-460c-9ad4-1337a303b8a8)
![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/6b88cd90-693a-4b8d-ab00-60b934a78fb5)

 Introduction to IDS/IPS
 
 IDS 
 
 IDS is a passive monitoring solution for detecting possible malicious activities, abnormal incidents etc. . It is responsible for generating alerts for each suspicious event. 
 
 2 types of IDS 
 
 Network Intrusion Detection System (NIDS)
 
 NIDS monitors the traffic flow from various areas of the network. Investigate the traffic on the entire subnet.  If a signature is identified, an alert is created.
 
Host-based Intrusion Detection System (HIDS)

It monitors the traffic flow from a single endpoint device. Investigate the traffic on a particular device. If a signature is identified, an alert is created.

IPS

IPS is an active protecting solution for preventing possible malicious activities/patterns, abnormal activities. It is responsible for stopping/preventing/terminating the suspicious event as soon as the detection is performed.

4 types
Network Intrusion Prevention System (NIPS)

Behaviour-based Intrusion Prevention System(NBA)

Wireless Intrusion Prevention System (WIPS)

Host-based Intrusion Prevention System (HIPS)

Detection/Prevention Techniques

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/9763f6b8-3dce-4dd2-b29f-2c4cbd9d2b45)

Snort has three main use models;

Sniffer Mode - Read IP packets and prompt them in the console application.
Packet Logger Mode - Log all IP packets (inbound and outbound) that visit the network.
NIDS (Network Intrusion Detection System)  and NIPS (Network Intrusion Prevention System) Modes - Log/drop the packets that are deemed as malicious according to the user-defined rules


Which snort mode can help you stop the threats on a local machine?

HIPS

Which snort mode can help you detect threats on a local network?

NIDS

Which snort mode can help you detect the threats on a local machine?

HIDS

Which snort mode can help you stop the threats on a local network?

NIPS

Which snort mode works similar to NIPS mode?

NBA

According to the official description of the snort, what kind of NIPS is it?

full-blown

NBA training period is also known as 

Baselining







