# cyart-soc-team

# Week 2 – SOC Alert & Incident Response Exercises

## Overview
This folder contains Week 2 exercises for Security Operations Center (SOC) training.  
The focus is on **alert prioritization, incident classification, basic incident response, evidence preservation, and full alert-to-response simulations**.  
These exercises develop hands-on skills for detecting, triaging, responding to, and documenting security incidents using real-world frameworks and SOC tools.

---

## 1. Theoretical Knowledge

### 1.1 Alert Priority Levels
- **Core Concepts:**  
  - Severity levels based on **impact** (data loss, service disruption) and **urgency** (active exploitation).  
  - Example: **Critical = ransomware encryption**, **High = unauthorized admin access**.

- **Assignment Criteria:**  
  - Consider **asset criticality**, **exploit likelihood**, and **business impact**.  
  - Example: CVSS 9.8 (Log4Shell, CVE-2021-44228) → Critical.

- **Tools & Scoring:**  
  - CVSS for risk scoring  
  - SOC dashboards (Wazuh, Splunk) for alert prioritization

- **Learning Resources:**  
  - [FIRST CVSS Guide](https://www.first.org/cvss/)  
  - NIST SP 800-61 – Incident Severity Classification  
  - Real-world case studies (e.g., CISA alerts)

---

### 1.2 Incident Classification
- **Core Concepts:**  
  - Categories: Malware, Phishing, DDoS, Insider Threats, Data Exfiltration  
  - Frameworks: **MITRE ATT&CK**, **ENISA Incident Taxonomy**, **VERIS**  
  - Enrich incidents with **metadata**: affected systems, timestamps, IOCs

- **Learning Resources:**  
  - MITRE ATT&CK Mapping  
  - ENISA & VERIS Documentation  
  - SANS Phishing Case Studies

---

### 1.3 Basic Incident Response
- **Incident Lifecycle:**  
  1. Preparation – Playbooks & Policies  
  2. Identification – Alert Triage  
  3. Containment – Isolate Systems  
  4. Eradication – Remove Malware  
  5. Recovery – Restore Services  
  6. Lessons Learned – Post-Mortem

- **Procedures:**  
  - System isolation, evidence preservation, communication protocols, SOAR tools (Splunk Phantom)

- **Learning Resources:**  
  - NIST SP 800-61  
  - SANS Incident Handler’s Handbook  
  - Let’s Defend Simulated Scenarios

---

## 2. Practical Application

### 2.1 Alert Management Practice
**Tasks:**
- Create alert classification system in Google Sheets
- Prioritize alerts using CVSS
- Visualize alerts in Wazuh dashboards
- Draft incident tickets in TheHive
- Role-play escalation emails for critical alerts

**Sample Alert Table:**

| Alert ID | Type             | Priority | MITRE Tactic |
|----------|-----------------|----------|--------------|
| 001      | Phishing        | High     | T1566        |
| 002      | Brute-force SSH | Medium   | T1110        |

**Checklist:**
- [ ] Create Google Sheets table for alerts  
- [ ] Assign CVSS scores  
- [ ] Configure Wazuh dashboard visualization  
- [ ] Draft TheHive ticket for critical alerts  
- [ ] Write escalation email (100 words)

---

### 2.2 Response Documentation
**Tasks:**
- Create incident response templates in Google Docs
- Document investigation steps
- Conduct a mock post-mortem

**Sample Investigation Table:**

| Timestamp            | Action                  |
|----------------------|------------------------|
| 2025-08-18 14:00:00 | Isolated endpoint       |
| 2025-08-18 14:30:00 | Collected memory dump   |

**Checklist:**
- [ ] Executive Summary  
- [ ] Timeline of events  
- [ ] Impact Analysis  
- [ ] Remediation Steps  
- [ ] Lessons Learned

---

### 2.3 Alert Triage Practice
**Tasks:**
- Simulate alert triage in Wazuh
- Validate IOCs using VirusTotal or AlienVault OTX

**Sample Triage Table:**

| Alert ID | Description         | Source IP     | Priority | Status |
|----------|-------------------|---------------|----------|--------|
| 002      | Brute-force SSH    | 192.168.1.100 | Medium   | Open   |

**Checklist:**
- [ ] Analyze mock alert in Wazuh  
- [ ] Cross-check IP/file hash with Threat Intelligence  
- [ ] Document findings in 50 words

---

### 2.4 Evidence Preservation
**Tools:** Velociraptor, FTK Imager

**Tasks:**
- Collect volatile data (network connections)
- Acquire memory dump & hash with SHA256

**Sample Evidence Table:**

| Item       | Description   | Collected By | Date       | Hash Value |
|------------|---------------|-------------|------------|------------|
| Memory Dump| Server-X Dump | SOC Analyst | 2025-08-18 | <SHA256>  |

**Checklist:**
- [ ] Collect volatile data (netstat)  
- [ ] Acquire memory dump  
- [ ] Generate SHA256 hash  
- [ ] Document chain-of-custody

---

### 2.5 Capstone Project: Full Alert-to-Response Cycle
**Tasks:**
- Simulate attack using Metasploitable2 (e.g., VSFTPD backdoor exploit via Metasploit)
- Detect alerts in Wazuh
- Triage & isolate VM
- Block attacker via CrowdSec
- Document & report incident

**Sample Detection Table:**

| Timestamp            | Source IP     | Alert Description | MITRE Technique |
|----------------------|---------------|-----------------|----------------|
| 2025-08-18 11:00:00 | 192.168.1.100 | VSFTPD exploit   | T1190           |

**Checklist:**
- [ ] Exploit Metasploitable2 vulnerability  
- [ ] Configure Wazuh alert rules  
- [ ] Isolate VM & block attacker IP  
- [ ] Document incident in Google Docs (200 words)  
- [ ] Prepare stakeholder briefing (100 words)

---

## 3. Submission Guidelines
- **Deadline:** Friday, 4:30 PM  
- **Repository:** `cyart-soc-team`  
- **Folder Structure:**  
