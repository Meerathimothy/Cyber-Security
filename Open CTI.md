Task 1  Room Overview

The concepts and usage of OpenCTI, an open-source threat intelligence platform. 

Task 2  Introduction to OpenCTI

OpenCTI

OpenCTI is another open-sourced platform designed to provide organisations with the means 
to manage CTI through the storage, analysis, visualisation and presentation of threat 
campaigns, malware and IOCs.

The platform's main objective is to create a comprehensive tool that allows users to 
capitalise on technical and non-technical information while developing relationships between
each piece of information and its primary source

Task 3  OpenCTI Data Model

OpenCTI uses a variety of knowledge schemas in structuring data, the main one being the 
Structured Threat Information Expression (STIX2) standards
STIX is a serialised and standardised language format used in threat intelligence exchange. 
It allows for the data to be implemented as entities and relationships

services include:

GraphQL API: The API connects clients to the database and the messaging system.

Write workers: Python processes utilised to write queries asynchronously from the 
RabbitMQ messaging system

Connectors: Another set of Python processes used to ingest, enrich or export data on the
platform. These connectors provide the application with a robust network of integrated 
systems and frameworks to create threat intelligence relations and allow users to improve
their defence tactics

Connectors

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/bcae7396-36a4-4726-b251-7cffae9a962f)

OpenCTI Dashboard 1

Follow along with the task by launching the attached machine and using the credentials provided; log in to the OpenCTI Dashboard via the AttackBox on http://MACHINE_IP:8080/. Give the machine 5 minutes to start up and it is advisable to use the AttackBox on fullscreen.

Username: info@tryhack.io

Password: TryHackMe1234

OpenCTI Dashboard

Once connected to the platform, the opening dashboard showcases various visual widgets summarising the threat data ingested into OpenCTI. Widgets on the dashboard showcase the current state 
of entities ingested on the platform via the total number of entities, relationships, reports and observables ingested, and changes to these properties noted within 24 hours.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/20dfe2df-6109-4534-82db-1c182edeeffd)

Activities & Knowledge

The activities section covers security incidents ingested onto the platform in the form of reports.They allow for easier identification of the source of information by analysts. Analysts can 
add their investigation notes and other external resources for knowledge enrichment.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/85a92086-5eb2-422a-9b31-7aab647ce2ec)

 Events

 Security analysts investigate and hunt for events involving suspicious and malicious activities across their organisational network. Within the Events tab, analysts can record their findings
 and enrich their threat intel by creating associations for their incidents.

 Observations

 Technical elements, detection rules and artefacts identified during a cyber attack are listed under this tab: one or several identifiable makeup indicators

 ![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/22f0b35c-ee4d-4f9f-abb7-8ed4e4f03564)

 Threats

 Threat Actors: An individual or group of attackers seeking to propagate malicious actions against a target

 Intrusion Sets: An array of TTPs, tools, malware and infrastructure used by a threat actor against targets who share some attributes. APTs and threat groups are listed under this category on 
                 the platform due to their known pattern of actions

Campaigns: Series of attacks taking place within a given period and against specific victims initiated by advanced persistent threat actors who employ various TTPs.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/e4276371-cc69-4d31-a89e-fbc0c0f99751)

Arsenal

Malware - Known and active malware and trojan are listed with details of their identification and mapping based on the knowledge ingested into the platform

Attack Patterns: Adversaries implement and use different TTPs to target, compromise, and achieve their objectives

Courses of Action: MITRE maps out concepts and technologies that can be used to prevent an attack technique from being employed successfully.

Tools: Lists all legitimate tools and services developed for network maintenance, monitoring and management. Adversaries may also use these tools to achieve their objectives.

Vulnerabilities: Known software bugs, system weaknesses and exposures are listed to provide enrichment for what attackers may use to exploit and gain access to systems.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/ae1baeb9-8c5c-41fe-ba2a-6c68335a565f)

Entities

This tab categorises all entities based on operational sectors, countries, organisations and individuals. This information allows for knowledge enrichment on attacks, organisations or 
intrusion sets

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/47b6d370-158d-44d4-9352-0d57cd67bbd0)

1) What is the name of the group that uses the 4H RAT malware?

Navigate to arsenal

putter panda

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/db39eeae-ca16-4643-bd77-637003b5c0be)

2) What kill-chain phase is linked with the Command-Line Interface Attack Pattern?

Navigate to arsenal. Go to attack pattern and then to command line interface.

  ![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/fbb6afec-49e4-4de2-9b19-bc12924d4836)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/3f680b0b-d755-4768-9766-aa2074ab2521)
 
execution-ics

3) Within the Activities category, which tab would house the Indicators?

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/6c0da549-a4a0-48f2-b488-ed090a15d713)

observations
