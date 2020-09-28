---
layout: post
title:  "Microsoft Security Update September 2020"
author: maximilian_leire
categories: [ Microsoft-security-update, Microsoft ]
image: assets/images/Microsoft-Patch-Tuesday.png
description: "Microsoft Security Update September 2020"
featured: true
hidden: true

---

This *Patch Tuesday* fixes 129 known vulnerabilities of which 23 are rated as critical. <br>

Software affected by this patch is: 
* Microsoft Windows 
* Edge (EdgeHTML-based and Chromium-based 
* ChakraCore 
* Internet Explorer (IE) 
* SQL Server 
* Office and Office Services and Web Apps 
* Microsoft Dynamics 
* Visual Studio 
* Exchange Server 
* ASP.&#8203;NET 
* OneDrive 
* Azure DevOps 
<br>

If you are using any product of the software above (which you probably are) then make sure you are up to date on the latest vulnerabilities you might be vulnerable to. None of the security issues have been reported to be publicly known or exploited, but since they are public knowledge now you should implement this patch as soon as possible as to not fall victim to these known issues. <br>

## [CVE-2020-16875](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-16875) | Microsoft Exchange Memory Corruption 

The most notable fix this patch is for this remote code execution vulnerability that impacts Microsoft Exchange servers. It has a CVSS score of 9.1 out of 10 and allows attackers to run arbitrary ( and in case of an attack, most likely malicious) code as the "system" user on the server using a specially crafted mail. As the system user has even more privileges than a local administrator account this is a serious issue. Microsoft has noted that this can only be done by a user who is authenticated on the server which would make an attack far less likely but this is not confirmed by the researcher that found this bug. We recommend all exchange users to check if their version is impacted [here](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-16875) and patch as soon as possible if you are running a vulnerable server. <br>

## Other Remote Code Execution vulnerabilities <br>

More critical Remote code Execution vulnerabilities have been found in other software as well. One was reported for Microsoft Windows and seven CVE's where made public for similar issues in Sharepoint. An attacker can execute malicious code using a specifically crafted file in both so this is definitely a case where having well trained employees wary of suspicious files is really important. Obviously this shouldn't be your only defense so make sure to apply the necessary patches as soon as possible here too. <br> 

More info can be found using the links below. <br>

If you need any assistance or have any questions regarding digital security within your company, don’t hesitate to [contact us](hhttps://www.ordina.be/en/services/security-and-privacy/). 

 

**Sources:** 

* [Microsoft - September 2020 Security Updates](https://portal.msrc.microsoft.com/en-us/security-guidance/releasenotedetail/2020-Sep) 
* [CVE-2020-16875 - Microsoft Exchange Memory Corruption](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-16875) 
* [CVE-2020-1129 - Microsoft Windows Codecs Library Remote Code Execution Vulnerability](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-1129) 
* [CVE-2020-1210 - Microsoft SharePoint Remote Code Execution Vulnerability](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-1210) 
* [CVE-2020-1595 - Microsoft SharePoint Remote Code Execution Vulnerability](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-1595) 