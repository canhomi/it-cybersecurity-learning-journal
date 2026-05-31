# 03 - Ubuntu Server Lab

## Objective

Document the installation and first configuration steps of an Ubuntu Server virtual machine for IT Support, Linux administration and cybersecurity practice.

## Environment

- Host machine: macOS
- Virtualization platform: VirtualBox
- Guest system: Ubuntu Server
- Purpose: Build a basic Linux server lab for administration and security training

## What is Ubuntu Server?

Ubuntu Server is a Linux operating system commonly used to run servers, applications, services, cloud workloads and cybersecurity labs.

Unlike a regular desktop system, Ubuntu Server usually runs without a graphical interface and is managed mainly through the command line.

## Why This Matters

Ubuntu Server is important for IT and cybersecurity because many companies use Linux servers for:

- Web servers
- Application servers
- Databases
- Cloud systems
- Security tools
- Log collection
- Monitoring platforms
- SOC and SIEM labs

## Basic Concepts Learned

- Server operating system
- Command-line administration
- System updates
- User management
- Network verification
- Service management
- Safe lab environment

## Commands Practiced

```bash
whoami
pwd
ls
ip a
ping 8.8.8.8
sudo apt update
sudo apt upgrade
sudo reboot
sudo shutdown now
```

## Useful System Commands

```bash
hostname
uname -a
df -h
free -h
top
systemctl status
```

## What I Learned

- How to start using an Ubuntu Server system
- How to check the current user
- How to verify the server IP address
- How to test internet connectivity
- How to update the system
- How to reboot and shut down a Linux server
- Why servers are usually managed through the terminal

## Real-World Use

Ubuntu Server knowledge is useful for:

- IT Support
- Junior System Administration
- Cloud Support
- SOC Analyst roles
- Cybersecurity labs
- SIEM and log monitoring environments

## Common Mistakes

- Forgetting to update the system after installation
- Not knowing the server IP address
- Confusing reboot and shutdown commands
- Running commands with sudo without understanding them
- Not documenting configuration changes
- Not taking snapshots before important changes

## Security Notes

This lab is used only for legal, ethical and defensive learning.

All tests are performed in a private and controlled virtual environment.

## Next Step

Document Kali Linux usage and basic networking commands.