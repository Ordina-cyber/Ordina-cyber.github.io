---
layout: post
title: "Privacy for security professionals 1 : Is a userID considered as personal data?"
author: "jeffrey_van_moortel"
categories: [ Privacy ]
image: assets/images/Posts/GDPR/Classified_document.jpg
description: "Privacy for security professionals 1 : Is a userID considered as personal data?"
featured: true
hidden: false
---

The boundaries between security & privacy are blurring. Today security professionals are expected to have experience in both fields and to be able to advise on cases related to protection of personal data.

Having a good understanding of security basic principles (such as confidentiality, integrity, availability) is a must, but these days a security professional also needs to broaden his horizon and take into account the most general personal data protection principles.

If you are an security expert, it is a good to have some basic knowledge on privacy and privacy legislation (such as GDPR). This blog series can be seen in this light and will answer some questions you might be facing.

## Definition(s) of personal data

Personal data, personal information or personal identifiable information (PII), … ? What term should we use? The general concept behind all these terms is similar: any information that relates to a specific person can be considered "personal."

However, different data privacy regulations use different terms for data that can be used to identify someone. The term "PII" is largely used in the US, while the General Data Protection Regulation (GDPR)refers to "personal data," and the California Consumer Privacy Act (CCPA) refers to "personal information."

Additionally, each piece of privacy legislation has its own definitions for personal information, personal data, or PII; organizations should carefully review the descriptions in the legislation that applies to them.

<table><thead><tr class="header"><th colspan="2">Personal Data (GDPR)</th></tr></thead>
<tbody><tr class="odd"><td>Personally Identifiable Information (PII)</td><td>Not PII but Personal Data under GDPR</td></tr>
<tr class="even"><td><ul><li><p>Name</p></li><li><p>Home address</p></li><li><p>Email address</p></li><li><p>National registry number</p></li><li><p>Telephone number</p></li><li><p>Personal characteristics</p></li><li><p>Biometric data</p></li><li><p>First or last name</p></li><li><p>Place of birth</p></li><li><p>Gender</p></li><li><p>Race</p></li><li><p>Religion</p></li></ul></td><td><ul><li><p>Device ID (e.g. mobile phone device ID)</p></li><li><p>IP address</p></li><li><p>Cookies</p></li><li><p>Browser type</p></li><li><p>Plug-in details</p></li></ul></td></tr></tbody></table>

<br>

## Personal data according to GDPR

Personal data is any information that relates to an **identified or identifiable living individual**. Different pieces of information, which collected together can lead to the identification of a particular person, also constitute personal data.

Personal data that has been de-identified, encrypted or **pseudonymised** but can be used to re-identify a person **remains** personal data and falls within the scope of the GDPR.

Personal data that has been rendered **anonymous** in such a way that the individual is not or no longer identifiable is no longer considered personal data. For data to be truly anonymised, the anonymisation must be irreversible.

## Is a userID considered as personal data?

For example, as you start working at a new customer, you will most probably receive an account (userID – password) to log on to the customer’s network. For some applications/systems you‘ll use that same account to log on (via SSO), for some other applications/systems you might even receive some additional accounts.

A userID is usually linked with a unique ‘user’ (you), so the userID “relates to an identified or identifiable living individual”. A userID can be seen as a form of pseudonymization: your real name (identity) is replaced by some other ‘data’, where that new piece of data is unique and can be linked back to your identity (as, in the case of a userID, your customer will have a mapping table that links userIDs to employees/consultant names).

Remark: if you would render the userID anonymous, then this would no longer concern personal data and GDPR would not be applicable anymore… but what’s the use of a userID when it cannot be linked anymore to a unique person?

Often it is possible to link individual actions performed in a system to an individual employee, by means of the userID. The userID is often present in audit or logfiles and makes it possible to link logfile information to individual users. Examples where personal data can be linked to you by the means of your userID: information about your log-on/log-off time, information on the websites you visited during working hours, …

### If you need any assistance or have any questions regarding privacy or cybersecurity in general, feel free to [contact us](https://www.ordina.be/diensten/security-and-privacy/).