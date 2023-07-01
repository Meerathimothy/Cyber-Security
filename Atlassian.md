Task 1  Introduction

On May the 30th, 2022, an organisation named Volexity identified an un-authenticated RCE vulnerability (scoring 9.8 on NIST) within Atlassian's Confluence Server and Data Center editions.

Confluence is a collaborative documentation and project management framework for teams. Confluence helps track project status by offering a centralised workspace for members.

![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/f9cc6abe-60a9-41cf-be25-8f1d96040934)

1) What is the full CVE entry for this exploit?

 CVE-2022-26134

 2) You discover a server running Confluence with the version of 7.16.2, is this vulnerable? 
Answer format: yay/nay

yay

Task 2  Deploy the Vulnerable Machine

 login page on the following URL loads: HTTP://MACHINE_IP:8090

 ![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/f8ea2e1e-c40e-4dd7-bf78-24f222006908)

 Task 3  Explaining the Vulnerability

 It uses  OGNL (Object-Graph Navigation Language) expression language for Java.OGNL is used for getting and setting properties of Java objects.OGNL is used to bind front-end elements such as text boxes to back-end objects and can be used in Java-based web applications such as Confluence.Values are input to a web form, where these values will be stored into objects within the application

 ![image](https://github.com/Meerathimothy/Cyber-Security/assets/57287429/133b0331-0a0f-40de-aa84-8659bcbad82f)

 1) What does the acronym OGNL stand for?

    Object-Graph Navigation Language

Task 4  Exploit Detection and Patching

  Detection - Log Files

   Confluence is an Apache Tomcat server which has logging located in /opt/atlassian/confluence/logs

   can use commands like grep to search for HTTP GET requests of payloads that are using Java runtime to execute commands. For example:
      
   grep -R "/%24%7B%40java.lang.Runtime%40getRuntime%28%29.exec%28%22"

   Detection - YARA

   If Yara installed on the server running Confluence, Volexity (the finders of the vulnerability) has created the following Yara rule for you to use

   Task 5 Exploitation


