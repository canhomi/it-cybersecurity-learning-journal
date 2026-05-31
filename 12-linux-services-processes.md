# 12 - Linux Services and Processes

## Objective

Document basic Linux services and processes concepts used in IT Support, system administration and cybersecurity.

## Why Services and Processes Matter

Linux systems run many background tasks.

Understanding services and processes helps with:

- Troubleshooting
- Server administration
- Security monitoring
- Performance analysis
- Application support
- Incident investigation

## Basic Concepts

### Process

A process is a running program.

Examples:

```text
Terminal session
Web browser
Security agent
System task
Application service
```

### Service

A service is a background program usually managed by the operating system.

Examples:

```text
SSH service
Web server
Database service
Wazuh agent
Logging service
```

### Daemon

A daemon is a background process that runs without direct user interaction.

Many Linux services are daemons.

## Useful Commands

### Show Running Processes

```bash
ps aux
```

### Monitor Processes in Real Time

```bash
top
```

### Show System Resource Usage

```bash
free -h
df -h
```

### Check a Service Status

```bash
systemctl status service-name
```

Example:

```bash
systemctl status ssh
```

### Start a Service

```bash
sudo systemctl start service-name
```

### Stop a Service

```bash
sudo systemctl stop service-name
```

### Restart a Service

```bash
sudo systemctl restart service-name
```

### Enable a Service at Boot

```bash
sudo systemctl enable service-name
```

### Disable a Service at Boot

```bash
sudo systemctl disable service-name
```

## Example With Wazuh Agent

```bash
sudo systemctl status wazuh-agent
sudo systemctl stop wazuh-agent
sudo systemctl start wazuh-agent
sudo systemctl restart wazuh-agent
sudo systemctl disable wazuh-agent
```

## What I Learned

- What a process is
- What a service is
- How to check running processes
- How to monitor system activity
- How to check service status
- How to start, stop and restart services
- How services are important for security tools like Wazuh

## Real-World Use

Services and processes are used in:

- Linux administration
- Server troubleshooting
- SOC investigations
- Security monitoring
- Cloud support
- Application support
- Incident response

## Common Troubleshooting Scenarios

### Service Not Running

Useful command:

```bash
systemctl status service-name
```

Possible action:

```bash
sudo systemctl restart service-name
```

### Server Is Slow

Useful commands:

```bash
top
free -h
df -h
```

### Disk Is Full

Useful command:

```bash
df -h
```

### High Memory Usage

Useful command:

```bash
free -h
top
```

### Unknown Process

Useful command:

```bash
ps aux
```

## Common Mistakes

- Restarting services without checking logs
- Killing processes without understanding their purpose
- Disabling important services
- Ignoring disk space
- Ignoring memory usage
- Not documenting what was changed
- Using sudo without understanding the command

## Cybersecurity Perspective

Processes and services are important for security investigations.

SOC analysts may need to check:

- Suspicious processes
- Unexpected services
- Security agents running or stopped
- Persistence mechanisms
- Unusual resource usage
- Failed services
- Log collection problems

## Professional Importance

Understanding services and processes is essential for Linux, servers and cybersecurity.

Priority level:

```text
Essential for Linux
Important for troubleshooting
Important for SOC analysis
Mandatory for system administration
```

## Next Step

Create a basic troubleshooting documentation file for IT Support and cybersecurity labs.