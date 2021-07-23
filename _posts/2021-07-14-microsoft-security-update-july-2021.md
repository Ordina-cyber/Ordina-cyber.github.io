---
layout: post
title:  "Microsoft Security Update July 2021"
author: maximilian_leire
categories: [ Microsoft-security-update, Microsoft ]
image: assets/images/Microsoft-Patch-Tuesday.png
description: "Microsoft Security Update July 2021"
featured: true
hidden: false
---

Patches for 117 CVEs were released this month by Microsoft. 13 of these are rated as critical also 6 of these exploits are publicly known and 4 are reported being currently exploited. The most notable bug this month was named *Printnightmare* which was patched before the usual monthly security updates. We will have a look at this bug first.

## [CVE-2021-34527](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-34527) | Windows Print Spooler Remote Code Execution Vulnerability
This issue exists in the Windows Print Spooler Service which is why it was given the name *Printnightmare*. When successfully exploited this vulnerability could allow an attacker to run (malicious) code with SYSTEM privileges. SYSTEM privileges are normally only granted to the Windows OS and have even more permissions than an admin account.

Malicious code ran with this kind of privileges can do a lot of damage so make sure you update your systems asap if you haven't done so yet.

Check the official Microsoft information [here](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-34527) and make sure you follow their instructions to keep your systems safe.


## [CVE-2021-34494](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-34494) | Windows DNS Server Remote Code Execution Vulnerability
If you have DNS servers running on site make sure to pay close attention to this CVE. This bug could allow an attacker to remotely run malicious code on your DNS server. Some privileges on the server are needed as stated by Microsoft. The vulnerability not being exploited currently according to Microsoft, but as the bug is now publicly known make sure you are one step ahead of cybercriminals by keeping your systems up to date. 


## [CVE-2021-34448](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-34448) | Scripting Engine Memory Corruption Vulnerability
Last but not least we have another bug that could lead to remote code execution. An attacker could execute malicious code on a user's computer by making them browse to a specially crafted webpage. The code would be ran as the user that is currently logged in.

A bug like this is another reminder to only use administrator accounts when necessary since malicious code ran as administrator can do far more damage than when it's ran as a non-privileged user. Besides this, it's also a good reminder to make sure everyone in your company is adequately trained to spot suspicious emails and links.

This bug is currently being exploited so make sure to patch this quickly.



For a list of all vulnerabilities that were disclosed this month [go here](https://msrc.microsoft.com/update-guide).


### If you need any assistance, cybersecurity training for your employees or have any questions regarding cybersecurity within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).