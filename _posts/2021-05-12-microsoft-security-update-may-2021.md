---
layout: post
title:  "Microsoft Security Update May 2021"
author: maximilian_leire
categories: [ Microsoft-security-update, Microsoft ]
image: assets/images/Microsoft-Patch-Tuesday.png
description: "Microsoft Security Update May 2021"
featured: true
hidden: false
---

Microsoft released patches for 55 CVEs this month of which 26 are rated as critical. This makes it a slower month than usual but there are still some very important vulnerabilities you should definitely be paying attention to. One bug we will be discussing in this article particularly grabbed our attention in this month's release. 

## [CVE-2021-28476](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-28476) | Hyper-V Remote Code Execution Vulnerability
This patch has a very high CVSS score of 9.9. The bug could allow for a Denial Of Service attack on systems running on Hyper-V, this would be done in the form of a *[bugcheck](https://docs.microsoft.com/en-us/windows-hardware/drivers/devtest/interpreting-a-bug-check-code#:~:text=When%20Microsoft%20Windows%20encounters%20a,might%20have%20caused%20this%20error.)*. A bug check occurs when Microsoft Windows encounters a condition that compromises safe system operation, the system wilt halt so you can take the necessary actions and since the system isn't usable in that state, a Denial Of Service attack would have been successfully executed. If you have critical systems running on Hyper-V make sure to have a look at this fix as soon as possible.


## [CVE-2021-31181](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-31181) | SharePoint Remote Code Execution Vulnerability
Quite a few Sharepoint bugs were fixed this patch with the most notable being this remote code execution vulnerability. Microsoft unfortunately didn't release a lot of info about these but if you have servers running Sharepoint we recommend to apply these patches as soon as possible. 


## [CVE-2021-31166](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-31166) | HTTP Protocol Stack Remote Code Execution Vulnerability
We kept the most notable of all vulnerabilities for last this time. A critical vulnerability was found in the HTTP Protocol Stack. This affects Windows 10 as well as multiple versions of Windows Server. An attacker could potentially execute malicious code by sending specially crafted HTTP packets to a vulnerable machine. This code will be ran as *kernel* which means it has virtually all rights on the machine, even more so than administrators. To make matters even worse Microsoft has reported that the vulnerability is wormable which means an attacker could make it so the targeted machine spreads the malicious software over the network to other vulnerable machines.

One thing to note is that the security flaw only applies to machines running a web server so luckily not all Windows 10 & Windows Server machines are vulnerable.

Make sure to put this on the top of your priority list and patch this issue as soon as possible!


For a list of all vulnerabilities that were disclosed this month [go here](https://msrc.microsoft.com/update-guide).


### If you need any assistance or have any questions regarding cybersecurity within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).
