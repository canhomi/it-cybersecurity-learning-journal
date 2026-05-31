# 02 - VirtualBox Lab

## Objective

Document the creation and use of virtual machines for IT Support, Linux, Windows and Cybersecurity practice.

## Environment

- Host machine: macOS
- Virtualization platform: VirtualBox
- Guest systems:
  - Kali Linux
  - Ubuntu Server
  - Windows Lab VM

## What is VirtualBox?

VirtualBox is a virtualization tool that allows me to run different operating systems inside my main computer.

This is useful because I can create safe labs without changing or damaging my main system.

## Why This Matters

Virtual machines are used in IT and cybersecurity to:

- Practice operating system installation
- Test Linux, Windows and server environments
- Build cybersecurity labs
- Simulate networks
- Analyze logs and security events
- Practice troubleshooting safely

## Basic Concepts Learned

- Host machine: the real physical computer
- Guest machine: the virtual machine running inside VirtualBox
- ISO file: installation image used to install an operating system
- Snapshot: saved state of a virtual machine
- Network adapter: controls how the VM connects to the network
- Shared folder: allows file sharing between host and guest

## Practical Steps

1. Install VirtualBox
2. Download an operating system ISO
3. Create a new virtual machine
4. Assign CPU, RAM and disk space
5. Attach the ISO file
6. Start the VM
7. Install the operating system
8. Update the system
9. Test internet connection
10. Take a snapshot after setup

## Useful Commands Inside Linux VMs

```bash
whoami
pwd
ls
ip a
ping 8.8.8.8
sudo apt update
sudo apt upgrade
```

## Common Mistakes

- Allocating too little RAM
- Forgetting to attach the ISO file
- Using the wrong network mode
- Not taking snapshots
- Installing tools without understanding their purpose
- Mixing personal files with lab files

## Real-World Use

Virtualization is used by:

- IT Support Technicians
- System Administrators
- SOC Analysts
- Cloud Engineers
- Cybersecurity Analysts
- Malware analysts in isolated environments

## Security Notes

All cybersecurity tests must be done only in legal, controlled and authorized lab environments.

Virtual machines should not be used to attack third-party systems.

## What I Learned

- How virtual machines work
- Why labs are important for technical training
- How to separate my learning environment from my main computer
- How to prepare systems for IT and security practice

## Next Step

Create separate documentation for Ubuntu Server, Kali Linux and Windows Lab.