#BTLO Phishing Analysis Level 1 
Hands-on phishing email analysis write-ups covering header analysis,
IOC extraction, URL/attachment sandboxing, and verdict reporting.

Scenario: A user has received a phishing email and forwarded it to the SOC Team. My task was to analyse the email headers, body and embedded links to determine whether it was genuine phishing attmeot and extract indicatorsof compromise.
<img width="587" height="215" alt="image" src="https://github.com/user-attachments/assets/fff440d6-117b-4ede-aca9-bf96f02bb14f" />

Lab Details can be gotten from here: https://blueteamlabs.online/home/challenge/phishing-analysis-f92ef500ce

# BTLO Phishing Analysis 1
| Tools Used: Thunderbird, Sublime Text, VirusTotal, URL2PNG |
| Date | June 2026 |

# Objective
Investigate the email and attachment to collect useful artifacts.

Analysis Process
=======================================
# Step 1: Email Header Analysis
From Address: 
To Address: kinnar1975@yahoo.co.uk (Primary recipient)
Email Subject: Undeliverable: Website contact form submission
Date and Time of email: 18 March 2021 04:14
Originating IP Address: 103.9.171.10
Resolved Host on IP Address: c5s2-1e-syd.hosting-services.net.au
FileName: Website contact form submission.eml
URL: hxxps[:]//35000usdperwwekpodf[.]blogspot[.]sg?p=9swghxxps[:]//35000usdperwwekpodf[.]blogspot[.]co[.]il?o=0hnd (defanged)
spf=none; dmarc=none; dkim=none; arc=none
service hosted on webpage: 

# Step 2: Body & Content Analysis
(What social engineering tactics were used?
Urgency? Impersonation? Typos?)

# Step 3: URL / Attachment Investigation
(Did you sandbox anything? What did VirusTotal say?
What was the file hash?)

# Step 4: IOC Extraction
- **Sender:** 
- **Originating IP:** 
- **Malicious URL:** 
- **File Hash (SHA256):** 

# Verdict
(Malicious / Suspicious / Legitimate — explain WHY)

# What I Learned
(What was new to you? What would you do differently?)

# Screenshots
(Drag and drop images directly into the GitHub
