Task2 Introduction

TheHive Project is a Security Incident Response Platform. 

TheHive Project is a scalable, open-source and freely available Security Incident Response Platform . It is used to track, investigate and act upon identified security incident. It ensuring real-time information applicable to new or existing cases, 

 https://thehive-project.org/
 
 3 core functions for thehive project to work:-
 
 1) Collaborate 
 
 Multiple analysts from one organisation can work together on the same case simultaneously. Through its live stream capabilities,
 every analyst can keep an eye on the cases in real time.
 
 2) Elaborate

 Details of each case can be broken down into associated tasks. Analysts can record their progress, attach artifacts of evidence and assign tasks. 
 
 3) Act

Allow analysts to add observables to their cases, to flag IOCs and identify previously seen observables. 


Which open-source platform supports the analysis of observables within TheHive?

Cortex

Task3 TheHive Features & Integrations

Thehive project has platform rich feature set and integrations to support workflows. These features include:-

1) Case/Task Management

Every investigation is meant to a case that has been created. Each case can be broken down into one or more tasks or can be turned into templates for easier management.

2) Alert Triage

Cases can be imported from SIEM alerts, email reports and other security  sources. In this feature it will go through these imported alerts and decide whether they should be used into investigations or not.

3) Observable Enrichment with Cortex

One of the main feature integrations TheHive supports is Cortex. Cortex allows analysts to collect more information from threat indicators by performing correlation analysis and developing patterns from the cases.

4) Active Response

Run active actions to communicate, share information about incidents and prevent or contain a threat.

5) Custom Dashboard

Statistics on cases, tasks, observables, metrics etc. can be compiled and distributed on dashboards which is  used to generate KPIs within an organisation. 

6) Built-in MISP Integration 

Another useful integration is with MISP. It is a platform for sharing and storing IOC of targeted attacks, financial fraud, vulnerability information or even terrorism information. This integration allows analysts to create cases from MISP events

Other notable integrations that TheHive supports are DigitalShadows2TH & ZeroFox2TH

Task4 User Profiles & Permissions

One of its features is the ability to create organization groups and assign different roles to analysts based on pre-configured user profiles. By creating an organization group in TheHive, administrators can group analysts together based on their roles, departments, or any other criteria relevant to their organization.

 ![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/dc4d9037-15c5-4fa3-8ba3-09dfaea2fa5e)

The pre-configured user profiles are:

Admin: full administrative permissions on the platform. They can't manage any Cases or other data related to investigations.

Org-admin: manage users and all organisation-level configuration. It create and edit Cases, Tasks etc.

Analyst: can create and edit Cases, Tasks, Observables and run Analysis.

Read-only: Can only read, Cases, Tasks and Observables details

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/caad5ba6-7372-48a1-8916-3092a1662af9)

Each user profile has a pre-defined list of permissions that would allow the user to perform different tasks based on their role. When a profile has been selected, its permissions will be listed

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/850e71c2-9ce3-48f1-b8d8-5abf80df7d46)

The list of permissions 

Permission                                Functions

manageOrganisation       -        Create & Update an organisation

manageConfig              -       Update Configuration

manageProfile            -        Create, update & delete Profiles

manageTag             -         Create, update & Delete Tags

manageCase            -          Create, update & delete Cases

manageALert            -         Create, update & import Alerts

manageUser              -        Create, update & delete Users

manageTask               -       Create, update & delete Tasks

manageAnalyse             -       Execute Analyse

manageAction             -        Execute Actions

manageAnalyserTemplate    -   Create, update & delete Analyser Templates


Organisations, configuration, profiles and tags - administrative permission

Actions, analysis and template are available only if the Cortex connector is enabled

Which pre-configured account cannot manage any cases?

admin

Which permission allows a user to create, update or delete observables?

manageobservables

Which permission allows a user to execute actions?

manageaction

Task5  Analyst Interface Navigation

SCENARIO
You have captured network traffic on your network after suspicion of data exfiltration being done on the network. This traffic corresponds to FTP connections that were established. Your task is to analyse the traffic and create a case on TheHive to facilitate the progress of an investigation. If you are unfamiliar with using Wireshark, please check out this room first and come back to complete this task. 

Source of PCAP file: IntroSecCon CTF 2020

Creating new case

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/99fa0e0f-680c-4141-bbe6-5bffd8dcc2b0)

On clicking theNew Case tab, a pop-up window opens, providing the analyst with fields to input their case details and tasks

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/de699780-c8f1-4188-9900-5c1564bdea75)

i)   severity - impact of incident being investigated in environment. It is from low to critical.

ii)  TLP: The Traffic Light Protocol is to ensure that sensitive information is shared with the appropriate audience. The range of colours 
     represents a scale between full disclosure of information (White) and No disclosure/ Restricted (Red).
     
iii) PAP: The Permissible Actions Protocol is used to indicate what an analyst can do with the information. It uses a colour scheme similar 
     to TLP

Creating new task for the secenario

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/0c2d46c0-ea8f-4f7a-b284-994eb46b8331)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/56902d80-082a-4d6c-8076-a0ab31ed0f52)

Next we are adding tactic and technique associated with the case. This provides additional information that can be helpful to map out the threat.

As this is an exfiltration investigation, tactic chosen and followed by the specific T1048.003 technique for Exfiltration Over Unencrypted/Obfuscated Non-C2 Protocol

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/ec3fa594-32fc-4dd0-a623-69d74d5edf69)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/f3e0a5f9-0cd0-4f8d-9ab5-eb15db407718)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/c429cb74-7aa9-4455-959e-63b91705e446)

By clicking add ttp

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/c0fef682-eab0-4db2-8f7e-84255d409903)

Next we are adding case observables from observable table

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/1f4135f8-7347-47f0-bf1c-cd4d86b9a5c6)

In our scenario, we are adding the IP address 192... as our observable as this IP is the source of the FTP requests.

Creating observables

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/dc7bc24e-911e-4f82-8f7c-55964c71df6d)


Where are the TTPs imported from?

 MITRE ATT&CK framework
 
According to the Framework, what type of Detection "Data source" would our investigation be classified under?

Network Traffic

Upload the pcap file as an observable. What is the flag obtained from https://10.10.98.122//files/flag.html

THM{FILES_ARE_OBSERVABLERS}.


