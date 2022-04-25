---
layout: post
title:  "Network Segmentation Part 4"
author: jordy_bekaert
categories: [ ]
image: assets/images/Posts/NetworkSegmentation/image1.jpeg
description: "Network Segmentation Part 4"
featured: true
hidden: false
---

In the previous articles, we have looked the concept of network segmentation. In this article, I will introduce best practices of the network segmentation.

Top 10 Network (micro)segmentation best practices
=================================================

\#1 Data classification - know your crown jewels (the golden nuggets)
---------------------------------------------------------------------

Perform data classification, meaning:

-   know your ‘crown jewels’, the ‘company golden nuggets’, and

-   identify valuable / sensitive / business critical data and assets

Not all assets and data in your organization have the same business criticality, value and sensitivity (when leaked outside). **Assigning levels of importance is crucial as the first step of doing network segmentation.** So these labels should take into account both the **sensitivity of the data** (i.e. from public to strictly confidential) and **the importance of the systems and applications holding and/or processing that data**. These labels will later be used to define the (micro) segmentation policies and zones of trust within the company network, optionally in accordance to applicable regulations (such as PCI-DSS, Payment Card Industry – Data Security Standard).

\#2 Map data flows across the network – know who needs what data
----------------------------------------------------------------

Knowing who needs what data is crucial. Although network segmentation and the respective sets of controls bound to those segments make it more difficult for an attacker to laterally move through the network and accomplishing initial access, there are a number of legitimate data flows that need to be permitted and respected. All those legitimate data flows across all the systems should be mapped, including:

-   north-bound traffic: exiting outbound traffic, like employees visiting salesforce.com from managed devices connected to the corporate network

-   east-West traffic: traffic between systems inside the same network perimeter, such as a front-end webserver and back-end database servers in the data center network

-   south-bound traffic: inbound data entering a network segment or zone. For instance, access of customers or employees to a web server located in a DMZ or the company’s intranet or extranet

\#3 Get your asset management straight and define asset groups
--------------------------------------------------------------

Certain assets serve similar purposes and often communicate to each other. Segmenting these systems off as a group from the rest makes sense, as the typical inter-systems communications are known and allowed.

When defining asset groups, it is also important to consider the sensitivity of the various assets on the corporate network. Any assets serving similar purposes and with similar sensitivity levels should be grouped together in one segment separating them from other assets with different trust levels or functions.

\#4 Deploy a segmentation gateway and create access control policies
--------------------------------------------------------------------

After defining the network segments, it’s important to set the access controls and enforce these boundaries and restrictions, which is done by deploying a segment gateway.

All network traffic entering and exiting that specific segment pass the segment gateway and because of that, an organization might need several segment gateways to implement its effective segmentation.

Intersegment traffic is inspected and checked against the configured policies. These policies should be defined based upon the principle of **least privilege** (sounds familiar?), which states that applications, devices and users should have the minimum level of permissions required to do their job. These permissions should be defined based upon the legitimate data flows identified in 6.2.

\#5 Perform periodic audits and reviews
---------------------------------------

Defining a network segmentation policy is not a one-time ‘set-and-forget’ action. Segmentation policies are needed to be periodically reviewed and updated in order to:

-   accommodate and align with changes in the business and resulting business requirements, re-orgs, etc

-   cope with initial logical design flaws or oversights

-   accommodate and align with risk changes


*To be continued in part 5..*

### Ordina is your partner in this journey and enables you to go ahead of change against the security challenges of the digital age. If you need any assistance with cybersecurity, want training for your employees or have any questions regarding cybersecurity within your company, don’t hesitate to [contact us](https://www.ordina.be/diensten/security-and-privacy/).