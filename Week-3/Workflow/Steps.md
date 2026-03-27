 # SOC Workflow Steps

## Step 1: Log Ingestion

* Uploaded CSV logs into Elastic
* Created index: `advanced-log-analysis`

## Step 2: Log Correlation

* Filtered Event ID 4625
* Identified suspicious outbound traffic

## Step 3: Anomaly Detection

* Created detection rule:
  bytes_out > 1000000
* Generated alerts

## Step 4: Log Enrichment

* Created GeoIP pipeline
* Enriched destination_ip

## Step 5: Threat Intelligence

* Imported OTX feed into Wazuh
* Created custom IOC rule

## Step 6: Threat Hunting

* Query used:
  rule.mitre.id:"T1078"

## Step 7: Incident Escalation

* Created case in TheHive
* Escalated to Tier 2

## Step 8: Evidence Collection

* Used Velociraptor
* Collected memory dump
* Verified using SHA256

## Step 9: Capstone Simulation

* Exploited Samba (Metasploit)
* Detected in Wazuh
* Blocked using CrowdSec
* Escalated via TheHive

---

