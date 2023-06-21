Introduction

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

TheHive Features & Integrations

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

 User Profiles & Permissions

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

manageOrganisation               Create & Update an organisation

manageConfig                     Update Configuration

manageProfile                    Create, update & delete Profiles

manageTag                        Create, update & Delete Tags

manageCase                       Create, update & delete Cases

manageALert                      Create, update & import Alerts

manageUser                       Create, update & delete Users

manageTask                       Create, update & delete Tasks

manageAnalyse                    Execute Analyse

manageAction                     Execute Actions

manageAnalyserTemplate          Create, update & delete Analyser Templates

Organisations, configuration, profiles and tags - administrative permission

Actions, analysis and template are available only if the Cortex connector is enabled

Creating a case

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/08e15b86-a606-45d1-a7a2-567b61f11a6b)



















