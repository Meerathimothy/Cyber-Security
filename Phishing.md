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

4) From what you can gather, what do you think will be a domain of interest? Defang the domain.

etekno[.]xyz

5) 
What is the shortened URL? Defang the URL.

hxxps[://]t[.]co/yuxfZm8KPg?amp=1

Task 8  Phishing Case 2

Scenario: You are a Level 1 SOC Analyst. Several suspicious emails have been forwarded to you from other coworkers. You must obtain details from each email for your team to implement the appropriate rules to prevent colleagues from receiving additional spam/phishing emails. 

A malicious attachment from a phishing email inspected in the previous Phishing Room was uploaded to Any Run for analysis. 

Task: Investigate the analysis and answer the questions below. 

1) What does AnyRun classify this email as?
   
![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/b63fd87e-f481-4548-84a1-095135e3fee4)

Suspicious activity

2) What is the name of the PDF file?

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/c91c7c2b-cce5-42cc-bbfb-35db163442b6)

Payment-updateid.pdf

3) What is the SHA 256 hash for the PDF file?

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/2efb72c5-2ea5-4037-8ac7-6d03dd912f2d)

CC6F1A04B10BCB168AEEC8D870B97BD7C20FC161E8310B5BCE1AF8ED420E2C24

4) What two IP addresses are classified as malicious? Defang the IP addresses. (answer: IP_ADDR,IP_ADDR)

On the text report document, find the connections section, get malicious reputation IP

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/f9db72b2-c8ce-4fdf-a27b-ab74bf872b89)

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/d11371d2-6c56-4735-b91e-4cde7a6d0194)

Defang using cyberchef.

2[.]16[.]107[.]24,2[.]16[.]107[.]83

5) What Windows process was flagged as Potentially Bad Traffic?

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/b2a0ccf6-c664-4fef-9a46-a7e305f66e56)

svchost.exe

Task 9  Phishing Case 3

Scenario: You are a Level 1 SOC Analyst. Several suspicious emails have been forwarded to you from other coworkers. You must obtain details from each email for your team to implement the appropriate rules to prevent colleagues from receiving additional spam/phishing emails. 

A malicious attachment from a phishing email inspected in the previous Phishing Room was uploaded to Any Run for analysis. 

Task: Investigate the analysis and answer the questions below. 

1) What is this analysis classified as? 

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/f2e59800-8dee-4874-ad55-6f53a6c022e5)

Malicious Activity

2) What is the name of the Excel file?

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/7193eba0-afa4-46bc-b085-9486329b6a24)
   
CBJ200620039539.xlsx

3) What is the SHA 256 hash for the file?

Click on the excel file. We will get details.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/dcd932c8-25b9-4358-8b45-cf0d2dba196f)

5F94A66E0CE78D17AFC2DD27FC17B44B3FFC13AC5F42D3AD6A5DCFB36715F3EB

4) What domains are listed as malicious? Defang the URLs & submit answers in alphabetical order. (answer: URL1,URL2,URL3)

We will takr text report and check in connections/ DNS request

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/9b64dc81-2022-4253-8a5e-10d1c0331299)

Defanging it 

biz9holdings[.]com,findresults[.]site, ww38[.]findresults[.]site

5) What IP addresses are listed as malicious? Defang the IP addresses & submit answers from lowest to highest. (answer: IP1,IP2,IP3)

We will takr text report and check in connections/ DNS request

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/2f1ee4fb-c5c7-4566-873e-27e908f8b00b)

204[.]11[.]56[.]48,103[.]224[.]182[.]251,75[.]2[.]11[.]242

6) What vulnerability does this malicious attachment attempt to exploit?

For vulnerability exploitation, we take CVE number.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/2b355ae4-033b-4737-a6ee-79b7773da8e6)

CVE-2017–11882

Some other tools

https://mxtoolbox.com/

https://phishtank.com/?

https://www.spamhaus.org/
