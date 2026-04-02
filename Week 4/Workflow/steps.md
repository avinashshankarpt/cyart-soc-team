# SOC Workflow (Week 4)

## 1. Attack Simulation
- Used Metasploit to exploit Samba vulnerability

## 2. Detection
- Wazuh generated alerts for suspicious activity

## 3. Triage
- Alerts analyzed in TheHive
- Observables added (IP, hash)

## 4. Response
- Blocked attacker IP using CrowdSec
- Isolated compromised system

## 5. Evidence Analysis
- Used Velociraptor to analyze netstat
- Identified suspicious connection on port 4444

## 6. Automation
- Created playbook in TheHive
- Automated IP blocking

## 7. Post-Incident Analysis
- Performed 5 Whys root cause analysis
- Created Fishbone diagram

## 8. Metrics
- MTTD: 2 hours
- MTTR: 4 hours
- Dwell Time: 6 hours
