---
layout: post
title:  "Microsoft Security Update December 2020"
author: maximilian_leire
categories: [ Microsoft-security-update, Microsoft ]
image: assets/images/Microsoft-Patch-Tuesday.png
description: "Microsoft Security Update December 2020"
featured: true
hidden: false
---

We end 2020 with a slower month, as per usual for December patches. 58 vulnerabilities have been addressed this final month of the year, of which 9 are rated critical and 46 as important. Fortunately, none of them are reported to be publicly known or exploited. This brings the total number of disclosed Microsoft vulnerabilities to 1250 for this year. Let’s have a look at the most notable flaws found and consequently where your priorities for patching should lie. We will be focussing on the CVE’s with the highest CVSS scores which consist of many remote code execution vulnerabilities.

## Microsoft Exchange Remote Code Execution Vulnerabilities
* [CVE-2020-17132](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17132)
* [CVE-2020-17142](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17142)
* [CVE-2020-17141](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17143)
* [CVE-2020-17144](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17144)
* [CVE-2020-17117](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17117)

All vulnerabilities listed above are remote code execution vulnerabilities found on MS Exchange server.[CVE-2020-17132](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17132) and [CVE-2020-17142](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17142) score the highest of all the vulnerabilities announced this month with a CVSS score of 9.1. Luckily, to exploit these flaws, attackers need high privilege access (e.g. administrator access).

[CVE-2020-17144](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17144) is also notable since it targets Microsoft Exchange Server 2010 which became end-of-life this past October. Good to see Microsoft is still willing to provide a patch for this either way but if you are still running this old version, it’s a good reminder to upgrade as soon as possible. Luckily high privileges are also required here to be able to exploit this vulnerability. 

## Microsoft Excel, Powerpoint & Sharepoint Remote Code Execution Vulnerabilities
* [CVE-2020-17121](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17121)
* [CVE-2020-17118](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17118)
* [CVE-2020-17122](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17122)
* [CVE-2020-17123](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17123)
* [CVE-2020-17124](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17124)
* [CVE-2020-17125](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17125)
* [CVE-2020-17127](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17127)
* [CVE-2020-17128](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17128)
* [CVE-2020-17129](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17129)

This month, 2 Sharepoint, 1 Powerpoint and 6 Excel remote code execution vulnerabilities have been addressed. 

The 2 Sharepoint vulnerabilites ([CVE-2020-17121](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17121) and [CVE-2020-17118](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17118)) score a very high 8.8 and 8.1 respectively. These should be one of your priorities to patch. 

[CVE-2020-17121](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17121)  has a low attack complexity and no user interaction is needed to exploit this flaw. Luckily privileges are still required but as these only have to be for a standard user, you should put this high on your watchlist. [CVE-2020-17118](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17118) doesn’t require any privileges but does require user interaction, another vulnerability which stresses user awareness within a company. 

All Excel vulnerabilities state the preview pane in Windows Explorer is not an attack vector. That means attackers need a user to open the file. Make sure all users in your organization are extra careful when clicking links and opening files until you apply the necessary patch (but of course it doesn’t hurt to be extra careful all the time). Notably Excel for Mac has not yet received an update but there should be one available soon. 


For a list of all vulnerabilities that were disclosed this month [go here](https://msrc.microsoft.com/update-guide).

### If you need any assistance or have any questions regarding cybersecurity within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).