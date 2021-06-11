---
layout: post
title:  "Microsoft Security Update June 2021"
author: maximilian_leire
categories: [ Microsoft-security-update, Microsoft ]
image: assets/images/Microsoft-Patch-Tuesday.png
description: "Microsoft Security Update June 2021"
featured: true
hidden: false
---

Microsoft released patches for 50 CVEs this month, 5 are rated as critical and the others as important. An unusually high amount of bugs are reported to be publicly exploited at this moment, 6 to be exact of which 3 are publicly known. 

The six currently exploited vulnerabilities are:
* [CVE-2021-33742](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-33742) | Windows MSHTML Platform Remote Code Execution Vulnerability
* [CVE-2021-33739](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-33739) | Microsoft DWM Core Library Elevation of Privilege Vulnerability
* [CVE-2021-31199](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-31199) | Microsoft Enhanced Cryptographic Provider Elevation of Privilege Vulnerability
* [CVE-2021-31201](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-31201) | Microsoft Enhanced Cryptographic Provider Elevation of Privilege Vulnerability
* [CVE-2021-31955](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-31955) | Windows Kernel Information Disclosure Vulnerability
* [CVE-2021-31956](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-31956) | Windows NTFS Elevation of Privilege Vulnerability


### [CVE-2021-33742](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-33742) | Windows MSHTML Platform Remote Code Execution Vulnerability
This first vulnerability is the only CVE rated as critical this patch. As this is also reported being actively exploited in the wild make sure to put this one at the top of your priority list.

This bug could allow an attacker to execute malicious code if a user views a specially crafted webpage. Since the vulnerability is in the Trident engine (the software used to render webpages in Internet Explorer) all versions of internet explorer are impacted but older software making use of this engine are impacted as well. This impacts all Windows versions.


### [CVE-2021-31199](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-31199) & [CVE-2021-31201](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-31201) | Microsoft Enhanced Cryptographic Provider Elevation of Privilege Vulnerability
These two vulnerabilities are linked to an Adobe Reader remote code execution bug which was [fixed by Adobe last month](https://helpx.adobe.com/security/products/acrobat/apsb21-29.html). Remote Code execution attacks are a lot more dangerous when used in combination with Elevation of Privilege attacks which is probably what happened here. When combining these vulnerabilities an attacker could use phishing to have a user open a malicious pdf and then run code which exploits the Elevation Of Privilege vulnerability so the malicious software would be ran with higher privileges than normal.

As Adobe Reader is used in almost every company make sure to apply these patches for your Windows systems and make sure your Adobe software is up to date as well.

### [CVE-2021-31962](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-31962) | Kerberos AppContainer Security Feature Bypass Vulnerability
Last but not least we have the vulnerability with a CVSS score of 9.4, this is the highest this month. This bug could allow an attacker to bypass authentication in services that use Kerberos authentication accessed via an SPN. As Kerberos is widely used and is not secure without proper SPN authentication make sure you put this CVE high on your list as well.



For a list of all vulnerabilities that were disclosed this month [go here](https://msrc.microsoft.com/update-guide).


### If you need any assistance or have any questions regarding cybersecurity within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).
