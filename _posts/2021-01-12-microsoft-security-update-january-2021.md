---
layout: post
title:  "Microsoft Security Update January 2021"
author: maximilian_leire
categories: [ Microsoft-security-update, Microsoft ]
image: assets/images/Microsoft-Patch-Tuesday.png
description: "Microsoft Security Update January 2021"
featured: true
hidden: false
---

The first patch Tuesday of 2021! The blog team wishes you all the best for this new year. We kick the year off with 83 bugfixes this patch including one zero day vulnerability that Microsoft has reported is being currently exploited. Of these 83 vulnerabilities, 10 are rated as critical and 73 as important. Let’s take a look at the most important ones.

## [CVE-2021-1647](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-1647) | Microsoft Defender Remote Code Execution Vulnerability
This is the bug that has been reported to be exploited by Microsoft. The good news is that as long as your system is connected to the internet and the security patching isn’t explicitly blocked by a system administrator this bug should already have been patched on your device. Unfortunately Microsoft does not state how the attack exactly works or how widespread the attacks actually are. If you have anything blocking the security patching or if your system is not connected to the internet make sure to fix this one as soon as possible!


## [CVE-2021-1648](https://msrc.microsoft.com/update-guide/en-US/vulnerability/CVE-2021-1648) | Microsoft splwow64 Elevation of Privilege Vulnerability
This vulnerability is rated as important and is currently publicly known. Luckily despite being publicly known, Microsoft has reported that no attacks using this vulnerability have been detected. If this bug were to be exploited by an attacker it could allow malicious code to run with higher privileges than normal (elevation of privileges).

Even though Microsoft reports this bug hasn’t been publicly exploited (yet!), as the vulnerability is publicly known it could be weaponized quickly, so make sure you put this one on your priority list before you become a target.



## The other critical vulnerabilities
As for the rest of the critical vulnerabilities besides [CVE-2021-1647](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-1647), all but one are bugs that could allow for remote code execution.

5 of these are in the "[Remote Procedure Call Runtime](https://docs.microsoft.com/en-us/windows/win32/api/_rpc/)", for example [CVE-2021-1658](https://msrc.microsoft.com/update-guide/en-US/vulnerability/CVE-2021-1658). As all five of these vulnerabilities have a low attack complexity, low privileges required and do not require any user interaction, these are ones to definitely look out for.

A bug has been discovered in the HEVC video extension but this should be automatically patched by your organisation or Windows Store on your device. Similarly the remote code execution flaw found in Microsoft Edge should be automatically fixed in your next browser update as well.

For a list of all vulnerabilities that were disclosed this month [go here](https://msrc.microsoft.com/update-guide).

### If you need any assistance or have any questions regarding cybersecurity within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).