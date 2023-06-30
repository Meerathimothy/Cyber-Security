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

Task5 OpenCTI Dashboard 2

Overview Tab: Provides the general information about an entity being analysed and investigated. In our case, the dashboard will present you with the entity ID, confidence level, description, relations created based on threats, intrusion sets and attack patterns, reports mentioning the entity and any external references

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/7e500fcb-c780-4b4a-b332-7f5679884599)

Knowledge Tab: Presents linked information associated with the entity selected. This tab will include the reports associated, indicators, relations and attack pattern timeline of the entity.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/55363b50-6931-4503-a61c-fba2d5ae93d8)

Analysis Tab: Provides the reports where the identified entry has been seen. The analysis provides usable information about a threat and guides investigation tasks.

Indicators Tab: Provides information on IOC identified for all the threats and entities.

Data Tab: Contains the files uploaded or generated for export that are related to the entity. 

History Tab: Changes made to the element, attributes, and relations are tracked by the platform worker and this tab will outline the changes.

1) What Intrusion sets are associated with the Cobalt Strike malware with a Good confidence level? (Intrusion1, Intrusion2)

Once on the OpenCTI dashboard, look to the panel on the left. we  will see Arsenal. click on it. This will open the Malware section in the main part of the window on the right

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/44e3070c-c87a-4f03-9220-d691f3b2772a)

Using the search bar type Cobalt Strike into it and press enter.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/67afe208-1a7a-48d8-803a-182163c01e7b)

From here we are going to click on the Knowledge tab at the top panel.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/e49fd514-f168-4aca-9996-1c41451cec30)

click on Intrusion sets.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/6cddfd98-7179-4bce-bb13-c95ad0d1c285)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/0a3e58ac-b51a-499c-861e-e405983de4d4)

CopyKittens, FIN7

2) Who is the author of the entity?

   click on the Overview tab.

   ![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/a83c7858-661a-4fd5-8592-a06b8e434bba)

The MITRE Corporation

Task 6  Investigative Scenario

As a SOC analyst, you have been tasked with investigations on malware and APT groups rampaging through the world. Your assignment is to look into the CaddyWiper malware and APT37 group. Gather information from OpenCTI to answer the following questions.


1) What is the earliest date recorded related to CaddyWiper?  Format: YYYY/MM/DD

   The Malware tab is already selected, after you have clicked on the Arsenal tab. So at the top, will be a search bar, type Caddywiper into the search bar and press enter. we will now be at the Overview page of the CaddyWiper Malware, scroll down till you reach the Latest reports about this entity. Will have one result, click on the result.
will now be at the Overview page of the CaddyWiper Malware, scroll down till you reach the Latest reports about this entity.

Once you are down on the Latest Reports about this entity panel, the bottom entry is the one we are looking for. You can see part of the date on it. Click this entry.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/801d1fcc-f2c7-4c03-95aa-e3fbb2de573f)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/85ba2d21-c3bc-4ac1-a533-273d9a153bb1)

2022, March 15

2) Which Attack technique is used by the malware for execution

  Open caddywiper malware.  Go back to the top panel, and click on the Knowledge Tab.When the Knowledge panel loads, a new panel will load on the right side of the screen. On this panel, click the Attack patterns.
  the Attack technique during the execution phase, so scroll over to till you see the Execution column

  Once we reach the Execution column, we will see one of the technique boxes is red, this indicate that it is used in the Caddywiper malware. So the answer is what is written in the red box.

  Native API

 3) How many malware relations are linked to this Attack technique?

Going back to the Execution technique section, click on answer to the previous question.When the page loads for this execution technique, click the Knowledge tab at the top of the page.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/ea2cba73-b1e3-4a68-82ba-6a6e38c6524b)

On the Knowledge page, we will find the answer. You we see three panels at the top of the center of the page, under them is two panels, looking at these two panels look at the one on the right. It is labeled Distribution of Relations, and one of the categories is Malware. Inside that box is a number.

113

4) Which 3 tools were used by the Attack Technique in 2016? (Ans: Tool1, Tool2, Tool3)

   Staying in the Knowledge tab of this technique, look to the right and we will see a panel with different tabs, one of the tabs is labeled Tools. Click on it.

   we have the tools, but we have both 2019 and 2016 mixed in. So to help organize it better, click on the Start time, this will Put the 2019 at the top and the three from 2016 at the bottom

   ShimRatReporter, Empire, Bloodhound

5) What country is APT37 associated with?

   Going back to OpenCTI, look to the panel on the left side of the screen. This time, click on the Threats tab. After we have clicked on the Threats tab, look to the top of the screen, you should see an Intrusion Sets tab, click on it. In search bar, Click in it and type APT37, and press enter to search it.

we will have two results, click on the first one labeled APT37.

When the page loads, will have two panels. Look to the panel on the right labeled Details, the answer can be found under the description within the first sentence

North Korean

6) Which Attack techniques are used by the group for initial access? (Ans: Technique1, Technique2)

   Staying on the APT37, look to the top of the page and click on the Knowledge tab.In the knowledge tab, you will see two large panels. Under these panels on the left are two tabs, click on the Global Kill Chain tab.

   Scroll down till you reach the Initial Access, once you reach this section you will see the answer. They also have start and stop

   T1189, T1566
