### Phishing Email Triage Automation

## What This Project Does
A Python tootl that automates Tier 1 SOC Phishing investigation. 
It reads a phishing email (.eml file), extracts all suspicious URLs 
and IP addresses, checks each one against VirusTotal automatically,
and generates a structured triage report in under 2 minutes.

In a real SOC environment, this same process takes an analyst 
10-15 minutes per email when done manually. 

---
## Skills This project Demonstrates
- Python scripting and automation
- Email header forensics and IOC extraction
- VirusTotal API integration
- SOAR (Security Orchestration, Automation and Response) concepts
- Structured incident report writing

--- 
## How It Works
1. You run: python triage.py email.eml
2. The tool reads the email headers (sender, reply-to, routing path)
3. It extracts all URLs and IP addresses from the email body
4. It checks each one on VirusTotal (70+ security engines)
5. It writes a full triage report with a MALICIOUS or CLEAN verdict

---
## Files in This Repo
- triage.py  - run this to start the tool
- analyzer.py  - reads the email an extract IOCs
- vt_lookup.py  -  checks URLs/IPs on VirusTotal
- report_gen.py  - Formats and saves the output report
- requirements.txt -  pythons libaries needed
- smaple_reports/ -  3 example output report from real phishing samples
- screenshots/ -  proof the tool works

---
## MITRE ATT&CK Techniques Covered
| Technique | ID | How This Tool Helps |
| :--- | :--- | :--- |
| Phishing | T1566 | Detects malicious links in email body |
| User Execution | T1204 | Flags malicious URLs before user clicks |
| Credential Theft | T1056 | Identifies lookalike phishing domains |

---
## Sample Report Output
see Sample_reports/folder for full example reports.

---
## Setup Instructions 
1. Clone this repo
2. Run: pip install -r requirements.txt
3. Add you VirusTotal API key to a .env file: VT_API_KEY= your_key
4. Run: Python tirage.py your_email.eml

---
 ## Author
 Afeez Akorede | SOC Analyst | Comptia Security+
 linkedin.com/in/afeezakorede


## 📸 Project Screenshots

<img width="922" height="828" alt="sample-101-scan" src="https://github.com/user-attachments/assets/2ec0c84f-f64d-4a26-aa8b-1f87ca7fdd67" />


<img width="789" height="472" alt="sample-1-scan png" src="https://github.com/user-attachments/assets/4cc6e50f-b459-4483-b947-b40659ce8170" />


 <img width="751" height="352" alt="sample-10-scan png" src="https://github.com/user-attachments/assets/7be2fb6b-9a76-40ce-a323-6ce324a2b7a4" />


 
<img width="767" height="409" alt="sample-100-scan png" src="https://github.com/user-attachments/assets/6298ee82-07e5-4674-94f8-f2d74b6210b0" />

