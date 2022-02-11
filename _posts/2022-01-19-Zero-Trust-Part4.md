---
layout: post
title:  "What is Zero Trust Architecture and why is it so important to understand? Part 4"
author: jordy_bekaert
categories: [ ]
image: assets/images/ZeroTrust.jpg
description: "What is Zero Trust Architecture and why is it so important to understand? Part 4"
featured: false
hidden: false
---

## The trust algorithm
Within a Zero Trust Architecture, the Policy Engine (PE) is the master brain and the trust algorithm is the primary thought process allowing or denying access.

![Trust_Algorithm](..\assets\images\Posts\ZeroTrust\P4.png)

The Policy engine’s Trust Algorithm makes a decision based on several input sources: 

- Access Request: information about the access requester is to be trusted or not (based on  OS/patch version, software patches, ….)
- Subject Database and History: who is / has been requesting access
  - Set of subjects (humans and processes) and assigned attributes/privileges
  - User identity can be a mix of local identity (user account) and the results of authentication checks by PEPs
  - Attributes of identity then get factored in the given trust/confidence level, together with time and geographical location
  - Privileges are being assigned individually, on a per request basis
- Asset database: contains the known status of each company owned and non-enterprise/BYOD(Bring Your Own Device) asset and is compared to the observable status (like OS version, software present, integrity, network location and geo location)
- Resource requirements: in addition to the user ID and the attributes database, this set of policies may include MFA network location (for example deny access from US IP’s), data sensitivity
- Threat intel

The weight of importance of each data source may be built-in to the used algorithm or may be tweaked manually. The final determination is then passed to the PA (Policy Administrator) for execution, which configures the Policy Enforcement Points (PEPs) to enable authorized communication and block unauthorized access.

Looking back to the analogy made during the intro in the first article of this series, now every person who’d be responsible to catch you is monitored and his/her behavior is analyzed. If someone turns out to be untrustworthy, the person will be removed before you will take the jump, and the situation will be reviewed again to confirm if it is still safe to jump.
If this is not the case, you won’t be able to jump because your bodyguard doesn’t allow you to, and saves you from breaking your neck or worse.

## Conclusion

Instead of just allowing users and system to access company data purely based on a username and password (with the result of breaches we still see every day), Zero Trust Architecture principles verify the identity of users and devices based on several attributes and context (such as time, date, location) and aspects that reflect the security posture of a device. After the device and user are granted access, only the right specific privileges will be provided. Access means only access to a specific source and not to the whole network. A key element of the Zero Trust model is the continuous evaluation and adjustment of trust ; if important properties of a device or user change, the verification process restarts.

With Zero Trust integrated into your IT infrastructure, you are in a much better shape to make it harder for adversaries to reach their goals.   
This shift from the historical (‘trust but verify’) security governance concepts to Zero Trust does not only take and trigger a drastic mindset change (which some people and organizations still need to make), but also a phased approach for implementation; this does not happen overnight.

#### Ordina is your partner in this journey and enables you to go ahead of change against the security challenges of the digital age. If you need any assistance with cybersecurity, want training for your employees or have any questions regarding cybersecurity within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).