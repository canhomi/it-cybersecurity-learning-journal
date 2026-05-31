# 13 - Basic Troubleshooting

## Objective

Document a basic troubleshooting methodology for IT Support, system administration and cybersecurity labs.

## What is Troubleshooting?

Troubleshooting is the process of identifying, analyzing and solving technical problems in a structured way.

In IT, troubleshooting is used when something is not working as expected, such as:

- No internet connection
- Slow computer
- Login problems
- Application errors
- Server not responding
- Service stopped
- Printer issues
- VPN problems
- Security alerts
- System performance issues

## Why Troubleshooting Matters

Troubleshooting is one of the most important skills for IT professionals.

A good technician does not only try random solutions.

A good technician follows a process, collects evidence, tests possibilities and documents the result.

## Basic Troubleshooting Method

1. Identify the problem
2. Gather information
3. Ask what changed
4. Check basic symptoms
5. Test the most likely causes
6. Apply a solution
7. Verify the result
8. Document what was done

## Step 1 - Identify the Problem

Ask:

```text
What exactly is not working?
When did it start?
Does it affect one user or many users?
Is the problem constant or intermittent?
Was anything changed recently?
```

## Step 2 - Gather Information

Useful information includes:

```text
Device name
Operating system
Username
IP address
Error message
Time of the issue
Application involved
Network used
Recent updates or changes
```

## Step 3 - Check Basic Connectivity

### Linux / macOS

```bash
ip a
ifconfig
ping 8.8.8.8
ping google.com
nslookup google.com
traceroute google.com
```

### Windows

```cmd
ipconfig
ping 8.8.8.8
ping google.com
nslookup google.com
tracert google.com
```

## Step 4 - Check System Resources

### Linux

```bash
top
free -h
df -h
ps aux
```

### Windows

```text
Task Manager
Disk usage
Memory usage
CPU usage
Startup Apps
```

## Step 5 - Check Services

### Linux

```bash
systemctl status service-name
sudo systemctl restart service-name
```

### Windows

```text
Services
Task Manager
Event Viewer
Windows Security
```

## Step 6 - Check Logs

Logs help identify what happened.

Common log sources:

```text
Windows Event Viewer
Linux system logs
Application logs
Security tool alerts
Wazuh alerts
Firewall logs
Authentication logs
```

## Common Scenario: No Internet

Possible checks:

```text
Is Wi-Fi or cable connected?
Does the device have an IP address?
Can it ping 8.8.8.8?
Can it resolve DNS?
Is VPN enabled?
Is the gateway reachable?
Is the firewall blocking traffic?
```

Useful commands:

```bash
ping 8.8.8.8
ping google.com
nslookup google.com
```

## Common Scenario: DNS Problem

Symptom:

```text
Ping to 8.8.8.8 works, but websites do not open.
```

Possible cause:

```text
DNS resolution problem
```

Useful command:

```bash
nslookup google.com
```

## Common Scenario: Slow Computer

Possible checks:

```text
CPU usage
Memory usage
Disk usage
Startup applications
Background processes
Updates running
Malware or unwanted software
Low disk space
```

## Common Scenario: Login Problem

Possible checks:

```text
Correct username
Correct password
Account locked
MFA issue
Network connection
Domain connection
Conditional Access policy
Expired password
```

## Common Scenario: Service Not Working

Possible checks:

```text
Is the service running?
Was it recently updated?
Are logs showing errors?
Is the port open?
Is there enough disk space?
Was configuration changed?
```

Useful Linux command:

```bash
systemctl status service-name
```

## What I Learned

- Troubleshooting must follow a structured process
- It is important to collect information before changing settings
- Basic network tests are essential
- Logs are important for understanding problems
- Documentation helps avoid repeating mistakes
- Many problems can be solved by checking simple causes first

## Real-World Use

Troubleshooting is used in:

- IT Support
- Help Desk
- Service Desk
- System Administration
- Cloud Support
- SOC Analysis
- Incident Response
- Endpoint Security
- Network Support

## Common Mistakes

- Trying random solutions without understanding the problem
- Not asking what changed recently
- Ignoring error messages
- Not checking basic connectivity
- Not checking logs
- Not documenting the solution
- Restarting systems without investigation
- Assuming the user is wrong without verifying

## Cybersecurity Perspective

Troubleshooting is also important in cybersecurity.

Security analysts need to determine whether an issue is:

```text
Normal system behavior
User error
Misconfiguration
Technical failure
Suspicious activity
Confirmed security incident
```

## Professional Importance

Troubleshooting is essential for employability in IT.

Priority level:

```text
Essential for IT Support
Important for Help Desk
Mandatory for system administration
Very useful for SOC Analyst Level 1
```

## Next Step

Document the main skills required for entry-level IT Support roles.