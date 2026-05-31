# 08 - First SOC Analysis

## Objective

Document a basic SOC alert investigation workflow for beginner-level defensive cybersecurity practice.

## Environment

- Lab systems:
  - Wazuh
  - Ubuntu Server
  - Kali Linux
  - Windows Lab VM
  - macOS
- Purpose: Learn how to investigate security alerts in a structured and professional way

## What is SOC Analysis?

SOC analysis is the process of reviewing security alerts, logs and events to determine whether an activity is normal, suspicious or malicious.

A SOC Analyst Level 1 usually performs the first review of alerts and escalates cases when needed.

## Why This Matters

Security tools generate many alerts.

The analyst needs to understand:

- What happened
- When it happened
- Which system was affected
- Which user was involved
- Whether the activity is expected or suspicious
- What evidence supports the conclusion
- Whether escalation is necessary

## Basic SOC Workflow

A basic investigation can follow this structure:

1. Identify the alert
2. Check the affected host
3. Check the user involved
4. Review the timestamp
5. Understand the event type
6. Search for related logs
7. Compare with normal behavior
8. Classify the event
9. Document the findings
10. Escalate if necessary

## Alert Investigation Template

### Alert Name

```text
Example: Failed login attempt
```

### Date and Time

```text
YYYY-MM-DD HH:MM
```

### Affected System

```text
Hostname or IP address
```

### User Involved

```text
Username or account involved
```

### Source IP

```text
Internal or external IP address
```

### Event Description

```text
Short explanation of what happened
```

### Evidence Reviewed

```text
Logs, alerts, timestamps, process names, IP addresses or commands reviewed
```

### Initial Classification

```text
Benign / Suspicious / Malicious / Needs escalation
```

### Analyst Notes

```text
Personal observations and reasoning
```

### Recommended Action

```text
Monitor / Investigate more / Escalate / Block / Reset password / Isolate endpoint
```

## Example Investigation

### Alert Name

```text
Multiple failed login attempts
```

### Date and Time

```text
2026-05-31 14:20
```

### Affected System

```text
Windows Lab VM
```

### User Involved

```text
test-user
```

### Source IP

```text
192.168.1.50
```

### Event Description

```text
Several failed login attempts were detected for the same user account.
```

### Evidence Reviewed

```text
Authentication logs
Security event timestamp
Source IP address
Affected username
Number of failed attempts
```

### Initial Classification

```text
Suspicious
```

### Analyst Notes

```text
The activity may indicate a wrong password, user mistake or possible brute-force attempt.
More context is needed before confirming malicious activity.
```

### Recommended Action

```text
Check whether the user was trying to log in.
Review additional authentication logs.
Monitor for repeated attempts.
Escalate if attempts continue or come from an unknown source.
```

## Useful Questions During Analysis

- What triggered the alert?
- Which system generated the alert?
- Which user was involved?
- What time did it happen?
- Is the source IP internal or external?
- Is this normal behavior for this user or system?
- Are there similar events before or after?
- Is there evidence of compromise?
- Does this need escalation?

## Common Mistakes

- Closing alerts too quickly
- Assuming every alert is malicious
- Assuming every alert is harmless
- Not checking timestamps
- Not checking the affected system
- Not documenting evidence
- Not escalating when needed
- Not understanding the difference between alert and incident

## Alert vs Incident

An alert is a notification that something may need attention.

An incident is a confirmed or strongly suspected security event that may affect confidentiality, integrity or availability.

Not every alert is an incident.

## Real-World Use

This workflow is useful for:

- SOC Analyst Level 1
- Blue Team practice
- SIEM alert triage
- Endpoint security monitoring
- Incident response preparation
- Security documentation

## Professional Importance

SOC analysis documentation is very important for entry-level cybersecurity roles.

Priority level:

```text
Important for employability
Essential for SOC learning
Useful for interviews
Good portfolio evidence
```

## Next Step

Practice with real lab alerts, screenshots and structured incident notes.