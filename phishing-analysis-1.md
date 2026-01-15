## BTLO – Phishing Analysis 1

**Objective:**  
Analyze the provided email headers to determine whether the email was legitimate or malicious.

**Tools Used:**  
- Outlook email client (header extraction)  
- URL2PNG (Snapshots of URL)
- MXToolbox (Reverse DNS Lookup)
- WHOIS Lookup (Domain Name Lookup)

**Summary:**  s
The email headers were reviewed to trace the delivery path,check sender authenticity and validate authentication results.
Analysis included examining Received headers, Message-ID, and SPF/DKIM/ARC results using the Outlook email client. All headers
showed no relations to a malicious infrastructure, and no anomalies were observed. Based on the header analysis, the email was determined to be legitimate

## Indicators Observed
- No authentication failures observed (SPF/DKIM/DMARC/ARC)
- Consistent sender and infrastructure details
- Timestamps aligned across all hops
- No suspicious or unexpected email routing

## Analyst Action
- Email classified as legitimate
- No remediation required
- Case closed as informational
