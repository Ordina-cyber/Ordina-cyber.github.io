---
layout: post
title: "Risk Management for Security Professionals 1 : What is Risk?"
author: "kozue_connor"
categories: [ security-management ]
image: assets/images/isovsnist.jpg
description: "Risk Management for Security Professionals 1 : What is Risk?"
featured: true
hidden: false
---

Security is an important topic for many companies but if you think only security is the matter, you may go too far or wrong direction. Through this blog series, I will explain risk management general and look from a bit higher viewpoint than the security scope.

## Risk includes probability

In one of the most common risk management frameworks ISO 31000:2018 Risk Management – Guidelines, risk is defined as *“<u>effect of uncertainty on objectives</u>”*. For those who are not familiar with risk management, *“<u>the possibility of something bad happening</u>”* (Cambridge Dictionary (online)) may be easier to understand. The point here is that risk includes probability.

Image below is example of a common risk assessment approach, risk heat map (or risk matrix). In this approach, risks are assessed by 2 or more dimensions including likelihood (or probability).

**Risk Heat Map**

<table>
<colgroup>
<col style="width: 30%" />
<col style="width: 23%" />
<col style="width: 23%" />
<col style="width: 23%" />
</colgroup>
<thead>
<tr class="header">
<th><span style="float: right;">Impact</span>
    <br><br>
        <span>Likelihood</span></th>
<th>Low - 1</th>
<th>Medium - 2</th>
<th>High - 3</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Very Likely - 3</td>
<td style="background-color: #515115;">3</td>
<td style="background-color: #88541B;">6</td>
<td style="background-color: #EC5A54;">9</td>
</tr>
<tr class="even">
<td>Likely - 2</td>
<td style="background-color: #515115;">2</td>
<td style="background-color: #88541B;">4</td>
<td style="background-color: #88541B;">6</td>
</tr>
<tr class="odd">
<td>Unlikely - 1</td>
<td style="background-color: #3F7820;">1</td>
<td style="background-color: #515115;">2</td>
<td style="background-color: #515115;">3</td>
</tr>
</tbody>
</table>

<br>
## Problem is not Risk

There are several terms often get confused with risk. Let’s check these concepts in the table below.

<table>
<colgroup>
<col style="width: 16%" />
<col style="width: 49%" />
<col style="width: 16%" />
<col style="width: 18%" />
</colgroup>
<thead>
<tr class="header">
<th>Term</th>
<th>Definition</th>
<th colspan="2">Example</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>Threat</td>
<td><em>“potential cause of an unwanted incident, which can result in harm to a system or organization”</em> (ISO/IEC 27000:2018)</td>
<td>Fire</td>
<td>Information disclosure</td>
</tr>
<tr class="even">
<td>Vulnerability</td>
<td><em>“weakness of an asset or control that can be exploited by one or more threats”</em> (ISO/IEC 27000:2018)</td>
<td>Lack of fire extinguisher</td>
<td>Poor access management</td>
</tr>
<tr class="odd">
<td>Hazard</td>
<td><em>“something that is dangerous and likely to cause damage”</em> (Cambridge Dictionary (online))</td>
<td>Large amount of gasoline</td>
<td>A compromised user credential</td>
</tr>
<tr class="even">
<td>Problem</td>
<td><p><em>“a situation, person, or thing that needs attention and needs to be dealt with or solved”</em> (Cambridge Dictionary (online))</p>
<p><em>“a cause, or potential cause, of one or more incidents”</em> ( ITIL® 4)</p></td>
<td>Lack of employees’ safety mindset</td>
<td>Lack of security personnel</td>
</tr>
</tbody>
</table>

In reality, threat is often used to label the risk (e.g. “fire risk”), but you need to consider the probability when you discuss about the risk. In security area, it is also common to describe risk with threat and vulnerability like *“risk = threat \* vulnerability”* (Certified Information Systems Security Professional (CISSP) Official Study Guide 9<sup>th</sup> Edition).

## Risk is not Limited to Negative Risk

By the way, the ISO 31000 risk definition *“effect of uncertainty on objectives”* has some notes including *“An effect is a deviation from the expected. <u>It can be positive, negative or both</u>, and can address, create or result in opportunities and threats.”*. We normally look risks negatively but this note highlights that risk is actually not limited to negative risks. Investment is an example area that manages positive risks. Imagine a situation you are about to invest in a stock. You may select a newly launched business even probability of the business failure is more than large infrastructure companies. Why? Because the probability that the stock price will jump up is high as well.

Reducing risks may ruin opportunities of the positive effect too. That is why risk appetite *(*ISO 31000:2018 refers *“amount and type of risk that may or may not be taken”*) must be established based on the company’s context, and commitment of the management is essential for it. Risk management is indivisible from business strategy, so to say.

***Reference***

*ISO 31000:2018 Risk management — Guidelines, https://www.iso.org/iso-31000-risk-management.html*