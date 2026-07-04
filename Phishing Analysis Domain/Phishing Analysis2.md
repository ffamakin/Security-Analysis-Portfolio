#BTLO Phishing Analysis Level 2 Hands-on phishing email analysis write-ups covering header analysis, IOC extraction, URL/attachment sandboxing, and verdict reporting.

Scenario: Put your phishing analysis skils to the test by triaging and collecting information about a recent phishing campaign.
<img width="575" height="175" alt="image" src="https://github.com/user-attachments/assets/5c09016f-f097-472e-a9c7-ed3fd087ab6e" />

Lab Details can be gotten from here: https://blueteamlabs.online/home/challenge/phishing-analysis-2-a1091574b8

BTLO Phishing Analysis 1
| Tools Used: Thunderbird, Text Editor, VirusTotal, | Date | June 2026 |

Objective
Investigate the email and attachment to collect useful artifacts.

Analysis Tools
We made use of Thunderbird as our email clent, Notepad as text editor and URL2PNG for url analysis

Q1: What is the sending email address? Opening the emailin Thunderbird, the sender is: amazon@zyevantoby.cn
<img width="350" height="114" alt="image" src="https://github.com/user-attachments/assets/1b7277be-1541-424f-a645-014c5cc673d5" />

Q2: What is the recipient email address? saintington73@outlook.com 
Q3:What is the subject line of the email? Your Account has been locked
Q4: What company is the attacker trying to imitate? From the body of the email, Amazon is the company
<img width="675" height="236" alt="image" src="https://github.com/user-attachments/assets/9205bd09-f0c7-48f1-9831-a9aa56eab417" />

Q5:What is the date and time the email was sent? From the text editor: Wed, 14 Jul 2021 01:40:32 +0900
<img width="415" height="95" alt="image" src="https://github.com/user-attachments/assets/b8207a7e-3ae2-45c1-ab00-57754099845c" />
Q6: What is the URL of the main call-to-action button? Embedded in the "Review Account" button: hxxps[:]//emea01.safelinks.protection[.]outlook[.]com/?url=hxxps%3A%2F%2Famaozn[.]zzyuchengzhika.cn%2F%3Fmailtoken%3Dsaintington73%40outlook[.]com&data=04%7C01%7C%7C70072381ba6e49d1d12d08d94632811e%7C84df9e7fe9f640afb435aaaaaaaaaaaa%7C1%7C0%7C637618004988892053%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C1000&sdata=oPvTW08ASiViZTLfMECsvwDvguT6ODYKPQZNK3203m0%3D&reserved=0

<img width="577" height="60" alt="image" src="https://github.com/user-attachments/assets/90ee7777-17c9-4a53-9bc4-54fcf36a5c63" />

Q7:  What is the first sentence (heading) displayed on this site? This web page could not be loaded.

<img width="513" height="127" alt="image" src="https://github.com/user-attachments/assets/a97df7bf-ae44-4643-98b7-0140f55f85d5" />
Q8: When looking at the main body content in a text editor, what encoding scheme is being used?
<img width="405" height="103" alt="image" src="https://github.com/user-attachments/assets/7257e826-663f-4832-8d07-895290f3e729" />
Q9: What is the URL used to retrieve the company’s logo in the email? We will be making use of Cyberchef and copy the base 64 code for analysis.
<img width="1507" height="812" alt="image" src="https://github.com/user-attachments/assets/ea4d009c-9cdf-4269-93ff-65a56b39a648" />
 hxxps[:]//images[.]squarespace-cdn[.]com/content/52e2b6d3e4b06446e8bf13ed/1500584238342-OX2L298XVSKF8AO6I3SV/amazon-logo?format=750w&amp;content-type=image%2Fpng
Q10: For some unknown reason one of the URLs contains a Facebook profile URL. What is the username (not necessarily the display name) of this account, based on the URL? amir.boyka.7
