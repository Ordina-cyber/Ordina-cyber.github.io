---
layout: post
title:  "Microsoft Security Update August 2021"
author: maximilian_leire
categories: [ Microsoft-security-update, Microsoft ]
image: assets/images/Microsoft-Patch-Tuesday.png
description: "Microsoft Security Update August 2021"
featured: true
hidden: false
---

A smaller patch this month, with fixes for 44 CVEs. But don't let your guard down as Microsoft reported 2 publicly known vulnerabilities and even 1 that is currently being exploited. 

## [CVE-2021-36948](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-36948) | Windows Update Medic Service Elevation of Privilege Vulnerability
We start by having a closer look at the vulnerability that is currently being exploited. The Windows Update Medic Service is a Windows 10 feature that automatically repairs Windows Update components in case they stop working correctly. By using specially crafted software an attacker could gain higher privileges than the current user should have. Luckily the attacker would need full access to a device to execute this exploit but it can be potentially very damaging when used in combination with other vulnerabilities.


## [CVE-2021-36942](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-36942) | Windows LSA Spoofing Vulnerability
Luckily the only flaw currently being exploited is the one we discussed first but these next two are publicly know so they could become exploited very soon. Make sure you are ahead of the attackers by keeping your systems up to date!

This fix is futher mitigation of vulnerabilities for *PetitPotam* which you can read Microsoft's official info about [here](https://support.microsoft.com/en-us/topic/kb5005413-mitigating-ntlm-relay-attacks-on-active-directory-certificate-services-ad-cs-3612b773-4043-4aa9-b23d-b87910cd3429). This update could have usability impact on some systems so make sure you are fully informed before rolling these out.


## [CVE-2021-36936](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-CVE-2021-36936) | Windows Print Spooler Remote Code Execution Vulnerability
Finally, just like last month, we have another fix for more Windows Print Spooler RCE vulnerabilities. After the infamous *PrintNightmare* vulnerabilities which dominated the security news last month and made Microsoft release an emergency patch, more of the same kind of vulnerabilities still pop up.

Make sure to apply this patch and read up on all official Microsoft documentation so you have all the necessary security measures in place to keep you and your company safe from potential attacks.

Microsoft has released further info for all print spooler vulnerabilities [here](https://support.microsoft.com/en-us/topic/kb5005652-manage-new-point-and-print-default-driver-installation-behavior-cve-2021-34481-873642bf-2634-49c5-a23b-6d8e9a302872).



For a list of all vulnerabilities that were disclosed this month [go here](https://msrc.microsoft.com/update-guide).


### If you need any assistance with cybersecurity, want training for your employees or have any questions regarding cybersecurity within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).