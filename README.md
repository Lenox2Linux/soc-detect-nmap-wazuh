# SOC Detection Lab: Nmap Scan Observed in Wazuh

## Overview

This project documents a simple SOC detection exercise in which network scanning activity was generated with Nmap and reviewed through Wazuh. The goal was to better understand how attacker behavior can appear in a monitored environment and how defensive tools can help identify suspicious activity.

## Objective

- Generate scan activity with Nmap
- Observe whether the activity appeared in Wazuh
- Practice connecting offensive actions to defensive visibility
- Document the workflow as part of a hands-on SOC lab

## Tools Used

- Nmap
- Wazuh
- Kali Linux
- Ubuntu/Linux lab systems
- Homelab network environment

## Detection Workflow

1. Prepared the lab systems and confirmed connectivity.
2. Generated scan activity using Nmap from the attacker system.
3. Reviewed logs and alerts in Wazuh.
4. Compared scan behavior with what was visible from the defender side.
5. Documented screenshots and results.

## What I Learned

This project helped me understand that detection work is not just about running tools, but about interpreting what activity looks like from both the attacker and defender perspective. It also reinforced the relationship between network scanning, log visibility, and alerting.

## Screenshots## 

### 1. Kali Linux Attacker VM

The Kali virtual machine used to simulate attacker activity in the lab.

![Kali Linux attacker VM](screenshots/kali-attacker-vm.jpeg)

### 2. Nmap Reconnaissance Results

Nmap identified the target host as active and detected an open SSH service on port 22.

![Nmap scan results](screenshots/nmap-scan-results.jpeg)

### 3. SSH Access Attempt

An SSH login attempt was made from the Kali system to the Ubuntu target. The login attempt failed, but it generated authentication-related activity for review.

![SSH failed login](screenshots/ssh-failed-login.jpeg)

### 4. Wazuh Dashboard Overview

The Wazuh dashboard displayed collected security events from the monitored endpoint.

![Wazuh dashboard overview](screenshots/wazuh-dashboard-overview.jpeg)

### 5. Wazuh Authentication Alerts

Wazuh reflected multiple authentication-related events associated with the SSH attempt.

![Wazuh authentication alerts](screenshots/wazuh-authentication-alerts.png)

## Related Project

For the broader Wazuh lab environment, see the related repository:
`soclab-wazuh`
