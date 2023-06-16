                     Phishing Analysis Tools
                     
we will outline the steps performed when analyzing a suspicious or malicious email. Information collected from the email header:

Sender email address

Sender IP address

Reverse lookup of the sender IP address

Email subject line

Recipient email address (this information might be in the CC/BCC field)

Reply-to email address (if any)

Date/time

Now we check Email body :-

Any URL links (if an URL shortener service was used, then we'll need to obtain the real URL link)

The name of the attachment

The hash value of the attachment (hash type MD5 or SHA256, preferably the latter)

Tools For Message Header

1) Message Header Analyzer

   IT is a tool from Google that can assist us with analyzing email headers called Messageheader from the Google Admin Toolbox.SMTP message headers, which help identify the root cause of delivery delays. You can detect misconfigured servers and mail-routing problems.

2) Mailheader.org.

3) Ipinfo.io

With IPinfo, you can pinpoint your users’ locations, customize their experiences, prevent fraud, ensure compliance etc.

3) urlscan.io

   It is a free service to scan and analyse websites. When a URL is submitted to urlscan.io, an automated process will browse to the URL like a regular user and record the activity that this page navigation creates. This includes the domains and IPs contacted.

   url2png wannabrowser are also url analysers
   
5) virustotal
 
Analyze suspicious files and URLs to detect types of malware, automatically share them with the security community. Hash of the header is also analysed.

Task 3 Email header analysis

1) What is the official site name of the bank that capitai-one.com tried to resemble?

   captialone.com

Task 4 Email body analysis

How can you manually get the location of a hyperlink

Copy Link Location

Task 5 Malware Sandbox

online malware sandboxeS

1)Any.Run

Analyze a network, file, module, and the registry activity. Interact with the OS directly from a browser.See the feedback from your actions immediately.

2) Hybrid Analysis
   
This is a free malware analysis service for the community that detects and analyzes unknown threats using a unique Hybrid Analysis technology.

3) www.joesecurity.org

Joe Sandbox empowers analysts with a large spectrum of product features.  Live Interaction, URL Analysis & AI based Phishing Detection, Yara and Sigma rules support, MITRE ATTACK, AI based malware detection, Mail Monitor, Threat Hunting & Intelligence, Automated User Behavior
   
Task 6  PhishTool

With automated phishing analysis is PhishTool. PhishTool combines threat intelligence, OSINT, email metadata and battle tested auto-analysis pathways into one powerful phishing response platform.Phis
   
Pishtool connected with VirusTotal using API key


Look at the Strings output. What is the name of the EXE file?

#454326_PDF.exe

Task 7  Phishing Case 1

You are a Level 1 SOC Analyst. Several suspicious emails have been forwarded to you from other coworkers. You must obtain details from each email for your team to implement the appropriate rules to prevent colleagues from receiving additional spam/phishing emails. 

Task: Use the tools discussed throughout this room (or use your own resources) to help you analyze each email header and email body.

Here we are given  a email text file . we paste that in message header analyser. 

1) What brand was this email tailored to impersonate.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/484f9e35-dc3b-4a95-b03f-8989e9e44c80)

Netflix

2) What is the From email address?

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/9cd0d2d6-8829-4978-bfdb-cc428ecb9181)

GQ47wazXe1xYVBrkeDg-JOg7ODDQwWdR@JOg7ODDQwWdR-yVkCaBkTNp.gogolecloud.com

3) What is the originating IP? Defang the IP address.

 Defang means [.] with ip address. 
 
 ![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/ae0f4640-54d9-450f-ba33-6cc61c0449c6)

209[.]85[.]167[.]226

