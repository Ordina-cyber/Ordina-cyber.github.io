---
layout: post
title:  "Microsoft Security Update November 2020"
author: maximilian_leire
categories: [ Microsoft-security-update, Microsoft ]
image: assets/images/Microsoft-Patch-Tuesday.png
description: "Microsoft Security Update November 2020"
featured: false
hidden: false
---


The second Tuesday of the month is upon us again which means Microsoft has released its patch for this month, it provides fixes for 112 vulnerabilities. 17 patches have been rated critical and 93 are rated as important. There's one particularly interesting CVE that involves a non-microsoft product (Google Chrome) that is reported to be exploited and publicly known.

An important side note is the fact that Microsoft has changed the way it releases info about the vulnerabilities found. They are now using a revised security portal which you can find [here](https://msrc.microsoft.com/update-guide/) but they no longer release a write up for each CVE. This means that we may have less details to provide you with unfortunately but we will of course keep providing you the necessary info about the patches released each month. On a positive note, the new portal has a clear overview of some key aspects of each CVE such as: attack vector, attack complexity, scope, remediation level, etc. So it is worth having a look if you want some more info about a certain vulnerability.

That being said, let's have a look at the most prominent patches this month.


### [CVE-2020-17087](https://msrc.microsoft.com/update-guide/en-US/vulnerability/CVE-2020-17087) | **Windows Kernel Local Elevation of Privilege Vulnerability**
As stated before this vulnerability works in combination with Google Chrome, the flaw [was found by the team at Google](https://bugs.chromium.org/p/project-zero/issues/detail?id=2104) and is now being remediated in Windows as well. Using a bug in Chrome attackers could execute code with higher privilege than they should have on a vulnerable Windows machine, this bug is reported as being publicly known and exploited but it doesn't seem to be widespread. It is interesting to note that in the report from te team at Google they state the bug has been around since Windows 7.

This issue can NOT be fixed with only a Google Chrome update so make sure to install this Windows update to remediate this problem and protect yourself from becoming a target.



### [CVE-2020-17084](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2020-17084) | **Microsoft Exchange Server Remote Code Execution Vulnerability**
This is an interesting one as well as we have talked about this vulnerability before in our [September security update (CVE-2020-16875)](https://ordina-cyber.github.io/microsoft-security-update-september-2020/). The person that found this vulnerability back then has managed to bypass the patch Microsoft provided which means the flaw was exploitable once again. This is why Microsoft provided a second update to now hopefully fix this issue once and for all.

It was very important to apply the fix for this vulnerability as soon as possible the first time around so we recommend you to do the same now as well.


### (Example) [CVE-2020-17106](https://msrc.microsoft.com/update-guide/en-US/vulnerability/CVE-2020-17106) | **Microsoft Image and Video extensions Remote Code Execution Vulnerability**
Multiple RCE vulnerabilities have been reported in extensions from the Microsoft app store. Luckily if you don't have these installed your Windows system is not vulnerable to this but if your company uses a lot of video or images chances are you might have these installed so make sure your users have these updated as soon as possible.


### [CVE-2020-17051](https://msrc.microsoft.com/update-guide/en-US/vulnerability/CVE-2020-17051) | **Windows Network File System Remote Code Execution Vulnerability**
We unfortunately do not yet have any clear info regarding how this vulnerability can be exploited but with the info we have we can state this is definitely one to look out for as NFS is a widely used network service and the CVSS score for this CVE is 9.8 which is almost as high as it can get. The flaw is listed to have a low attack complexity on the Microsoft portal and can be exploited without user interaction (which means there is no need for any kind of phishing for example) so it’s definitely very dangerous.

## Azure Sphere
New this month are around 15 vulnerabilities listed for the Azure IoT platform Sphere. Luckily if you have any of these devices in your company they should have already been updated automatically at the time you are reading this but it can't hurt to double check of course.


For a list of all vulnerabilities that were disclosed this month [go here](https://msrc.microsoft.com/update-guide).

### If you need any assistance or have any questions regarding cybersecurity within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).
