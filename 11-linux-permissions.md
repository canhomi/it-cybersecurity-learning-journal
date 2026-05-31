# 11 - Linux Permissions

## Objective

Document basic Linux permissions concepts used in IT Support, Linux administration and cybersecurity.

## Why Linux Permissions Matter

Linux permissions control who can read, write or execute files and directories.

Understanding permissions is important because wrong permissions can cause:

- Access problems
- Application errors
- Security weaknesses
- Unauthorized access
- Service failures
- Troubleshooting issues

## Basic Permission Types

Linux uses three basic permission types:

```text
r = read
w = write
x = execute
```

## Permission Groups

Linux permissions are applied to three groups:

```text
user  = file owner
group = group associated with the file
other = everyone else
```

## Example Permission Output

When running:

```bash
ls -l
```

Example result:

```text
-rw-r--r-- 1 user user 1024 May 31 notes.txt
```

This means:

```text
-          regular file
rw-        owner can read and write
r--        group can read
r--        others can read
```

## Common Commands

### List Files With Permissions

```bash
ls -l
```

### Change File Permissions

```bash
chmod 644 file.txt
```

### Add Execute Permission

```bash
chmod +x script.sh
```

### Change File Owner

```bash
sudo chown user:user file.txt
```

### Check Current User

```bash
whoami
```

### Check User Groups

```bash
groups
```

## Numeric Permissions

Linux permissions can be represented by numbers:

```text
4 = read
2 = write
1 = execute
```

Examples:

```text
7 = read + write + execute
6 = read + write
5 = read + execute
4 = read only
```

Common permission examples:

```text
644 = owner can read/write, group and others can read
755 = owner can read/write/execute, group and others can read/execute
600 = only owner can read/write
700 = only owner can read/write/execute
```

## Common Examples

### Normal Text File

```bash
chmod 644 notes.txt
```

### Script File

```bash
chmod +x script.sh
```

### Private File

```bash
chmod 600 private.txt
```

### Private Directory

```bash
chmod 700 private-folder
```

## What I Learned

- How Linux permissions are structured
- Difference between read, write and execute
- Difference between user, group and other
- How to view permissions with `ls -l`
- How to change permissions with `chmod`
- How to change ownership with `chown`
- Why permissions are important for security

## Real-World Use

Linux permissions are used in:

- Server administration
- Web server configuration
- User access management
- Application troubleshooting
- Cloud systems
- Cybersecurity investigations
- Hardening
- Incident response

## Common Troubleshooting Scenarios

### Permission Denied

Possible checks:

```bash
whoami
ls -l
groups
```

### Script Does Not Run

Possible fix:

```bash
chmod +x script.sh
```

### User Cannot Access File

Possible checks:

```bash
ls -l file.txt
groups username
```

### Wrong Owner

Possible fix:

```bash
sudo chown user:user file.txt
```

## Common Mistakes

- Using `chmod 777` without understanding the risk
- Giving execute permission to files that do not need it
- Changing ownership of system files without reason
- Running everything with `sudo`
- Not checking file owner before troubleshooting
- Confusing file permissions and directory permissions

## Security Notes

The command below is risky and should not be used casually:

```bash
chmod 777 file-or-folder
```

It gives read, write and execute permissions to everyone.

In professional environments, permissions should follow the principle of least privilege.

## Cybersecurity Perspective

Weak permissions can allow attackers or unauthorized users to:

- Read sensitive files
- Modify scripts
- Execute malicious files
- Access private data
- Change application behavior
- Escalate privileges in some situations

Permission review is part of basic Linux hardening.

## Professional Importance

Linux permissions are essential for IT and cybersecurity.

Priority level:

```text
Essential for Linux
Important for employability
Mandatory for server administration
Important for security hardening
```

## Next Step

Study Linux services, processes and system monitoring commands.