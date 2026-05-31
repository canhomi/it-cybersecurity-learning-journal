# 07 - Windows Lab

## Objective

Document the creation and basic use of a Windows virtual machine for IT Support, system administration and cybersecurity practice.

## Environment

- Host machine: macOS
- Virtualization platform: VirtualBox
- Guest system: Windows
- Purpose: Build a Windows lab for support, troubleshooting, administration and security learning

## Why Windows Matters

Windows is one of the most used operating systems in companies.

For IT Support and Cybersecurity, Windows knowledge is essential because many business environments use:

- Windows workstations
- Windows Server
- Active Directory
- Microsoft 365
- Entra ID
- Intune
- Microsoft Defender
- Group Policy
- PowerShell
- Event Viewer

## Basic Concepts Learned

- Windows installation in a virtual machine
- User account setup
- System settings
- Network configuration
- Windows updates
- Basic troubleshooting
- Security settings
- Event logs

## Important Windows Tools

### Settings

Used to configure system options, network, accounts, updates and privacy.

### Control Panel

Traditional Windows configuration area still used for many administrative tasks.

### Device Manager

Used to check hardware, drivers and device problems.

### Task Manager

Used to check running processes, CPU, memory, disk and startup applications.

### Event Viewer

Used to view Windows logs and investigate system, application and security events.

### Windows Security

Used to check antivirus, firewall, device security and protection status.

### PowerShell

Command-line and scripting tool used for administration and automation.

## Basic Commands Practiced

### Command Prompt

```cmd
hostname
whoami
ipconfig
ping 8.8.8.8
ping google.com
tracert google.com
nslookup google.com
netstat -ano
```

### PowerShell

```powershell
Get-ComputerInfo
Get-Process
Get-Service
Get-NetIPAddress
Get-NetAdapter
Test-Connection google.com
Get-EventLog -LogName System -Newest 10
```

## What I Learned

- How to create a Windows virtual machine
- How to check basic system information
- How to verify network configuration
- How to test internet connectivity
- How to use basic troubleshooting commands
- How Windows logs can help in investigations
- Why Windows knowledge is important for IT and cybersecurity jobs

## Real-World Use

Windows knowledge is used in:

- IT Support
- Help Desk
- Service Desk
- Junior System Administration
- Microsoft 365 Administration
- Endpoint Security
- SOC Analysis
- Incident Response
- Identity and Access Management

## Common Troubleshooting Scenarios

### No internet connection

Useful commands:

```cmd
ipconfig
ping 8.8.8.8
ping google.com
nslookup google.com
```

### Slow computer

Useful tools:

```text
Task Manager
Startup Apps
Installed Programs
Windows Update
Disk usage check
```

### Login problem

Possible checks:

```text
User account status
Password issue
Network connectivity
Domain connection
Account lockout
MFA or Conditional Access issue
```

### Suspicious activity

Useful tools:

```text
Event Viewer
Task Manager
Windows Security
Installed Programs
Startup Apps
Network connections
```

## Cybersecurity Perspective

Windows is a major target in cybersecurity.

A SOC analyst must understand Windows events, authentication logs, processes, services and endpoint security alerts.

Important areas for future study:

- Event Viewer
- Windows Security logs
- PowerShell logs
- Defender alerts
- Failed login attempts
- Suspicious processes
- Persistence mechanisms
- User and group changes

## Common Mistakes

- Ignoring Event Viewer
- Not checking Windows Update
- Confusing Command Prompt and PowerShell
- Not documenting errors
- Running commands without administrator rights when needed
- Not understanding user permissions
- Disabling security features without a reason

## Professional Importance

Windows knowledge is essential for employability.

Priority level:

```text
Essential for starting
Very important for IT Support
Mandatory for Microsoft administration
Important for SOC Analyst Level 1
```

## Next Step

Create a first SOC analysis template to document alerts, logs, affected systems and investigation results.