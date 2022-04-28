---
layout: post
title:  "Network Segmentation Part 5"
author: jordy_bekaert
categories: [ ]
image: assets/images/Posts/NetworkSegmentation/image1.jpeg
description: "Network Segmentation Part 5"
featured: true
hidden: false
---

Continuing from the previous article, I will introduce best practices of the network segmentation.

\#6 Automate where possible
---------------------------

Defining network segmentation policies can be a huge task if one has to do it manually, especially at large enterprise networks. So automatic provisioning is key in order to succeed.  
Also in the early stages of discovery and classification, automation can be crucial for identifying newly added network assets, their traffic flows, vulnerability scanning and segmentation policy application.

\#7 Don’t over-segment or under-segment
---------------------------------------

Segmentation projects can be tricky. A good successful segmentation plan only entitles the necessary (micro) segments needed; overdoing micro segmentation makes everything too complicated but insufficient segmentation threatens your security.

This is why **knowing who needs what data** is important**.** If you don’t have a good view of your users and what they need to do their jobs, you may end up over-segmenting or under-segmenting. This is a common issue, and it means you might have to eventually go in and change the whole network. A few years ago, Gartner found that more than 70% of segmentation projects had to be redone because of over-segmentation.

\#8 Limit and segment third-party access
----------------------------------------

Third-party remote access risks remain a key vulnerability for organizations, since several vendor reports point out that giving too much privileged access to third parties, is still one of the biggest causes of security breaches.

“*Providing remote access to third parties without implementing the appropriate security safeguards is almost guaranteeing a security incident and a data breach involving sensitive and confidential information*,” said Dr. Larry Ponemon, Chairman and Founder of Ponemon Institute. ***“It is important that organizations assess the security and privacy practices of the third parties that have access to their networks and ensure that they have just enough access to perform their designated responsibilities and nothing more.”***

One way to mitigate this risk is to create isolated portals for third parties that need access to your network to provide services. This keeps their access limited to only necessary areas of your network. 

\#9 Make sure the legitimate path to data is easier that the illegitimate path
------------------------------------------------------------------------------

When segmenting your network, keep the architecture of your network in mind.

If there are only two firewalls between a bad actor and the data you need to be protected, but three or four between your vendors and the same data, it’s time to reorganize your architecture, so that the illegitimate path becomes the more difficult one. By the way, bad actors always choose the path of least resistance.

 \#10 Audit and monitor your network regularly
---------------------------------------------

It’s a process! Yes it is, segmentation is not a one-time ‘set and forget’ action. As the world evolves, so is the market, your business, your organization and also the organizational needs. So change management is key here.

Also, when auditing and monitoring your networks on a regular basis, the chance you’re missing gaps in your architecture that might be exploited by a bad actor decreases. We’re all human, right?

Important side remark about PCI-DSS
===================================

Network segmentation is required for PCI-DSS (Payment Card Industry Data Security Standard) compliance. Organizations that store, process and/or transmit payment card data must comply with PCI-DSS, which requires the organization to keep the cardholder data environment (CDE) separated from the other parts of the network by using network segmentation. With network segmentation, payment card data at rest, as well as in transit is being isolated and foreseen with separate and specific controls to better safeguard confidentiality and integrity of this data.

Conclusion
==========

Organizations are increasingly being challenged every day by bad actors, who are quickly gaining capabilities in breaching company security perimeters. The most important root cause of bad actors succeeding, is that anno 2022 still a lot of organizations operate a rather historical network architectures. The implementation of a Zero Trust Architecture will tremendously lower the risk of suffering data breaches.

Network (micro) segmentation is a requirement and the very basic foundation a Zero Trust Architecture is built upon. You cannot deploy and automate intelligent security controls if those controls are not specifically configured to secure a granular set of resources.

***Analogy: if you live in a house with only one big room, and all your belongings are laying around, guess what is being stolen when a thief steps in? Yes, the most precious goodies.***

There are some technical challenges in defining and implementing a strong and sustainable segmentation strategy, but throughout the years we’ve learned how to deal with those.  
  
Understanding the business of your organization, knowing the organization’s ‘crown jewels’ or ‘golden nuggets’ and who is in a need of which data, are key requirements and the most important information to start working with.

*Sources*
=======

- *[<u>Announcing the Azure Sentinel: Zero Trust (TIC3.0) Workbook - Microsoft Tech Community</u>](https://techcommunity.microsoft.com/t5/public-sector-blog/announcing-the-azure-sentinel-zero-trust-tic3-0-workbook/ba-p/2313761)*
- *[<u>Zero Trust Architecture (nist.gov)</u>](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-207.pdf)*
- *[<u>What Is Network Segmentation? - Palo Alto Networks</u>](https://www.paloaltonetworks.com/cyberpedia/what-is-network-segmentation)*
- *[<u>Network Segmentation Security Best Practices - Check Point Software</u>](https://www.checkpoint.com/cyber-hub/network-security/what-is-network-segmentation/network-segmentation-security-best-practices/)*
- *[<u>5 Network Segmentation Best Practices to Maximize… \| SecurityScorecard</u>](https://securityscorecard.com/blog/network-segmentation-best-practices-to-maximize-cybersecurity)*
- *[<u>7 Network Segmentation Best Practices to Level-up \| strongDM</u>](https://www.strongdm.com/blog/network-segmentation)*

### Ordina is your partner in this journey and enables you to go ahead of change against the security challenges of the digital age. If you need any assistance with cybersecurity, want training for your employees or have any questions regarding cybersecurity within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).