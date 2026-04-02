# Week 4 SOC Workflow Steps

## Attack Simulation
1. Exploit Metasploitable2 Samba using Metasploit `usermap_script`.
2. Set LHOST and RHOSTS, choose payload `cmd/unix/reverse`.
3. Run exploit and verify shell session.

## Detection and Triage
1. Configure Wazuh to alert on Samba exploit.
2. Create TheHive case for the alert.
3. Document alert details and MITRE Technique.

## Response and Containment
1. Isolate the VM.
2. Block attacker IP with CrowdSec.
3. Verify containment via ping.

## Escalation
1. Escalate TheHive case to Tier 2 with summary.

## Reporting
1. Write SANS-style report (Google Docs / PDF).
2. Draft stakeholder briefing (non-technical).
