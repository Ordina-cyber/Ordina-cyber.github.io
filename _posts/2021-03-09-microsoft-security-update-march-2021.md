---
layout: post
title:  "Microsoft Security Update March 2021"
author: maximilian_leire
categories: [ Microsoft-security-update, Microsoft ]
image: assets/images/Microsoft-Patch-Tuesday.png
description: "Microsoft Security Update March 2021"
featured: false
hidden: false
---

The third Patch Tuesday of the week brings more exploited vulnerabilities than usual so this is definitely one to pay attention to. A few of the CVEs were actually released last week in an emergency patch by Microsoft because of the severity of the vulnerabilities and the fact that they were being exploited in the wild. In total 89 CVEs were patched this month including the seven CVEs released for Exchange servers last week. Of these 89, 14 are rated as critical and 5 have been reported as being actively exploited.

## Emergency patch: Active attacks on Exchange servers
Microsoft released [a detailed and informative blogpost](https://www.microsoft.com/security/blog/2021/03/02/hafnium-targeting-exchange-servers/) on this matter so if you want to learn about this further or want to know if your company was impacted I recommend you to follow their recommendations. You can of course [ask for our help as well](https://www.ordina.be/diensten/security-and-privacy/)!

The first time we heard about this was on the second of March. Microsoft detected multiple 0-day exploits being used to attack on-premises versions of Microsoft Exchange Server in limited and targeted attacks. These security flaws allowed to attackers to access email accounts and gave them the ability to install malware which makes it possible for the attackers to have long-term access to the victim environments.

If you have an on-premise Exchange server it’s crucial to update this as soon as possible to avoid falling victim to these attacks but you also have to check your server for the IOCs (Indicators of Compromise) that Microsoft shared to ensure you have not been a victim already. In this case, simply applying the update will probably not be sufficient and we advise you to take further precautions and investigate your environment. 

Exchange Online was not affected.

## The 'usual' Patch Tuesday patches
### [CVE-2021-26411](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-26411) | Internet Explorer Memory Corruption Vulnerability
This patch fixes a security flaw in Internet Explorer and Microsoft Edge (The older EdgeHTML version). The vulnerability allows an attacker to run (malicious) code on a victim's computer by having them open a specially crafted HTML file. If your company still relies on these browsers it is definitely time to search for alternate options as the legacy Edge version reached it's end of life date today (9 march 2021) and Internet Explorer will have it's official support end on August 17th 2021.

This vulnerability has been reported by Microsoft to be publicly known and exploited so have a look at this quickly! If an attacker manages to run the malicious code on a victim's pc the code will be ran with the privileges of the user that is currently logged in so let this be a reminder to only use administrator accounts when necessary!


### [CVE-2021-26897](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-26897) | Windows DNS Server Remote Code Execution Vulnerability
This is the second month of DNS RCE vulnerabilities as we covered [CVE-2021-24078](https://portal.msrc.microsoft.com/en-US/security-guidance/advisory/CVE-2021-24078) in [last month's article](https://ordina-cyber.github.io/microsoft-security-update-february-2021/) as well.

As the name suggests this vulnerability allows an attacker to execute potentially malicious code on Microsoft Servers being used as DNS Servers. With a CVSS score of 9.8 this is one to look out for and with all these DNS server vulnerabilities popping up it can't hurt to pay some extra attention to your DNS server monitoring in the upcoming weeks.





For a list of all vulnerabilities that were disclosed this month [go here](https://msrc.microsoft.com/update-guide).


### If you need any assistance or have any questions regarding cybersecurity within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).
