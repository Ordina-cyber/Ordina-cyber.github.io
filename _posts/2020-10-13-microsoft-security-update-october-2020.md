---
layout: post
title:  "Microsoft Security Update October 2020"
author: maximilian_leire
categories: [ Microsoft-security-update, Microsoft ]
image: assets/images/Microsoft-Patch-Tuesday.png
description: "Microsoft Security Update October 2020"
featured: true
hidden: false
---

As every second Tuesday of the month, the Microsoft security patch has arrived. This month’s patch brings fixes for 87 vulnerabilities, 11 of which are rated critical and 75 are listed as important. There are less vulnerabilities disclosed this month but this is definitely not a reason to let your guard down as there are a few severe bugs that we’ll talk about below that require your immediate attention. 

This month’s focus is on RCE (Remote Code Execution) vulnerabilities as these are often the most dangerous. Numerous of these have been disclosed in a variety of Microsoft software. 

A remote code execution vulnerability allows attackers to execute code on a remote machine where he/she would normally not be allowed to. As seen in the examples below these kinds of vulnerabilities can be found in Windows itself as well as apps like Outlook, Sharepoint, etc. If an attacker were to exploit this kind of vulnerability against a company it could have disastrous consequences such as a complete takeover (including launching an all out ransomware attack) of the internal network if combined with privilege escalation(*) vulnerabilities.

### [CVE-2020-16898](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-16898) | **Windows TCP/IP Remote Code Execution Vulnerability**

This vulnerability is caused by the Windows TCP/IP stack mishandling ICMPv6 Router Advertisement packets. Such packets are periodically sent out or sent on request to devices on the network to advertise their presence. This is harmless and useful when used correctly, but if an attacker alters this packet with specifically crafted code it can allow for remote code execution on a remote Windows computer.

The update in this patch corrects the way Windows TCP/IP stack handles the ICMPv6 Router Advertisement packets which resolves this issue.


### [CVE-2020-16891](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-16891) | **Windows Hyper-V Remote Code Execution Vulnerability**

 This second security flaw is especially interesting since it allows authenticated users on a Hyper-V virtual machine to execute code on the host machine which this guest runs on. Normally virtual machines are seen as safe playgrounds but with vulnerabilities as these we are reminded once again to always stay alert even if we think nothing could go wrong. If this guest runs alongside other business critical virtual machines and something goes wrong with the host of these machines it could have a big impact.

 Luckily an attacker would need authenticated access to a guest machine which mitigates the danger of this vulnerability greatly, but we still recommend to patch this as soon as possible.

### [CVE-2020-16909](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-16909) | **Windows Error Reporting Elevation of Privilege Vulnerability**

In combination with one of the RCE flaws, this vulnerability could allow attackers to elevate their privileges which would allow for much greater damage to be done since the attacker would now have more or full administrator rights. This can be done by running a specially crafted application.

## Microsoft Outlook

Next we will take a look at two Outlook vulnerabilities, one of which stresses the importance of user awareness.

### [CVE-2020-16947](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-16947) | **Microsoft Outlook Remote Code Execution Vulnerability**

When a user executes a specially crafted file with Outlook installed on his/her Windows pc an attacker can execute code remotely with the rights of the user whom executed the file. If this is an administrator this will have a bigger impact than a normal user with restricted rights. This file could be sent to the user via email or be downloaded from a malicious site.

Vulnerabilities like these stress the importance of good user right restrictions and awareness of your companies employees.


### [CVE-2020-16949](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-16949) | **Outlook Denial of Service Vulnerability**

Using this exploit, it is possible for attackers to put your Outlook server out of commission for some time by sending a specially crafted email to it. While Microsoft doesn't clarify how this can be done, the preview pane in Outlook is confirmed to be involved so good user awareness might save yourself from this one as well.

While user awareness can protect you from these vulnerabilities, we still recommend to implement the necessary patches to protect yourself fully as the impact from attacks using these methods can be devastating for your business.


For a list of all vulnerabilities that were disclosed this month [go here](https://portal.msrc.microsoft.com/en-us/security-guidance).

*Privilege escalation is the act of exploiting a bug, design flaw or configuration oversight in an operating system or software application to gain elevated access to resources that are normally protected from an application or user.

### If you need any assistance or have any questions regarding cybersecurity within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).