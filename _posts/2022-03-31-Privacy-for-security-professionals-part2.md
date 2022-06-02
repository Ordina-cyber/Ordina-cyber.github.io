---
layout: post
title: "Privacy for security professionals 2 : How to embed privacy requirements in the design of new systems & applications"
author: "jeffrey_van_moortel"
categories: [ Privacy ]
image: assets/images/Posts/GDPR/Classified_document.jpg
description: "Privacy for security professionals 2 : How to embed privacy requirements in the design of new systems & applications"
featured: false
hidden: false
---

## How can I determine whether GDPR is applicable or not for an application/system?
Without going into ‘territorial’ details, the answer is rather simple: if your application/system is processing(*) personal data, then privacy legislation (e.g. GDPR) **IS** applicable.

But now, to what extent should privacy legislation be taken into account? Do we need to do a full privacy assessment if we only process a limited amount of personal data?

(*) **processing**: also hosting personal data, without doing anything else with this data, is seen as a “data processing activity”.

## How to embed privacy requirements in the design of new systems & applications?
Most companies use some **standard (or custom developed) questionnaire**, which are very similar to for example SDLC (Software Development Life Cycle) intakes. Typical privacy related questions (to be answered by business) can be:

- *Of which data subjects will personal data be processed?*
- *What kind of personal data will be processed? Will special category personal data be processed?*
- *What is the volume of records of personal data to be processed?*
- *Will there be outsourcing of some personal data processing activities to one or more vendors?*

Such “privacy intake” questionnaire, as you could call it, should help to estimate the ‘level’ of impact for privacy for this application. This is not an exact calculation but should lead to one of 3 possible outcomes:

- **NONE**; no personal data processed whatsoever
- **LIGHT**; personal data is processed but for a small group of people, no special category data, …
- **FULL**; lots of personal data records, vulnerable data subjects, special category data, outsourcing, …

Determining privacy requirements is difficult starting with a blank sheet. Just like you might use for example ISO27001 as a best practice for information security, you can use an existing framework for privacy/data protection that covers the most important topics (e.g. Nymity Privacy Framework, NIST Privacy Framework, ISO27701, …). Some important topics that should be addressed and which are represented in all these frameworks:

- Security & privacy by design: Technical & organizational measures (e.g. privacy design strategies)
- DPIA (Data Protection Impact Assessment) or not to DPIA
- Update record of processing activities
- Supplier relation (e.g. data processing agreements)
- Data retention requirements
- Data subject rights
- Data breach management

Listing all privacy requirements for a new project isn’t a walk in the park. Stick to standard privacy frameworks/checklists which will prevent you from neglecting several important data protection domains. Not all domains are always applicable, but once you’ve done a first assessment & filtering you can focus on the privacy domains you need to retain. From that point on, you can start translating the general privacy principles/guidelines into more specific privacy requirements for the project you are working on.


### If you need any assistance or have any questions regarding privacy or cybersecurity in general, feel free to [contact us](https://www.ordina.be/diensten/security-and-privacy/).