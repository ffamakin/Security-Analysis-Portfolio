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


1. Overview
==================
The recipient (johnsmith123@gmail[.]com) received an email with the subject "Website contact form submission" containing a mail delivery failure notice with an attached .eml message. My task was to analyse the raw email headers and the attached original message to establish where the email really came from, what it was trying to achieve, and extract all indicators of compromise.
This was a contact form abuse / spam injection attack, where a scammer abused a legitimate website's contact form to distribute get-rich-quick scam links.

2 Analysis Process
=======================================
2.1 Email Header Analysis/IOC Extraction 
Recipient kinnar1975@yahoo.co.uk 
Email Subject: Undeliverable: Website contact form submission
Date and Time of email: 18 March 2021 04:14
Originating IP Address: 103.9.171.10
URL: hxxps[:]//35000usdperwwekpodf[.]blogspot[.]sg?p=9swghxxps[:]//35000usdperwwekpodf[.]blogspot[.]co[.]il?o=0hnd (defanged)
Resolved Host on IP Address: c5s2-1e-syd.hosting-services.net.au (fromusing the whoisdomain lookup website)
<img width="438" height="119" alt="image" src="https://github.com/user-attachments/assets/446e78e6-dfea-4e00-8211-8a71ca669f53" />
Hosting Service for Webpage: Blogspot
<img width="801" height="312" alt="image" src="https://github.com/user-attachments/assets/80232273-c548-4004-a585-a9299e6dd96d" />
FileName: Website contact form submission.eml

<img width="443" height="93" alt="image" src="https://github.com/user-attachments/assets/c8702f5f-9c2f-4ec9-9598-5101523e7308" />

spf=none; dmarc=none; dkim=none; arc=none these headers do not pass (The sending domain had not SPF, DKIM and DMARK which throwa up a red flag as we are unable to verify the sender's authenticity)

#Verdict
==================
Confirmed malicious, financial scam (get-rich-quick lure) distributed via contact form abuse. No SPF/DKIM/DMARC, an originating IP belonging to a web hosting server rather than a mail provider.

# Recommended response actions:
Block the scam URLs and both IPs at th block list
Search the mail environment for other messages containing the Blogspot domains and purge them
Report the URLs to Google (already actioned- page removed) and the abused website's owner/host, so they can add CAPTCHA/validation to their contact form

N.B: This write-up documents methodology and findings for portfolio purposes. Completed as part of the Blue Team Labs Online phishing analysis track.




