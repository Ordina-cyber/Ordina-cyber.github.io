---
layout: post
title:  "Looking back on the SolarWinds Fallout"
author: joshua_adshead
categories: [ cybercrime ]
image: assets/images/worldnight.jpg
description: "Looking back on the SolarWinds Fallout"
featured: false
hidden: false
---

The phrase “A chain is only as strong as its weakest link” is commonly used in the cyber security world how only one weak entry point is needed for a malicious attacker to bring a whole network or company to its knees. But what happens when one of the strong links in the chain gives way?

The SolarWinds incident refers to just that. 

## What’s SolarWinds?

For those who are unaware, SolarWinds is a networking software company who helps its clients  to manage their IT portfolios. It provides a centralized approach to monitoring across an entire IT infrastructure with clients in both the public and private sectors, with a few leading examples being the US Department of Justice and the Centers for Disease Control and Prevention. The majority of the Fortune 500 companies also utilize the many products offered by SolarWinds.

The application in question when the word “SolarWinds” comes to mind for many would be the Orion Platform, known for infrastructure monitoring and the management. Orion allows administrators to remotely access corporate networks and monitor servers, workstations, and network devices.


## The Timeline
The initial origin of the SolarWinds compromise was discovered by a security firm FireEye after becoming victim of a cyber-attack. This led to their penetration testing tools being stolen on 8th December 2020 via a backdoor found on the SolarWinds Orion application.

As a result, SolarWinds made an announcement on 13th December 2020 regarding its ongoing investigation of its  Orion application . Soon after this, it was confirmed that the United States Treasury Department was also affected by the Orion backdoor. The vulnerability was given the name “SunBurst” and many determined this to have been carried out by a hacker group called APT29 (aka Cozy Bear / Russian SVR).

Further investigation revealed that the software versions released between March and June 2020 were tainted by the SunBurst malware which appeared to have been deployed as an update from SolarWinds’ own servers. 

SunBurst malware would activate remote access tools and connect to Command-and-Control servers and mimic legitimate SolarWinds traffic following 12-14 days of inactivity. The attacker would finally get the privileged access to the networks of those affected through SAML token-signing certificates.

Thousands of organisations worldwide were affected by this malware, with the numbers being estimated at roughly 18,000. Some of these organisations are known worldwide such as NATO, EU Parliament, United Kingdom’s Ministry of Defence, and many others.

## How is SunBurst special?
While being frequently heard about cyber-attacks, the SunBurst malware utilized sophisticated methods to reduce the chances of detection.
* Delayed Execution was used where the malware would lay dormant for 12-14 days prior to activation, doing so would prevent the organisation detecting the malware. 
* Anti-Sandbox behaviour was also used which would check if the machine it was installed on is connected to a domain by retrieving the domain name prior to execution. If this was not possible, the malware would remain dormant and not activate.
* DNS Resolution and IP Address checks were used, where if a resolved domain was related to a private IP address in the blacklist, the malware would not execute. Interestingly, if one of many Microsoft related IP addresses were discovered, the malware would also stop.

It was due to these above methods being used that the SunBurst malware spent so long undiscovered on host systems.

## Does this cause any concern for us?
Now, not everyone reading this blog will be from a Cyber Security background. But in no way does that mean that this shouldn’t cause any concern. Afterall, being aware of potential issues can only serve to open our minds and realise that even the strongest of chains can still be broken if the attacker is consistent and endures enough. 

What this means is that, even if you or your client don’t use the SolarWinds products, you should still be aware that attacks like these can still happen to any of the applications you may have installed. 


## How can Ordina help you?
Do not hesitate to [reach out](https://www.ordina.be/diensten/security-and-privacy/) to any of our team members at Ordina Belgium where we will be able to offer you a helping hand with any of your queries. We provide multiple services from a professional and friendly team.
