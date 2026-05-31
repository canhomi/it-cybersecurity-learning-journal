# 05 - Networking Basics

## Objective

Document basic networking concepts and commands used in IT Support, system administration and cybersecurity investigations.

## Environment

- Host machine: macOS
- Lab systems:
  - Kali Linux
  - Ubuntu Server
  - Windows Lab VM
- Purpose: Practice basic network troubleshooting and understand how devices communicate

## Why Networking Matters

Networking is one of the most important foundations in IT and cybersecurity.

Without understanding IP addresses, DNS, gateways, ports and protocols, it is difficult to troubleshoot systems, analyze logs, understand alerts or investigate security incidents.

## Basic Concepts Learned

### IP Address

An IP address identifies a device on a network.

Example:

```text
192.168.1.10
```

### Gateway

The gateway is the device that connects the local network to other networks, usually the internet.

### DNS

DNS translates domain names into IP addresses.

Example:

```text
google.com -> IP address
```

### DHCP

DHCP automatically gives IP addresses to devices on a network.

### TCP and UDP

TCP and UDP are transport protocols used for communication between systems.

- TCP is connection-oriented and reliable
- UDP is faster but does not guarantee delivery

### Ports

Ports identify specific services running on a system.

Examples:

```text
80   HTTP
443  HTTPS
22   SSH
53   DNS
3389 RDP
```

## Commands Practiced

### Linux / macOS

```bash
ip a
ifconfig
ping 8.8.8.8
ping google.com
traceroute google.com
nslookup google.com
netstat -tulnp
curl https://example.com
```

### Windows

```powershell
ipconfig
ping 8.8.8.8
ping google.com
tracert google.com
nslookup google.com
netstat -ano
```

## What I Learned

- How to check the IP address of a machine
- How to test internet connectivity
- How to test DNS resolution
- How to identify basic network routes
- How to check active connections
- Why networking is essential for cybersecurity
- How network problems appear in real troubleshooting scenarios

## Real-World Use

Networking knowledge is used in:

- IT Support
- Help Desk
- Service Desk
- System Administration
- Cloud Support
- SOC Analysis
- Incident Response
- Firewall troubleshooting
- VPN troubleshooting
- Endpoint security investigations

## Common Troubleshooting Scenarios

### No internet connection

Possible checks:

```bash
ip a
ping 8.8.8.8
ping google.com
```

If ping to `8.8.8.8` works but `google.com` does not, the problem may be DNS.

### DNS problem

Useful command:

```bash
nslookup google.com
```

### Route problem

Useful command:

```bash
traceroute google.com
```

On Windows:

```powershell
tracert google.com
```

### Open connections

Linux:

```bash
netstat -tulnp
```

Windows:

```powershell
netstat -ano
```

## Common Mistakes

- Trying advanced cybersecurity tools without understanding networking
- Confusing IP address and DNS name
- Not checking the gateway
- Not testing DNS separately
- Forgetting that Windows and Linux use different command syntax
- Ignoring firewall or VPN impact
- Not documenting troubleshooting steps

## Cybersecurity Perspective

Networking is essential for security monitoring.

SOC analysts need networking knowledge to understand:

- Suspicious connections
- External IP addresses
- DNS requests
- Open ports
- Firewall logs
- VPN logs
- Lateral movement
- Command and control traffic indicators

## Professional Importance

Networking is essential for employability in IT and cybersecurity.

Priority level:

```text
Essential for starting
Important for employability
Mandatory before advanced cybersecurity
```

## Next Step

Practice basic Windows networking commands and document the Windows Lab.