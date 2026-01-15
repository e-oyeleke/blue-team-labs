# Phishing Analysis 2

## Overview
This lab focuses on analyzing a second phishing email sample from Blue Team Labs Online.

## Objective
- Identify malicious indicators
- Analyze URLs and headers
- Determine attacker intent

## Tools Used
- Outlook email client (header extraction)
- URL2PNG (Snapshots of URL)
- CyberChef (URL Decoder)
- Notepad (Text editor)
  
## Email Overview
Reciever Address: saintington73@outlook[.]com
Sender Address: amazon@zyevantoby[.]cn
Subject: Your Account has been locked
Date: Wed, 14 Jul 2021 01:40:32 +0900
Sender IP: 103.9.171.10
Malicious URL: hxxps[://]emea01[.]safelinks[.]protection[.]outlook[.]com/?url=hxxps%3A%2F%2Famaozn[.]zzyuchengzhika[.]cn%2F%3Fmailtoken%3Dsaintington73%40outlook[.]com&data=04%7C01%7C%7C70072381ba6e49d1d12d08d94632811e%7C84df9e7fe9f640afb435aaaaaaaaaaaa%7C1%7C0%7C637618004988892053%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&sdata=oPvTW08ASiViZTLfMECsvwDvguT6ODYKPQZNK3203m0%3D&reserved=0

## Observations
-URL was URL-encoded to obscure its final destination
-Decoded URL redirected to a third-party domain unrelated to the claimed sender
-Domain reputation appeared suspicious and inconsistent with legitimate services

## Lessons Learned
URL encoding is commonly used to evade detection
Header analysis remains critical even when payloads are simple
Basic phishing attempts still rely heavily on social engineering
