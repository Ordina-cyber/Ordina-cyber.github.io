---
layout: post
title:  "Microsoft Security Update February 2021"
author: maximilian_leire
categories: [ Microsoft-security-update, Microsoft ]
image: assets/images/Microsoft-Patch-Tuesday.png
description: "Microsoft Security Update February 2021"
featured: false
hidden: false
---

For the second patch of 2021 we have 56 CVEs to look at. 11 of these vulnerabilities have been rated as critical and 43 as important. While the number of CVEs is significantly lower than the past few months the amount of publicly known issues is higher. 1 security flaw is stated to be actively exploited and 6 were already publicly known at the time of this patch's release. Luckily the 6 publicly known bugs have not yet been detected being actively exploited.


## [CVE-2021-1732](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-1732) | Windows Win32k Elevation of Privilege Vulnerability
Let's start with arguably the most urgent of all issues since this one has been reported to be exploited in the wild. This local privilege escalation vulnerability could allow an attacker who has access at the user level to execute code with higher privileges. If a user's pc would be compromised or infected with malware this could have far graver consequences than if an attacker would only have 'user' access rights. This means this patch should definitely be one at the top of your priority list.


## [CVE-2021-24078](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-24078) | Windows DNS Server Remote Code Execution Vulnerability
This bug allows remote code execution in a privileged service without the need for authentication. The fact that no credentials are needed, and this can be executed remotely as well as the malicious code would be run in a privileged environment makes this CVE very dangerous. Luckily only Windows Servers set up as DNS servers are vulnerable to this. But if you rely on a Windows DNS Server make sure to implement this fix as soon as possible.


## Multiple Security Updates Affecting TCP/IP
* [CVE-2021-24074](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2021-24074) | Windows TCP/IP Remote Code Execution Vulnerability
* [CVE-2021-24086](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2021-24086) | Windows TCP/IP Denial of Service Vulnerability
* [CVE-2021-24094](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2021-24094) | Windows TCP/IP Remote Code Execution Vulnerability

Microsoft released [a blog post](https://msrc-blog.microsoft.com/2021/02/09/multiple-security-updates-affecting-tcp-ip/) about these vulnerabilities so we have a lot more info about these than usual.

Microsoft states the Denial of Service vulnerability could allow an attacker to cause a *stop error* on a remote machine which may cause users to receive a blue screen and hinder their ability to use their Windows computer.

The Remote Code Execution vulnerabilities could allow an attacker to execute malicious code remotely and without authentication.

[CVE-2021-24074](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2021-24074) can be exploited using IPv4 source routing requests. Luckily this is disallowed by default in Windows installations. You should definitely still implement the patch to be secure, if the patch can't immediately be implemented Microsoft also provided a workaround which is documented in the [CVE](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2021-24074).

[CVE-2021-24094](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2021-24094) could allow an attacker to send a large amount of packet fragments which could lead to the remote code execution. This vulnerability affects IPv6, fortunately for this bug Microsoft also provides a patch and a workaround in the CVE ([CVE-2021-24094](https://msrc.microsoft.com/update-guide/vulnerability/CVE-2021-24094)).

Furthermore while preparing to install the patches these three security issues, be aware that they can be remediated virtually on edge devices such as load balancers or firewalls, by blocking IPv4 Source Routing requests and IPv6 fragments.



For a list of all vulnerabilities that were disclosed this month [go here](https://msrc.microsoft.com/update-guide).
For Microsoft's blogpost about the TCP/IP vulnerabilities [go here](https://msrc-blog.microsoft.com/2021/02/09/multiple-security-updates-affecting-tcp-ip/).


### If you need any assistance or have any questions regarding cybersecurity within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).
