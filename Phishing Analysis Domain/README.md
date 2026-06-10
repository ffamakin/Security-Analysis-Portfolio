#BTLO Phishing Analysis Level 1
Hands-on phishing email analysis write-ups covering header analysis,
IOC extraction, URL/attachment sandboxing, and verdict reporting.
Scenario: A user has received a phishing email and forwarded it to the SOC. Can you investigate the email and attachment to collect useful artifacts?
# BTLO Phishing Analysis 1
| Tools Used | Thunderbird, Sublime Text, VirusTotal, URL2PNG |
| Date | June 2026 |

## Objective
A user received a suspicious email and forwarded it to the SOC.
Investigate the email and attachment to collect useful artifacts.

Analysis Process
=======================================
# Step 1: Email Header Analysis
(What did you find in the From, To, Return-Path,
SPF/DKIM results? Was there a mismatch?)

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
