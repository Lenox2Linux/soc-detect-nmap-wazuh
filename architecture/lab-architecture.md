# Lab Architecture

## Overview
This lab used a simple attacker-target-monitoring workflow.

- **Kali Linux VM** acted as the attacker machine
- **Ubuntu endpoint** acted as the monitored target
- **Wazuh** collected and displayed endpoint security events

## Flow
1. Kali Linux launched in VirtualBox
2. Nmap scanned the Ubuntu target
3. SSH access was attempted against the target
4. Wazuh captured authentication-related events
5. Alerts were reviewed through the Wazuh dashboard

## Roles
- **Attacker:** Kali Linux
- **Target:** Ubuntu endpoint
- **SIEM/Monitoring:** Wazuh
- **Analyst:** User reviewing dashboard evidence
