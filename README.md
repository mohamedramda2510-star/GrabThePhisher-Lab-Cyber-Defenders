GrabThePhisher Lab – Phishing Investigation Report

Platform: CyberDefenders
Category: Threat Intelligence
Difficulty: Easy
Level: SOC Analyst Tier 1 – Level 2
Tools: Text Editor, Telegram API
MITRE ATT&CK Tactics: Initial Access, Exfiltration
Status: Completed – 10/10 Questions

---

1. Lab Overview

The objective of this lab was to investigate a cryptocurrency phishing campaign targeting users of the PancakeSwap exchange.

The investigation revealed a phishing website impersonating the legitimate exchange to trick victims into submitting their MetaMask wallet seed phrases. The phishing kit was hosted on a compromised server and used a Telegram bot to exfiltrate stolen credentials.

The main goal was to analyze the phishing kit, extract IOCs, investigate the exfiltration mechanism, and identify information related to the threat actor.

2. Investigation Findings

#| Question| Finding

Q1| Targeted Wallet| MetaMask

Q2| Phishing Kit Filename| "metamask.php"

Q3| Programming Language| PHP

Q4| Geolocation Service| Sypex Geo

Q5| Previously Collected Seed Phrases| 3

Q6| Most Recent Incident Seed Phrase| Redacted

Q7| Credential Exfiltration Medium| Telegram

Q8| Telegram Channel Access Token| Redacted

Q9| Phisher's Channel Chat ID| "5442785564"

Q10| Developer Alias| "j1j1b1s@m3r0"

3. Technical Analysis

The investigation identified the following findings:

- Phishing Infrastructure: Identified "metamask.php" as the phishing kit's main file.
- Target Identification: The campaign targeted MetaMask wallet users.
- Code Analysis: Confirmed that the phishing kit was developed using PHP.
- Geolocation: Identified Sypex Geo as the service used to retrieve victim machine information.
- Credential Harvesting: Identified three previously collected wallet seed phrases.
- Data Exfiltration: Discovered that Telegram was used to transmit stolen credentials.
- Threat Actor Intelligence: Extracted the Telegram Chat ID and identified the phishing kit developer's alias.

4. Indicators of Compromise (IOCs)

Type| Indicator
File| "metamask.php"
Target| MetaMask
Geolocation Service| Sypex Geo
Exfiltration Channel| Telegram
Telegram Chat ID| "5442785564"
Developer Alias| "j1j1b1s@m3r0"

Note: Sensitive credentials, including wallet seed phrases and Telegram access tokens, have been redacted to prevent accidental exposure.

5. Evidence & Screenshots

Q1 – Targeted Wallet

Finding: MetaMask

Evidence:

<img width="1400" height="744" alt="Screenshot (69)" src="https://github.com/user-attachments/assets/1d7fddcf-27c5-42af-b66b-56f48d81244c" />


Q2 – Phishing Kit Filename

Finding: "metamask.php"

Evidence:

<img width="827" height="222" alt="Screenshot (70)" src="https://github.com/user-attachments/assets/5942a6ab-76a6-4ee4-8599-599c14453ecb" />


Q3 – Programming Language

Finding: PHP

Evidence:

<img width="1400" height="744" alt="Screenshot (69)" src="https://github.com/user-attachments/assets/f308c09f-78bb-45fe-8681-c7ebbd8d9ef0" />


Q4 – Geolocation Service

Finding: Sypex Geo

Evidence:

<img width="1423" height="745" alt="Screenshot (71)" src="https://github.com/user-attachments/assets/f1e0d792-2cc7-43a4-80c7-bd85c9cb16f4" />


Q5 – Previously Collected Seed Phrases

Finding: 3

Evidence:

<img width="1409" height="748" alt="Screenshot (72)" src="https://github.com/user-attachments/assets/f71964e8-324e-4f05-8ce0-ebb6bbde9aae" />


Q6 – Most Recent Phishing Incident

Finding: Seed phrase identified (redacted).

Evidence:

<img width="1420" height="753" alt="Screenshot (73)" src="https://github.com/user-attachments/assets/0548812f-e205-4a03-8354-594a660828ee" />


Q7 – Credential Exfiltration Medium

Finding: Telegram

Evidence:

<img width="1425" height="742" alt="Screenshot (74)" src="https://github.com/user-attachments/assets/8e40bef4-2711-4100-ac73-b7648dc3de3f" />


Q8 – Telegram Channel Access Token

Finding: Identified (redacted).

Evidence:

<img width="1394" height="725" alt="Screenshot (75)" src="https://github.com/user-attachments/assets/06ecb19f-2114-42fe-8198-f0ca400f280f" />


Q9 – Phisher's Channel Chat ID

Finding: "5442785564"

Evidence:

<img width="1395" height="750" alt="Screenshot (76)" src="https://github.com/user-attachments/assets/3e519d0f-8978-48fe-9379-a684a2658356" />


Q10 – Phishing Kit Developer Alias

Finding: "j1j1b1s@m3r0"

Evidence:


<img width="1404" height="739" alt="Screenshot (77)" src="https://github.com/user-attachments/assets/c8fa8470-4fa5-4af3-b821-54d9ee0cf51c" />


6. Skills & Knowledge Gained

- Phishing kit source code analysis.
- Cryptocurrency phishing investigation.
- Identifying credential harvesting techniques.
- Analyzing PHP-based phishing infrastructure.
- Understanding Telegram-based data exfiltration.
- Extracting IOCs and threat actor intelligence.
- Analyzing attacker communication channels.
- Threat intelligence and incident response.

7. Conclusion

This lab provided practical experience investigating a cryptocurrency phishing campaign targeting MetaMask users.

The investigation demonstrated how phishing kits collect sensitive wallet credentials and use Telegram for data exfiltration.

It also strengthened practical skills in IOC extraction, phishing infrastructure analysis, threat actor intelligence, and incident investigation from a SOC Analyst perspective.

Lab Status: Successfully Completed – 10/10 Questions.
