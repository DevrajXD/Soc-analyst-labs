
# Phishing Detection & Triage (Splunk) – SOC L1 Simulation

Lab Type: Phishing Investigation  
Tools Used: Splunk (Dev), Threat Intel Lookup, URL Scanner  
Skills Practiced: Alert classification, triage workflow, IOC analysis, incident documentation  
Dataset: Simulated TryHackMe SOC L1 scenario (fully artificial)

---

## 1. Summary

Investigated multiple alerts triggered by phishing emails sent to test users.  
Validated suspicious URLs, enriched indicators, and classified alerts as true positives.

---

## 2. Alerts Investigated

| Alert ID | Type      | Severity | Status     |
|---------|-----------|----------|------------|
| 8815    | Phishing  | Medium   | True Positive |
| 8816    | Firewall  | High     | True Positive |
| 8817    | Phishing  | Medium   | True Positive |


## 3. Investigation Workflow

### Step 1 — Alert Validation
- Opened the alert in Splunk  
- Reviewed raw logs  
- Verified email headers and URL indicators  

### Step 2 — IOC Enrichment
- Checked URL/IP reputation  
- Looked up WHOIS details  
- Confirmed malicious indicators  

### Step 3 — Correlation
- Cross-checked with firewall/proxy logs  
- Identified affected users  
- Traced interaction timeline  

### Step 4 — Classification
- Categorized alerts as true positives  
- Justified classification with evidence  

---

## 4. Screenshots (Evidence)

<img width="1822" height="865" alt="Screenshot 2025-11-09 150354" src="https://github.com/user-attachments/assets/effa1fcf-8dc2-4829-b256-7caf11ede155" />

<img width="1808" height="835" alt="Screenshot 2025-11-09 150407" src="https://github.com/user-attachments/assets/c6bc0597-1279-4163-ba14-c30347660145" />


## 5. Key Learnings

- How to enrich phishing URLs/IPs  
- How Splunk searches work  
- How to classify alerts using SOC methodology  
- Understanding severity, dwell time, and resolution time  

---

## 6. Disclaimer
This simulation uses only artificial data.  
No real users, companies, or sensitive logs were involved.
