## Evidence and Screenshots

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
