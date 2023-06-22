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

Task 5  VFS (Virtual File System)

The VFS is simply a server side cache of the files on the endpoint.GUI to allow inspection of the client’s filesystem.

Below is what you should see when you first access the VFS for a client.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/579455e2-c923-47ab-a12d-636a15dffc81)

 there are 4 folders (or accessors, filesystem access drivers):

file - uses operating system APIs to access files

ntfs - uses raw NTFS parsing to access low level files

registry - uses operating system APIs to access the Windows registry

artifacts - previously run collections. 

Three buttons:-

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/6526a4e2-f15b-4c27-9bed-8138169b0a67)

Refresh the current directory (sync its listing from the client)

Recursively refresh this directory (sync its listing from the client)

Recursively download this directory from the client

1) Which accessor can access hidden NTFS files and Alternate Data Streams? (format: xyz accessor)

    ntfs accessor

2) Which accessor provides file-like access to the registry? (format: xyz accessor)

     registry accessor
     
3) What is the name of the file in $Recycle.Bin?

   Navigate to file, then to C: , then to ntfs folder ,then to recycle bin folder
   
![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/8407416c-b9fe-4124-8dd2-697a93a3d012)

   desktop.ini

4) There is hidden text in a file located in the Admin'sT Documents folder. What is the flag?
 
  Navigate to file, then to C: , then to ntfs folder, then to user folder, then to administrator and then to documents. open flag.txt.hidden file 
 
 ![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/6cf7f397-3e74-4be4-9cf0-228c3646bbd4)

THM{VkVMT0NJUkFQVE9S}Task 6  VQL (Velociraptor Query Language)

Task 6  VQL (Velociraptor Query Language)

VQL is a framework for creating highly customized artifacts, which allow you to collect, query, and monitor almost any aspect of an endpoint, groups of endpoints, or an entire network. It can also be used to create continuous monitoring rules on the endpoint, as well as automate tasks on the server

It is similar to SQL . It also have SELECT, FROM, and WHERE

To execute a simple VQL, first create a Notebook

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/193ab0df-2ff1-4420-b2ca-b6e67c7dee1e)

Notebooks consist of two languages - Markdown and VQL. If you are familiar with Jupyter Notebooks.

Creating notebook

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/25bc4909-45fb-4ab7-a341-386c755d0360)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/19a2ca5d-42e6-4591-b50f-c5b505f2cef0)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/b03758ca-c58d-4c46-9abe-3a0c1ed8170a)

Click into the lower box to display the options for this, then select the pencil to edit

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/b49beb9a-966a-474f-aa59-e625eecd0326)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/fadb9e31-09a1-4758-8b81-c9e57d661e69)

save this notebook and run it against the agent as demonstrated below

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/85d16618-0e5e-4f5d-abfa-fdc78c508be7)

VQL can also be run via the command line.  VQL is run from the command line querying an agent for details such as its hostname.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/ef428866-598d-4104-9e3b-29345715a7a0)

Artifacts

Velociraptor allows packaging VQL queries inside mini-programs called Artifacts. An artifact is simply a structured YAML file containing a query, with a name attached to it. This allows Velociraptor users to search for the query by name or description and simply run the query on the endpoint without necessarily needing to understand or type the query into the UI.

Task 7  Forensic Analysis VQL Plugins

VQL is not useful without a good set of plugins that make DFIR work possible. 

The categories surrounding forensic analysis

Searching Filenames

Searching Content

NTFS Analysis

Binary Parsing

Evidence of Execution

Event Logs

Volatile Machine State

1) What are the arguments for parse_mft()?

parse_mft(filename="C:$MFT", accessor="ntfs")

2) What filter expression will ensure that no directories are returned in the results?

IsDIR

Task8 Hunt for a nightmare

Use Velociraptor to create an artifact to detect the PrintNightmare vulnerability

Below are steps to construct your VQL query to find the DLL: 

The Select clause, the column accessors should be fullpath (concatenate C:/ to the fullpath column accessor) and filename. 

Make sure the column headers for each column accessor are renamed. Fullpath should be Full_Path, and for filename it should be File_Name.

Use parse_pe() to ensure only PE files are returned.

Make sure the column header for this plugin should be renamed to PE. 

The From clause should use parse_mft().

The Where clause should not return any directories, only return binaries (PE files).

Skeleton Query:

SELECT "C:/" + FullPath AS *********,FileName AS *********,parse_pe(file="C:/" + FullPath) AS **

FROM parse_mft(filename="C:/$***", accessor="****")

WHERE *** IsDir

AND FullPath =~ "Windows/System32/spool/drivers"

AND **

This is the complete skeleton query

SELECT “C:/” + FullPath AS Path_Path, FileName AS File_Name,parse_pe(file=”C:/” + FullPath) AS PE From parse_mft(filename=”C:/$MFT”, accessor=”ntfs”) where NOT IsDir AND FullPath =~”Windows/System32/spool/drivers” AND PE
