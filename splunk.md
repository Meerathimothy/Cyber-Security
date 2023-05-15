                           Log Analysis using SIEM
CB.EN.P2CYS22002

Meera E Thimothy

1) Understand the architecture of Splunk and the installation process. Setup collector and forwarder,then ensure the logs areaccumulated in Splunk. Familiarize yourself with the dashboard fields.

 Architecture Of Splunk

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/0c6c99a3-65c6-48cd-87fc-065ac186c111)

1) You can receive data from different sources and this process can be set to be automatic data forwarding by executing a few scripts.
2) All the files that are coming can be monitored and real-time detection of changes can be achieved.
3) The forwarder can play an important role to clone the data, capable of load balancing, and intelligently route the data. All these activities can be done before the data being reached out to the indexer.
4) A deployment server is used to manage the entire configuration, deployment, and policies, etc.
5) Once the data is received, it will reach to the indexer. Once the data is indexed, it will be stored in the form of events. This makes it very simple to perform any search activity
6) Using the Search heads, they can be visualized and analyzed using the graphical user interface.
7) Using the Search peers, one will be able to save the searches and will be able to generate reports and also do analysis by visualization dashboard.
8) Using Knowledge objects, you will be able to enrich the existing unstructured data.
9) The search heads and knowledge objects can be accessed via the Splunk web interface. All the communications happen via REST API connection.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/076ace48-af89-4d20-93c4-172edd29353a)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/56a09a24-849a-45e4-89ab-edba76ecdf4e)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/ec171a99-6432-4732-b4c9-8cc131afc50b)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/d57ab861-b6a4-4d02-a644-df7de81103c6)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/2369863f-27fd-485e-a677-e7e1e8baef74)


2) Run Splunk >> Forwarder can be inthe same system or another system(user’s convenience) Make sure the logs are indexing in the Splunk enterprise.

• Run any network and port scanning commands from the host to the target machine. Run at least 5 to 8 commands. (If required,any tools can also beused).

• Use the search section in Splunk to analyze the firewall logs to findthe log of the above process and the exact IP from where the scan was performed. HINT: Use the “stats” command.

• Analyze the log file and create an alert for any further similar activities.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/26bb4cf3-e027-48b9-ac13-fad8ae360602)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/3e8bd69e-9e2d-4eb0-bd8b-cd03711f6194)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/76c57f86-1fd8-4808-838b-ee2be7b282ad)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/65374b81-6988-417e-94bb-7286ee335406)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/f12af4d9-8e0e-4364-a6a5-68e16151cfc0)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/d9261ede-bfd2-4c4d-8a46-593959a78d5c)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/394fe828-7445-4ab9-a822-55072b1d0ac9)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/0d73a6d9-d743-44b0-873d-27efd557edbe)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/764bea95-3821-4a52-aaa5-98bffee6a26f)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/05effa49-e9e6-4b89-9d2b-dc154e577e1d)






