# 🐧 Linux Command Map for SOC Analysts

> **Your first-response building blocks.**
>
> Essential Linux commands for system navigation, process investigation, log analysis, user identification, network monitoring, and basic security investigation.

## 📌 Table of Contents

- [1. File & Directory Commands](#1-file--directory-commands)
- [2. Process Commands](#2-process-commands)
- [3. Log Analysis Commands](#3-log-analysis-commands)
- [4. Permission Commands](#4-permission-commands)
- [5. Identity Commands](#5-identity-commands)
- [6. Network Commands](#6-network-commands)
- [7. Persistence Commands](#7-persistence-commands)
- [8. Text Processing Commands](#8-text-processing-commands)

## 1. File & Directory Commands

| Command | Purpose |
|---|---|
| `pwd` | Display current directory |
| `ls -la` | List all files, including hidden files |
| `cd` | Change directory |
| `cat` | Display file contents |
| `less` | Read files interactively |
| `find` | Search files and directories |
| `file` | Identify file type |
| `stat` | View file metadata |
| `head` | Display first lines |
| `tail` | Display last lines |

## 2. Process Commands

| Command | Purpose |
|---|---|
| `ps aux` | List running processes |
| `top` | Monitor processes in real time |
| `pgrep -a` | Search processes by name |
| `pstree -p` | View process relationships |
| `pidof` | Find process ID |
| `kill` | Send a signal to a process |

## 3. Log Analysis Commands

| Command | Purpose |
|---|---|
| `tail -f` | Monitor logs continuously |
| `grep` | Search log entries |
| `journalctl` | View systemd journal logs |
| `journalctl -u` | View service-specific logs |
| `dmesg -T` | View kernel messages |
| `zgrep` | Search compressed logs |
| `wc -l` | Count log lines |

**Example:**

```bash
grep -i "failed" /var/log/auth.log
sudo journalctl -u ssh
tail -f /var/log/syslog
```

## 4. Permission Commands

| Command | Purpose |
|---|---|
| `ls -l` | View file permissions |
| `chmod` | Change permissions |
| `chown` | Change ownership |
| `getfacl` | View access control lists |
| `sudo -l` | Check sudo privileges |

## 5. Identity Commands

| Command | Purpose |
|---|---|
| `whoami` | Display current username |
| `id` | Display user and group IDs |
| `who` | Show logged-in users |
| `w` | Show user activity |
| `last` | Review login history |
| `groups` | Display user groups |
| `getent passwd` | Query user accounts |

## 6. Network Commands

| Command | Purpose |
|---|---|
| `ip addr` | Display IP addresses |
| `ip route` | View routing table |
| `ss -tulnp` | Identify listening ports |
| `ss -antp` | View TCP connections |
| `ping` | Test network connectivity |
| `dig` | Perform DNS queries |
| `curl` | Send HTTP requests |
| `tcpdump` | Capture network packets |

## 7. Persistence Commands

| Command | Purpose |
|---|---|
| `crontab -l` | List scheduled jobs |
| `systemctl status` | Check service status |
| `systemctl is-enabled` | Check service startup configuration |
| `systemctl list-timers` | List systemd timers |
| `systemctl list-unit-files` | Review service configurations |
| `ls /etc/cron.d/` | Inspect system cron jobs |

## 8. Text Processing Commands

| Command | Purpose |
|---|---|
| `grep` | Search matching text |
| `awk` | Extract fields from text |
| `sed` | Filter or modify text |
| `cut` | Extract columns |
| `sort` | Sort lines |
| `uniq` | Identify repeated lines |
| `wc` | Count lines or words |
| `tee` | Display and save output |

### 🔎 Quick SOC Investigation Examples

```bash
# Identify logged-in users
who

# Review running processes
ps aux

# Check listening ports
ss -tulnp

# Search failed authentication events
grep -i "failed" /var/log/auth.log

# Monitor system logs
sudo journalctl -f

# Find files in temporary directories
find /tmp -type f

# Review scheduled tasks
crontab -l

# Extract and count unique IP addresses from a log
awk '{print $1}' access.log | sort | uniq -c
```

### 🎯 Learning Objective

Understand how Linux commands help SOC analysts:

- Investigate suspicious processes and files.
- Analyze authentication and system logs.
- Identify users and privilege levels.
- Monitor network connections.
- Inspect common persistence mechanisms.
- Extract useful information during security investigations.

**Practice these commands in a Linux VM or authorized security lab.**

