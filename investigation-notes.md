# Investigation Notes

## Scenario
A Kali Linux VM was used to perform reconnaissance and an SSH login attempt against a monitored Ubuntu endpoint in a home lab environment.

## Activity Observed
- Host discovery confirmed the target was online
- Nmap identified port 22 as open
- Service detection showed SSH was running
- An SSH login attempt failed
- Wazuh displayed authentication-related activity

## Analyst Interpretation
The activity in this lab would be relevant to a SOC analyst because:
- Open services increase attack surface
- Authentication attempts should be reviewed for legitimacy
- Repeated failed logins can indicate unauthorized access attempts
- SIEM visibility helps correlate user activity and endpoint events

## Outcome
The project successfully demonstrated a basic detection and investigation workflow using Kali Linux, Nmap, SSH, and Wazuh.
