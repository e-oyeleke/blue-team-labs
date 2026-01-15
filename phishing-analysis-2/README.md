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

| Field | Value |
|------|------|
| Receiver Address | saintington73@outlook[.]com |
| Sender Address | amazon@zyevantoby[.]cn |
| Subject | Your Account has been locked |
| Date | Wed, 14 Jul 2021 01:40:32 +0900 |
| Sender IP | 103.9.171.10 |
| Malicious URL | hxxps[://]emea01[.]safelinks[.]protection[.]outlook[.]com/... |


## Observations
- URL was URL-encoded to obscure its final destination
- Decoded URL redirected to a third-party domain unrelated to the claimed sender
- Domain reputation appeared suspicious and inconsistent with legitimate services

## Lessons Learned
- URL encoding is commonly used to evade detection
- Header analysis remains critical even when payloads are simple
- Basic phishing attempts still rely heavily on social engineering
