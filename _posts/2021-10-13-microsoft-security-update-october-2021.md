---
layout: post
title:  "Microsoft Security Update October 2021"
author: maximilian_leire
categories: [ Microsoft-security-update, Microsoft ]
image: assets/images/Microsoft-Patch-Tuesday.png
description: "Microsoft Security Update October 2021"
featured: false
hidden: false
---

71 CVEs have been fixed this patch Tuesday, on top of this 8 Microsoft Edge and 3 OpenSSL patches were released earlier this month. This is also the first patch Tuesday to include Windows 11 fixes.

Two of these 71 CVEs are rated as critical.

## [CVE-2021-40449](https://msrc.microsoft.com/update-guide/en-US/vulnerability/CVE-2021-40449) | Win32k Elevation of Privilege Vulnerability
This is the only CVE this month that has been detected being exploited in the wild. Exploiting this vulnerability could give an attacker higher privilege on a system. Using this in malware or in combination with a remote code execution vulnerability could have disastrous consequences so don't fall victim and protect yourself by staying up to date!

## [CVE-2021-40486](https://msrc.microsoft.com/update-guide/en-US/vulnerability/CVE-2021-40486) | Microsoft Word Remote Code Execution Vulnerability
This vulnerability allows an attacker to execute malicious code on a target machine when a user opens a specially crafted Word document. In case this vulnerability is combined with an escalation of privilege vulnerability like [CVE-2021-40449](https://msrc.microsoft.com/update-guide/en-US/vulnerability/CVE-2021-40449) this could be used to gain total control over a device.


## [CVE-2021-40454](https://msrc.microsoft.com/update-guide/en-US/vulnerability/CVE-2021-40454) | Rich Text Edit Control Information Disclosure Vulnerability
Rich Text Edit Control is a component in [Microsoft power apps](https://powerapps.microsoft.com/en-us/). When abused this bug allows an attacker to read passwords from memory in cleartext. Make sure to deploy this patch quickly if you use powerapps in your company.


For a list of all vulnerabilities that were disclosed this month [go here](https://msrc.microsoft.com/update-guide).


### If you need any assistance with cybersecurity, want training for your employees or have any questions regarding cybersecurity within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).