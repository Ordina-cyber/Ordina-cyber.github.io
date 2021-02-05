---
layout: post
title:  "Ransomware: So….what can be done against it?"
author: amir_oulad
categories: [ransomware, cybercrime]
image: assets/images/ransomware.jpg
description: "Ransomware post 2: So….what can be done against ransomware"
featured: true
hidden: false
---

As the old saying goes, to prevent is better than to cure. In order to prevent ransomware, we need to know what the most common attack vectors (methods) are and how attackers are able to infect an organization with ransomware. 
The three most common attack vectors for ransomware are RDP (remote desktop protocol) compromise, email phishing and software vulnerabilities1.  

## a) RDP Compromise 

RDP enables (privileged/admin) users to log into a system remotely and access privileged tools and software. If the necessary RDP security controls haven’t been implemented, there is a 100% chance that criminals will use this vulnerability as an attack vector to compromise the system. <br>

Because RDP compromise occurs remotely, several preventive measures can be taken; 
* Put RDP behind a firewall; 
* Enable the use of a Network Access Control (NAC) system that verifies configuration of a system trying to log into the network; 
* Block the rapid movement of users from one system/network domain to another; 
* Employ a lock-out policy to prevent brute forcing; 
* Requiring strong passwords employ a Password Manager; 
* Employing multifactor authentication (MFA) (use a token based method and not SMS or Voice 
* MFA, as they have been found to be the least secure form of the MFA methods) ; 
* Limiting IP Access (in time and location); 
* Maintain and monitor (monitor means that reviewing must be done of) RDP logs;  
* Monitor the creation/deletion/modification of privileged users and their rights; 
* (preferably physically and logically) separate your systems and networks; 
* Employ a Zero trust architecture; 

## b) Email Phishing 

Attackers pretend to be a reputable entity or a person and distribute emails (or any other form of communication) to users. These emails contain a web link or attachment (such as Word document) includes a malicious script that can perform a variety of functions such as extraction of login credentials and placing malware (ransomware) on the victim’s system. <br>

Because phishing tries to take advantage at the weakest link, your employees, it is of the utmost importance to constantly train and test your employees by means of security awareness training; 

* Perform security awareness training (secure); 
* Perform phishing campaigns (before and after training) thereby testing the awareness of your employees to track the effectiveness of the training and user awareness; 
* Implement content filtering to filter out unwanted attachments, emails with malicious content, spam and unwanted network traffic; 
* Set-up a warning message when an e-mail is received from outside the organization; 
* Restrict the rights and permissions of users regarding the execution/downloading of software on their systems (whitelisting to prevent unknown executables from being executed at endpoints); 
* Restrict the rights and permissions of users regarding accessing of corporate data; 
* Employ a mobile device management tool that manages devices such as laptops, tablets, smartphones 
* Protip: Don’t host your own mail/exchange server; 

## c) Software vulnerabilities 

Unpatched and/or unsupported (end of life/support) software allow attackers to infiltrate networks, thereby enabling the compromise of systems with malware. Possible prevention measures are; 
<br>
* Perform antivirus (AV) scanning running the latest AV dictionaries (Endpoint protection); 
* Perform vulnerability/threat scanning on a continuous basis; 
* Have a complete CMDB system so the inventory of systems are known 
* Have a mature and robust patch & vulnerability management process; 
* Subscribe to threat intelligence services to be aware of the latest security news; 
* Remove /replace unsupported systems; 
* Perform risk assessments to evaluate and manage the probable risks; 
* Apply additional security controls if a system can’t be patched due to business reasons (physical/logical separation, 2FA,…); 
* Shift towards cloudification (PAAS/SAAS/IAAS), where traditional systems (applications, OS, server, infrastructure…) are transported from the local installations from the users’ local systems to the Cloud based services or its web equivalents; 
* Try to outsource non-essential IT services with a reputable IT service provider (please note that the organization remains accountable for the action of the service provider); 
* Employ a mobile application management tool, that secures and enables IT control over enterprise applications on user devices. 
<br>


### If you need any assistance or have any questions regarding ransomware within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).
