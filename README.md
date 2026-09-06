# Wazuh Windows Security Monitoring Lab

## 📌 Project Overview

This project demonstrates a hands-on SOC monitoring lab using **Wazuh** to monitor and analyze security events from a Windows endpoint.

The lab focuses on Windows security log collection, failed authentication detection, and security alert investigation.

## 🎯 Objectives

* Set up a Wazuh security monitoring environment
* Connect a Windows endpoint using the Wazuh Agent
* Collect Windows security events
* Detect failed authentication attempts
* Investigate Wazuh security alerts
* Understand the basic SOC alert investigation workflow

## 🛠️ Technologies Used

* Wazuh
* Wazuh Agent
* Windows
* Linux
* Windows Event Logs
* SIEM
* SOC Monitoring

## 🏗️ Lab Architecture

```text
Windows Endpoint
      |
      | Wazuh Agent
      ↓
Wazuh Manager
      |
      ↓
Wazuh Dashboard
      |
      ↓
Security Alerts
      |
      ↓
SOC Investigation
```

## 🔬 Lab 1 — Failed Login Detection

### Objective

Detect and investigate failed Windows authentication attempts using Wazuh.

### Procedure

1. Installed and configured Wazuh.
2. Installed the Wazuh Agent on Windows.
3. Connected the Windows Agent to the Wazuh server.
4. Verified that the agent was active.
5. Generated failed login attempts on the Windows endpoint.
6. Monitored the generated security events in Wazuh.
7. Investigated the resulting alerts.

### Windows Event ID

**4625 — Failed Logon**

The event was analyzed using:

* Username
* Timestamp
* Event ID
* Source information
* Logon Type
* Wazuh Rule
* Alert severity

## 📊 Result

Wazuh successfully collected Windows security events and generated alerts for failed authentication activity.

This demonstrated a basic SOC workflow:

```text
Endpoint Activity
       ↓
Log Collection
       ↓
Detection
       ↓
Alert
       ↓
Investigation
       ↓
Analysis
```

## 📸 Screenshots

Screenshots of the Wazuh dashboard, active Windows agent, and generated security alerts are available in the `screenshots` directory.

## 🚀 Future Improvements

* Add Sysmon monitoring
* Monitor PowerShell activity
* Configure File Integrity Monitoring
* Create custom Wazuh detection rules
* Map detections to MITRE ATT&CK
* Monitor Windows Defender events
* Implement Active Response
* Add additional attack-detection scenarios

## 📚 Skills Demonstrated

**Wazuh | SIEM | Windows Event Logs | SOC Monitoring | Alert Investigation | Endpoint Monitoring | Security Event Analysis | Incident Detection**
