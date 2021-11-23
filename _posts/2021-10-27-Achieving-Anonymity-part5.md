---
layout: post
title:  "Achieving anonymity and what defines it part 5"
author: emmanouil_perselis
categories: [ ]
image: assets/images/digitalfingerprint.jpg
description: "Achieving anonymity and what defines it part 5"
featured: false
hidden: false
---

*This article is a re-edition of a chapter of **Panopticism Ex Machina: Practical ways to obtain anonymity, confidentiality of data and repudiability of actions on the internet and why it is necessary** (Emmanouil Perselis, 2019).*

## Concepts used in the anonymity chain

One of the main purposes of anonymity is the segregation of a user from an action. The main concepts needed to achieve anonymity are analyzed in this part. An abstract overview of the concepts will be given as well as the utility and the importance of those concepts as a part of the anonymity chain and how they masquerade PII (Personally identifiable information).

## Anonymous emails

Almost all online services and applications require an email address to function. Email addresses are used as a verification system to identify users, as well as a single point of contact of users. The main issue of this practice is that all well-known email providers require users to hand over PII that can be used to identify them.

One of the required PII is the telephone number of users, which is used for verification. Of course, somebody could easily fabricate all this information. The main issue is with telephone numbers because forged numbers aren't usable and most mobile providers will ask users to register themselves as the owners of the phone numbers. Many websites and other providers are also getting more aware of online SMS receiving services and require the registration of phone numbers to be unique.

This hassle can be overcome by simply registering with an email provider that does not require such information. Registering with anonymous email providers protects a user from the leakage of PII as none is required. The only concern of this practice is the way that somebody accesses those email service providers. By accessing this service, 1P addresses of users are logged and IP addresses are PII. The following sections provide a solution to this problem.

## Onion routing

Onion routing is a concept that describes a network of several nodes called onion routers, having as main goal the anonymization of users. When a user initiates a connection using this network, messages of the connection are wrapped with multiple layers of encryption in such a way it resembles the peels of an onion. Each onion router adds another "wrap" around the packet.

The user remains unknown since each mediating node is only aware of the immediately preceding and the immediately following node. This concept provides protection against IP disclosure. The most prevalent implementation of this concept is the TOR network used in the work-case.

## Public networks

Although less effective than the Onion Routing concept, the usage of public networks can add an extra isolation node to the anonymity chain. In a common communication model, a user uses his personal home network to communicate with the internet. If at any time an action is traced back to this IP address, it is almost certain that the actor is the person by whom the internet connection has been registered. On the contrary, if an action is traced back to an IP address belonging to a public network, the scope of possible actors includes all the persons present in this network at the time the action was done.

The catch of this concept is the fact that a person is not aware of the monitoring measures present at the public place or network at any time. Public places are often monitored by CCTV and network monitoring systems or may even require a registration. Those measures could leak PII, either technical or non-technical. The hiding of non-technical PII in public places is out of this scope. The technical PII that could be leaked in such a context is the MAC address of the network card as well as the type of network activity. The MAC address is trivially spoofed and is even done automatically by the operating system that will be used in the work-case. Hiding the network activity on a monitored network is possible through the usage of a VPN although using a VPN has side effects. Generally, it is advised not to use monitored public networks.

## Trusted and amnesic operating systems

The most widespread personal operating systems today monitor user activities. They justify this practice by telling that it is used for the benefit of the consumer. Although this could be true, this information has historically been used for spying purposes. This fact should be the main motive to only use trusted operating systems. The only way to scrutinize an operating system is by making the development process transparent. One possible way to achieve this is by making the project open source.

An amnesic operating system is an operating system that resets itself to its initial state after each subsequent boot without keeping any non-volatile data on the system it is used on. This principle allows a user to wipe all data on the machine he used that is a byproduct of his actions. This practice limits the information that can link a machine to a certain action, and thus, to the actor.

The above prerequisites are fulfilled by an operating system called zTails OS is used in the work-case.

## Anonymous and untraceable payment systems

Some of the techniques used to achieve anonymity are paid services, such as the usage of a VPN service. The common payment methods used today are directly linked with a user through PII provided by the user and law enforces the providers to verify the legitimacy of the user in most of the cases. Using those payment systems to set-up an anonymity chain would be catastrophic.

With the wider acceptance of cryptocurrencies by vendors, and the development of new technologies using Bblockchain, anonymous payment systems have been developed. Those payment systems allow the transfer of value without disclosing the participants of the transaction. Opening a cryptocurrency wallet does not need any verification or submission of any PII. The cryptocurrency that will be used in the work-case is Monero.

## Synopsis

Through this blog series, I analyzed what anonymity is constituted of, how information that can de-anonymize you can leak, as well as conceptual approaches to counter those leakages. Although those concepts seem to be abstract, they are the bedrock on which the nodes of the anonymity chain will be built upon. Importance was also placed on the notions of PII, the context and how they interweave. At this point the manifestation of those concepts is still left untouched and without a good grasp of the available technologies and their applications, some of those concepts cannot be actualized.
