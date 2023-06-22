Task1    Introduction

Velociraptor is a unique, advanced open-source endpoint monitoring, digital forensic and cyber response platform. Velociraptor has the ability to
more effectively respond to a wide range of digital forensic and cyber incident response investigations and data breaches

Reconstruct attacker activities through digital forensic analysis

Hunt for evidence of sophisticated adversaries

Investigate malware outbreaks and other suspicious network activities

Monitory continuously for suspicious user activities, such as files copied to USB devices

Discover whether disclosure of confidential information occurred outside the network

Gather endpoint data over time for use in threat hunting and future investigations

Task 2  Deployment

Velociraptor is unique because it can act as a server or a client and it can run on Windows, linux and MacOS.  Velociraptor is also compatible 
with cloud file systems( Amazon EFS and Google Filestore).

Velociraptor running as a server in Linux (Ubuntu) and as a client running Windows.

In Attackbox,

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/fc3299c2-2de1-4eda-85d2-d0fd49c7daef)

In windows client , opening ubuntu server

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/1a920a9b-04ca-4bb4-9985-6f693324f083)

Starting velociraptor

command :- ./velociraptor-v0.5.8-linux-amd64 --config velociraptor.config.yaml frontend -v

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/36741df1-2200-4871-84dd-4f2dc12b1e7c)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/aa33a169-8c58-4f0c-bc46-10fb1d8f9c97)

Now launch Google Chrome and click the Velociraptor shortcut. 

Chrome is likely to show you "Your Connection is not private errors", this is expected and you can proceed to 127.0.01 via the advanced option 
with credentials provided

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/2a636eab-cbf0-4291-80e0-b4b1dfe6e855)

Task 3  Interacting with client machines

some links are grayed out when you first log into Velociraptor.

These links are specific to client endpoints and will become active once the analyst interacts with these endpoints.

Now adding client to velociraptor. The client will be Windows. 

command -  velociraptor-v0.5.8-windows-amd64.exe --config velociraptor.config.yaml client -v

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/4ac7377d-e80b-4dd2-aaee-efd624b86637)

With show all option it will display a list of client machines running the Velociraptor agent

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/1249200f-3631-4b83-9e45-65e419d66369)

When we click on client id , 

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/b6f8168e-0112-47b0-a43a-d074fa22531b)

Overview :- Gives  additional details 

VQL Drilldown

Memory and CPU usage over 24 hours timespan

Orange - Memory usage

Blue - CPU usage

Shell

With the shell, commands can be executed remotely on the client machine. Commands can be run in  PowerShell, CMD, Bash, or VQL.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/38dba2dc-c79b-4111-8a58-a6c8e4937e60)

Collected

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/26c22bfc-3a56-43ed-a583-eed22b751ae4)

Interrogate

 This is for introgating

