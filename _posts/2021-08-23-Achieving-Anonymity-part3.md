---
layout: post
title:  "Achieving anonymity and what defines it part 3"
author: emmanouil_perselis
categories: [ ]
image: assets/images/digitalfingerprint.jpg
description: "Achieving anonymity and what defines it part 3"
featured: true
hidden: false
---

*This article is a re-edition of a chapter of **Panopticism Ex Machina: Practical ways to obtain anonymity, confidentiality of data and repudiability of actions on the internet and why it is necessary** (Emmanouil Perselis, 2019).*

## Personally identifiable information

Personally identifiable information or PII, is any information that gives the holder the capability to identify or to trace a single individual. PII is also any information that can logically be associated with an individual. According to NIST (National Institute of Standards and Technology, science laboratory of the United States Department of Commerce) the following information is classified as PII:


<table>
<tr>
<th>Non-technical</th>
<th>Technical</th>
</tr>
<tr>
<td>

* Full name
* Human physiognomy
* Home address
* National identification number
* Passport number
* Vehicle registration number
* Driver's license number
* Fingerprints or handwriting
* Creditcard number
* Date of Birth
* Place of Birth
* Genetic information
* Telephone number
* Pseudonym
* Alma mater
* Religion
* Financial information
</td>
<td>

* Web cookie
* Asset information (e.g. IP, MAC address)
* Email address
* Geographical indicators
</td>
</tr>
</table>

Although this guideline is a good starting point, in terms of technological evolution, it is relatively outdated and limited regarding the technical category as it was written in 2010. PII leaked through technological means will be covered in the following sections.

## Browser fingerprinting 

Modern day trackers can create an almost unique fingerprint out of browser information leaked while surfing on the internet. This fingerprint is essentially an amalgam of information leaked without requiring users to give any personal information or even their consent. Fingerprints do not directly lead to individuals but can be stored and later associated with PII given by users and hence, correlate the two with an individual. This leaked information can also act as an interconnection between two contexts.

Using an up-to-date Firefox Quantum V65.0 browser, a site called https://panopticlick.eff.org was visited. This site performs multiple tests, trying to create a digital fingerprint of our browser. After performing the test, and without giving any explicit authorization, a report was presented stating the following:

"Within our dataset of several hundred thousand visitors tested in the past 45 days, only one in 25042.17 browsers have the same fingerprint as yours. Currently, we estimate that your browser has a fingerprint that conveys 14.61 bits of identifying information."

The same test was performed with a similar site, https://amiunique.org. Having a more detailed analysis, it listed the attributes having the lowest similarity ratio, meaning they distinguish a browser the most. Those attributes are the following and are specific to the used browser context:
* The User agent, containing information about the browser and the operating system, having a similarity ratio of <0.1%.
* The rendering variation of the HTML5 Canvas, having a similarity ratio of <0.1%.
* The list of plugins, having a similarity ratio of 0.13%.
* The content language, having a similarity ratio of 0.32%.
* The screen resolution, having a similarity ratio of 2.12%.

This technique drastically narrows the scope of possible actors and will significantly limit the search surface. Luckily, according to the Electronic Frontier foundation and by leaked NSA documents, by applying two measures, the uniqueness of the browser fingerprint can be reduced. These two measures are the TorButton (a component of the Tor browser that applies application-level security) and NoScript (browser extension that disabled JavaScript, Java Flash and other plugins).

*To be continued in the next article...*