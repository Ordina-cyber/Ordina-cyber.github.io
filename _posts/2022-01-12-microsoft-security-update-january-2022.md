---
layout: post
title:  "Microsoft Security Update January 2022"
author: maximilian_leire
categories: [ Microsoft-security-update, Microsoft ]
image: assets/images/Microsoft-Patch-Tuesday.png
description: "Microsoft Security Update January 2022"
featured: false
hidden: false
---

For the first patch Tuesday of the year Microsoft released patches for 96 vulnerabilities. Of these CVE's 9 are rated as critical


## [CVE-2022-21907](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2022-21907) | HTTP Protocol Stack Remote Code Execution Vulnerability
A very critical bug to start the Year with, this vulnerability could allow an attacker to execute malicious code on a target system by sending specially crafted network packets. If the targeted server utilises the HTTP Protocol Stack (http.sys) to process these packets, an attacker can execute malicious code on the machine without having any authentication or user interaction required.

Since this is a service running with higher privileges than a normal user this bug is wormable as well.

Attacks will probably mostly be aimed at Windows Servers but Windows 10/11 are potentially vulnerable to this as well depending on the configuration so make sure to check your endpoints as well as your servers.

This is definitely the most critical vulnerability of this patch so make sure to prioritize this one.


## [CVE-2022-21849](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2022-21849) | Windows IKE Extension Remote Code Execution Vulnerability
Another remote code execution vulnerability in Windows has been patched this month. Luckily this one only applies if your system has the IPSec service running.

If you use IPSec within your company make sure the devices running this service are patched as soon as possible.


## [CVE-2022-21846](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2022-21846) | Microsoft Exchange Server Remote Code Execution Vulnerability
Another Year, another Microsoft Exchange Server remote code execution vulnerability. This is one of three RCE vulnerabilities on Exchange servers being patched this month.

The attack vector for these vulnerabilities is listed as 'network' by Microsoft so an attacker would need direct network access to your server to be able to exploit these which makes exploitation less likely than the vulnerabilities that reached the headlines last year.

But nonetheless make sure to patch your servers as soon as possible to stay secure.


For a list of all vulnerabilities that were disclosed this month [go here](https://msrc.microsoft.com/update-guide).


### If you need any assistance with cybersecurity, want training for your employees or have any questions regarding cybersecurity within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).