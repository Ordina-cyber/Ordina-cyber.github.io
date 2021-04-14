---
layout: post
title:  "Microsoft Security Update April 2021"
author: maximilian_leire
categories: [ Microsoft-security-update, Microsoft ]
image: assets/images/Microsoft-Patch-Tuesday.png
description: "Microsoft Security Update April 2021"
featured: true
hidden: false
---

Patches for 114 CVEs were released this month which makes this the busiest month of 2021 so far. Of these bugs, 19 are rated as critical. 1 bug is currently being actively exploited and 4 others are publicly known, none of these are rated critical.

## [CVE-2021-28310](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-28310) | Win32k Elevation of Privilege Vulnerability

This is the CVE that is being actively exploited at the moment. This bug allows an attacker to gain more privileges on a system by running specially crafted software on a target system. Of course before an attacker could do this they would need access to that system or trick a user into running the software themselves.

A vulnerability like this can be disastrous when combined with malware. Malicious software ran with administrative privileges can potentially do far more damage than a normal user account could. Using this exploit an attacker could elevate the rights with which the malware is ran even if the compromised user only has restricted privileges.

Be sure to apply this fix as soon as you can.


## [CVE-2021-28480](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-28480) - [CVE-2021-28483](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-28483) | Win32k Elevation of Privilege Vulnerability

* [CVE-2021-28480](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-28480)
* [CVE-2021-28481](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-28481)
* [CVE-2021-28482](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-28482)
* [CVE-2021-28483](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-28483)

Once again vulnerabilities were found in Microsoft Exchange server, all of these are Remote Code Execution Vulnerabilities which could allow an attacker to execute malicious code on your server over the internet. Last month an emergency patch was carried out by Microsoft for a critical Exchange vulnerability and now 4 new RCE vulnerabilities were discovered again. It has probably been a busy few months for the Microsoft Exchange team and for administrators maintaining Exchange servers.

CVE-2021-28480 & CVE-2021-28481 received a CVSS score of 9.8 which is remarkably high. Both of these have 'Network' as attack vector, which means the attack can be executed remotely and the exploit might potentially be [wormable](https://www.cisco.com/c/en/us/products/security/what-is-a-worm.html#~response-methodologies). Furthermore the attack complexity is low and no privileges or user interaction are required. You definitely want to apply this patch as soon as possible.



For a list of all vulnerabilities that were disclosed this month [go here](https://msrc.microsoft.com/update-guide).


### If you need any assistance or have any questions regarding cybersecurity within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).