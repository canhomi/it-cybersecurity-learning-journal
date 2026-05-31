# 10 - Terminal Good Practices

## Objective

Document basic terminal good practices for Linux, macOS and cybersecurity labs.

## Why Terminal Skills Matter

The terminal is one of the most important tools in IT, Linux administration, cloud, networking and cybersecurity.

Many professional tasks are faster and more precise through the command line.

## Where Terminal Is Used

Terminal knowledge is useful in:

- Linux administration
- macOS administration
- Cloud environments
- Server management
- Networking troubleshooting
- Cybersecurity labs
- SOC investigations
- Log analysis
- Automation
- Scripting

## Basic Commands Practiced

```bash
pwd
ls
cd
clear
whoami
hostname
uname -a
ip a
ping 8.8.8.8
exit
```

## Important Command: exit

The command `exit` is used to close a terminal session properly.

Example:

```bash
exit
```

## When to Use exit

Use `exit` when:

- You finished working in the terminal
- You are connected to a remote server through SSH
- You want to close a shell session
- You want to leave a user session
- You want to avoid leaving sessions open unnecessarily

## Difference Between clear and exit

### clear

The command `clear` only cleans the terminal screen.

```bash
clear
```

It does not close the terminal session.

### exit

The command `exit` closes the current shell session.

```bash
exit
```

## Using sudo Carefully

The command `sudo` runs commands with administrator privileges.

Example:

```bash
sudo apt update
```

## Good sudo Practices

Before using `sudo`, always ask:

- Do I understand what this command does?
- Can this command change the system?
- Can this command delete files?
- Is this command from a trusted source?
- Am I in the correct machine or virtual machine?

## Dangerous Command Awareness

Some commands can damage a system if used incorrectly.

Examples of risky actions:

```text
Deleting system files
Changing permissions recursively
Disabling security services
Running unknown scripts
Executing commands copied from the internet without understanding
```

## Working in Labs

In a lab environment, it is important to:

- Use virtual machines
- Take snapshots before major changes
- Document commands used
- Keep personal data separate
- Avoid testing against real systems
- Use only legal and authorized environments

## Good Documentation Habits

When practicing commands, document:

- What command was used
- Why it was used
- What result was expected
- What result happened
- Any error message
- How the problem was solved

## Example Documentation

```text
Command:
ping 8.8.8.8

Purpose:
Test internet connectivity.

Result:
The machine received replies, confirming network connectivity.

Conclusion:
Internet access is working.
```

## Common Mistakes

- Closing the terminal window without understanding the session
- Forgetting to use `exit` when connected to remote systems
- Running commands without reading them
- Using `sudo` too often
- Copying commands from the internet without understanding
- Not documenting errors
- Not checking the current directory before running commands

## Cybersecurity Perspective

Terminal discipline is important in cybersecurity.

A small mistake can:

- Change the wrong system
- Delete important files
- Stop a service
- Expose sensitive data
- Create false lab results
- Damage an investigation

Professional analysts document their actions and understand the impact of each command.

## Professional Importance

Terminal knowledge is essential for IT and cybersecurity.

Priority level:

```text
Essential for starting
Important for employability
Mandatory for Linux and cloud
Very useful for SOC and troubleshooting
```

## Next Step

Practice file management, permissions and service management commands in Linux.