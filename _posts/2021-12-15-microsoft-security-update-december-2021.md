---
layout: post
title:  "Microsoft Security Update December 2021"
author: maximilian_leire
categories: [ Microsoft-security-update, Microsoft ]
image: assets/images/Microsoft-Patch-Tuesday.png
description: "Microsoft Security Update December 2021"
featured: true
hidden: false
---

The last patch Tuesday of the year. This month 67 patches for new CVEs were released by Microsoft. That brings the yearly total up to 887 patches.

One of the 67 CVEs has been reported by Microsoft to currently being exploited in the wild.

## [CVE-2021-43890](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2021-43890) | Windows AppX Installer Spoofing Vulnerability
This vulnerability has been detected being exploited so make sure to act quickly if this bug affects you!

Microsoft released info that this vulnerability has been used in malware such as the infamous [Emotet](https://www.hornetsecurity.com/us/knowledge-base/emotet/). This patch fixes a bug in the AppX installer for Windows.

For this vulnerability to be exploited an attacker would have to send a specially crafted attachment to a user and convince them to open it. The malicious software will then be run as the currently logged on user, if this user has administrator rights or this bug can be paired with an escalation of privilege vulnerability, it could have disastrous consequences.

Always stay alert for suspicious emails and make sure your coworkers are informed as well.

## [CVE-2021-43907](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2021-42907) | Visual Studio Code WSL Extension Remote Code Execution Vulnerability
Visual Studio Code is a widely used free code editor created by Microsoft. The WSL extension can be utilised by developers to develop Linux software on a Windows machine which makes it very popular with DevOps teams.

This extension currently has a security vulnerability that makes Remote Code Execution possible without any authentication or user interaction.

If teams in your company use this extension make sure to apply this patch as soon as possible.


## [CVE-2021-43905](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2021-43905) | Microsoft Office app Remote Code Execution Vulnerability
Due to improper input validation in the Microsoft Office App, an attacker could send a specially crafted request which would allow potentially malicious code to be executed on the target system.

Since almost every employee in every company has the Microsoft Office App installed make sure to patch this quickly.


For a list of all vulnerabilities that were disclosed this month [go here](https://msrc.microsoft.com/update-guide).


### If you need any assistance with cybersecurity, want training for your employees or have any questions regarding cybersecurity within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).