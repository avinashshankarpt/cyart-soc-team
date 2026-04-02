 # Week 3 - SOC Advanced Operations

## 🔍 Overview

This project demonstrates advanced SOC operations including:

* Log Correlation
* Anomaly Detection
* Log Enrichment
* Threat Intelligence Integration
* Incident Escalation
* Alert Triage
* Evidence Collection
* Full SOC Workflow Simulation

---

## 🛠 Tools Used

* Elastic Security (ELK Stack)
* Wazuh SIEM
* AlienVault OTX
* TheHive
* CrowdSec
* Velociraptor
* Metasploit

---

## 📊 Key Outcomes

### 1. Log Correlation

* Detected failed login (Event ID 4625)
* Correlated with outbound traffic

### 2. Anomaly Detection

* Rule: `bytes_out > 1000000`
* Generated 6 high severity alerts

### 3. Log Enrichment

* GeoIP added country and location data

### 4. Threat Intelligence

* Integrated OTX with Wazuh
* Detected malicious IP

### 5. Incident Escalation

* Case created in TheHive
* Escalated to Tier 2

### 6. Evidence Collection

* Memory dump acquired
* SHA256 hash verified

### 7. Capstone

* Simulated Samba exploit
* Detected, blocked, escalated, reported

---
        +----------------------+
        |     Log Sources      |
        | Firewall / Endpoint  |
        +----------------------+
                    |
                    v
        +----------------------+
        |      ELK Stack       |
        | Elasticsearch/Kibana |
        +----------------------+
                    |
                    v
        +----------------------+
        |   Detection Rules    |
        |   (bytes_out > 1MB)  |
        +----------------------+
                    |
                    v
        +----------------------+
        |        Alerts        |
        +----------------------+
                    |
                    v
        +----------------------+
        |        Wazuh         |
        |  Correlation + TI    |
        +----------------------+
                    |
                    v
        +----------------------+
        |       TheHive        |
        |   Case Management    |
        +----------------------+
                    |
                    v
        +----------------------+
        |   SOC Response       |
        | Investigate/Contain  |
        +----------------------+
        
## 📌 Conclusion

This project simulates real-world SOC operations and demonstrates detection, response, and investigation capabilities.

---

