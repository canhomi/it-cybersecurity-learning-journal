# 06 - Wazuh SOC Lab

## Objective

Document my first SOC lab using Wazuh to understand security monitoring, agents, logs, alerts and basic defensive cybersecurity workflows.

## Environment

- Host machine: macOS
- Virtualization platform: VirtualBox
- Lab systems:
  - Ubuntu Server
  - Kali Linux
  - macOS
  - Windows Lab VM
- Security platform: Wazuh
- Purpose: Learn basic SOC monitoring and endpoint visibility

## What is Wazuh?

Wazuh is an open-source security monitoring platform used for threat detection, log analysis, file integrity monitoring, vulnerability detection and endpoint security visibility.

It can collect data from agents installed on different systems and show security events in a centralized dashboard.

## Why This Matters

Wazuh is useful for cybersecurity because it helps analysts understand:

- Endpoint activity
- Security alerts
- System logs
- Authentication events
- Configuration issues
- Vulnerabilities
- Suspicious behavior
- Basic incident investigation

## SOC Concept

SOC means Security Operations Center.

A SOC is responsible for monitoring systems, detecting suspicious activity, investigating alerts and helping respond to security incidents.

A SOC Analyst Level 1 usually works with:

- Alerts
- Logs
- SIEM tools
- Endpoint security tools
- Ticketing systems
- Basic investigation
- Escalation to senior analysts

## Basic Concepts Learned

- Security monitoring
- Wazuh server
- Wazuh agent
- Endpoint visibility
- Log collection
- Alerts
- Dashboard
- Basic SOC workflow
- Defensive cybersecurity mindset

## Wazuh Agent Concept

The Wazuh agent is installed on an endpoint, such as Linux, Windows or macOS.

The agent collects security-relevant information and sends it to the Wazuh server for analysis.

## Commands Practiced

### Check Wazuh Agent Status

```bash
sudo systemctl status wazuh-agent
```

### Start Wazuh Agent

```bash
sudo systemctl start wazuh-agent
```

### Stop Wazuh Agent

```bash
sudo systemctl stop wazuh-agent
```

### Disable Wazuh Agent

```bash
sudo systemctl disable wazuh-agent
```

### Restart Wazuh Agent

```bash
sudo systemctl restart wazuh-agent
```

## What I Learned

- What a SOC is
- What Wazuh is used for
- What a Wazuh agent does
- How endpoints can send logs to a central platform
- How security tools help monitor systems
- Why logs are important for cybersecurity
- How to check if an agent is running
- How to stop, start and manage a security agent

## Real-World Use

Wazuh and similar tools are used in:

- SOC environments
- Security monitoring
- Endpoint security
- Compliance monitoring
- Vulnerability management
- Incident investigation
- Log analysis
- Threat detection

## Common Mistakes

- Installing an agent without understanding what it collects
- Not checking if the agent is connected
- Ignoring logs and alerts
- Confusing endpoint protection with security monitoring
- Not documenting installation steps
- Not understanding the difference between server and agent
- Installing security tools on a personal system without a clear lab purpose

## Security Notes

All tests in this lab are performed only in controlled and authorized environments.

The purpose of this lab is defensive cybersecurity learning, monitoring and analysis.

## First SOC Analysis Workflow

A basic SOC investigation can follow this structure:

1. Identify the alert
2. Check the affected endpoint
3. Review the timestamp
4. Understand what triggered the alert
5. Check related logs
6. Determine if the activity is expected or suspicious
7. Document findings
8. Escalate if needed

## Example Questions for an Analyst

When reviewing an alert, ask:

- Which system generated the alert?
- What user was involved?
- What time did it happen?
- What process or service was involved?
- Is this normal activity?
- Is there any sign of compromise?
- What evidence supports the conclusion?

## Defensive Cybersecurity Perspective

The goal is not just to install tools.

The goal is to understand what the tool is showing, why the alert happened and how to investigate it professionally.

## Professional Importance

Wazuh is useful for building SOC and Blue Team knowledge.

Priority level:

```text
Important for employability
Very useful for SOC Analyst Level 1
Good practical portfolio project
```

## Next Step

Document the first basic SOC analysis workflow and create a simple alert investigation template.