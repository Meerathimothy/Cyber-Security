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
 
What is the hostname for the client?

THM-VELOCIRAPTOR.eu-west-1.computer.internal

What is listed as the agent version?

2021–04–11T22:11:10Z

In the Collected tab, what was the VQL command to query the client user accounts?

In shell -> whoami and launch

collected -> Windows.System.PowerShell

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/ab7608e0-4ad6-4d8b-b9b5-26b1e416bc2e)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/4ef4d687-07a1-46a4-9da3-7e365278e38b)

"LET Generic_Client_Info_Users_0_0=SELECT Name, Description, Mtime AS LastLogin FROM Artifact.Windows.Sys.Users()"

In the Collected tab, check the results for the PowerShell whoami command you executed previously. What is the column header that shows the output of the command?

While clicking cliendId

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/38e6da0b-033d-4ade-9057-2ff3055cc482)

stdout

In the Shell, run the following PowerShell command Get-Date. What was the PowerShell command executed with VQL to retrieve the result?

click THM-VELOCIRAPTOR.eu-west-1.compute.internal -> shell ->

 -> run Get-Date -> go collected -> state the Get-Date -> log > powershell command
 
 ![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/7da6625c-398d-4bdc-855a-81632af19c69)

Task4 Creating a new collection

Go to client ID and click on collected option. Then add new collection

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/1ee2eb4a-2c02-47e2-ab4c-364143617f63)

There will be 5 stages in this process.

Select Artifacts

Configure Parameters

Specify Resources

Review

Launch

Select Artifacts

In the search bar, type Windows.KapeFiles.Targets

When you select the artifact, a brief description of the collector will be displayed on the right, along with a rundown of the parameters.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/8017d8ae-0f97-46f7-9123-c1e367688a06)

Configure Parameters

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/8129e581-75ff-44c3-868c-e3f61cb8ade7)

Scroll down and check Ubuntu.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/0abf0bed-3bbc-4df1-a789-7736b7969f5e)

Specify Resources

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/9d2a0b6f-d8e5-4a12-9391-ed3a64ffb5f2)

Review

The output will display in JSON format . Only one setting was enabled to collect, which was Ubuntu. 

Launch

Everything should be in order. Now it's time to launch the collection to gather the artifacts. 

When you click Launch, you will be redirected to the Collected view. Notice that there should be a new entry with the newly created collection. 

 It should show an hourglass which indicates the artifacts are actively being gathered for that collection. 

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/c8a5169b-e43e-488d-aa7f-ce11b8aeaec4)

Once the artifacts have been gathered, the state will change from an hourglass to a checkmark like the others. 

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/327ac37a-c143-40fe-bdbb-60c6ff9ff5a4)

1) Earlier you created a new artifact collection for Windows.KapeFiles.Targets. You configured the parameters to include Ubuntu artifacts. Review the parameter description for this setting. What is this parameter specifically looking for?

ubuntu on subwindows system for linux

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/04c361e0-4227-46c5-a676-dd2e4a49865e)

2) Review the output. How many files were uploaded?

20

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/9adbe2fb-7624-48ce-adc8-0e375e7eb01e)
