# Linux Notes

> 🚀 This repository documents my Linux learning journey toward becoming a Cloud Security Engineer.
> My goal is to build strong Linux fundamentals through hands-on practice, continuous learning, and real-world projects.
> Each topic includes hands-on labs, security perspectives, personal reflections, and key vocabulary to reinforce practical understanding.

---

# Goal

- Learn Linux fundamentals.
- Build practical Linux administration skills.
- Develop a strong foundation for Cloud Security.
- Practice through hands-on labs and real-world projects.
- Document my learning journey on GitHub.
- Continuously improve technical and problem-solving skills.

---

# Learning Roadmap

> 📅 This roadmap represents my one-year Linux learning journey toward becoming a Cloud Security Engineer.

## Week 1 - Linux Fundamentals

### Goal

- Understand Linux fundamentals.
- Build practical Linux administration skills.
- Develop a strong foundation for Cloud Security.

| Status | Day | Topic |
|--------|-----|----------------------------------|
| ✅ | Day 1 | Linux Basic Commands |
| ✅ | Day 2 | Linux Directory Structure |
| ✅ | Day 3 | Linux File Permissions |
| ✅ | Day 4 | Linux Users and Groups |
| ✅ | Day 5 | Linux Processes and Services |
| ✅ | Day 6 | Linux Networking Fundamentals |
| ✅ | Day 7 | Weekly Summary & Review |

---

## Week 2 - Linux System Administration

### Goal

- Learn essential Linux administration skills.
- Build confidence managing Linux servers.
- Prepare for SSH, package management, logging, and automation.

| Status | Day | Topic |
|--------|-----|----------------------------------|
| ⏳ | Day 8 | SSH and Remote Access |
| ⏳ | Day 9 | Package Management |
| ⏳ | Day 10 | Shell and Environment Variables |
| ⏳ | Day 11 | File Search and Text Processing |
| ⏳ | Day 12 | Log Files |
| ⏳ | Day 13 | Cron Jobs |
| ⏳ | Day 14 | Weekly Summary & Review |

---

# Why I'm Learning Linux

Linux is one of the most important skills for Cloud Security Engineers.

This repository is not just a collection of notes.
It documents my learning process, hands-on practice, and security-focused knowledge while preparing for an international Cloud Security career.

---

# Day 1

## Topic

Linux Basic Commands

## Objective

Become familiar with basic Linux commands and navigate the file system.

## Commands

| Command | Description | Example |
|----------|-------------|---------|
| `pwd` | Displays the current working directory. | `pwd` |
| `ls` | Lists files and directories. | `ls -l` |
| `cd` | Changes the current directory. | `cd /home` |
| `mkdir` | Creates a new directory. | `mkdir project` |
| `touch` | Creates an empty file. | `touch file.txt` |
| `cp` | Copies files or directories. | `cp a.txt b.txt` |
| `mv` | Moves or renames files or directories. | `mv old.txt new.txt` |
| `rm` | Removes files or directories. | `rm file.txt` |
| `cat` | Displays file contents. | `cat file.txt` |

## Hands-on Lab

- Navigate directories using `pwd`, `ls`, and `cd`
- Create directories using `mkdir`
- Create files using `touch`
- Copy, move, rename, and delete files

## What I Learned

- Linux commands are case-sensitive.
- The terminal is the primary interface for Linux administration.
- File management is performed through command-line tools.

## Security Perspective

Understanding basic Linux commands is essential because Cloud Security engineers frequently manage Linux servers through the command line.

## Next Step

Linux Directory Structure

---

# Day 2

## Topic

Linux Directory Structure

## Objective

Understand the purpose of the major Linux directories.

## Commands

| Command | Description | Example |
|----------|-------------|---------|
| `pwd` | Displays the current working directory. | `pwd` |
| `ls` | Lists directory contents. | `ls /etc` |
| `cd` | Changes directories. | `cd /var/log` |

## Hands-on Lab

Explore the following directories.

- `/`
- `/home`
- `/etc`
- `/var`
- `/usr`
- `/tmp`

## What I Learned

- `/` is the root directory.
- `/home` stores user home directories.
- `/etc` stores system configuration files.
- `/var` stores logs and variable data.
- `/usr` contains user applications and system utilities.
- `/tmp` stores temporary files.

## Security Perspective

Knowing where configuration files and log files are stored is important for troubleshooting, incident response, and Linux hardening.

## Next Step

Linux File Permissions

---

# Day 3

## Topic

Linux File Permissions

## Objective

Learn how Linux controls access to files and directories.

## Commands

| Command | Description | Example |
|----------|-------------|---------|
| `ls -l` | Displays detailed file permissions. | `ls -l` |
| `chmod` | Changes file permissions. | `chmod 644 file.txt` |

## Hands-on Lab

Create three files.

- `private.txt`
- `shared.txt`
- `script.sh`

Assign different permissions.

```bash
chmod 600 private.txt
chmod 644 shared.txt
chmod 755 script.sh

ls -l
```

Observe how the permissions change after each command.

## What I Learned

- Linux permissions consist of Read, Write, and Execute.
- Permissions are assigned to Owner, Group, and Others.
- Different files require different permission levels.
- `chmod` modifies file permissions.

## Security Perspective

Applying the Principle of Least Privilege helps reduce security risks by granting only the permissions required for each file.

## Next Step

Linux Users and Groups

---

# Day 4

## Topic

Linux Users and Groups

## Objective

Understand how Linux manages users and groups for access control.

## Commands

| Command | Description | Example |
|----------|-------------|---------|
| `whoami` | Displays the currently logged-in user. | `whoami` |
| `id` | Displays the user's UID, GID, and group information. | `id` |
| `groups` | Lists the groups the current user belongs to. | `groups` |
| `sudo` | Executes commands with administrator privileges. | `sudo apt update` |
| `passwd` | Changes a user's password. | `passwd` |

## Hands-on Lab

Run the following commands.

```bash
whoami
id
groups
cat /etc/passwd
```

Observe the relationship between users and groups.

## What I Learned

- Every Linux user has a unique UID.
- Users can belong to one or more groups.
- Groups simplify permission management.
- The root user has unrestricted privileges.

## Security Perspective

Linux users and groups are conceptually similar to AWS IAM identities.
Proper user and group management is fundamental to implementing the Principle of Least Privilege.

## Next Step

Linux Processes and Services

---

# Day 5

## Topic

Linux Processes and Services

## Objective

Understand how Linux manages running processes and learn basic process management commands.

## Commands

| Command | Description | Example |
|----------|-------------|---------|
| `ps` | Displays currently running processes. | `ps` |
| `ps -ef` | Displays all running processes in full format. | `ps -ef` |
| `top` | Displays real-time system and process information. | `top` |
| `htop` | Displays an interactive process viewer (if installed). | `htop` |
| `kill` | Terminates a running process using its PID. | `kill 1234` |
| `kill -9` | Forcefully terminates a running process. | `kill -9 1234` |
| `grep` | Searches for specific text in command output. | `ps -ef \| grep sleep` |

## Hands-on Lab

Run the following commands.

```bash
ps

ps -ef

top

sleep 1000 &

ps -ef | grep sleep

kill <PID>

ps -ef | grep sleep
```

Replace `<PID>` with the Process ID of the `sleep` process.

## What I Learned

- A process is a running instance of a program.
- Every process has its own Process ID (PID).
- The `ps` command displays process information.
- The `top` command monitors processes in real time.
- The `kill` command terminates running processes.
- The `grep` command searches specific text from command output.

## Security Perspective

Monitoring running processes is one of the most important tasks in Linux security.

Security engineers use process monitoring to identify suspicious applications, investigate malware, and troubleshoot abnormal system behavior.

## Reflection

### What did I learn today?

Today I learned how Linux manages running processes and how to monitor them using commands such as `ps`, `top`, and `grep`.

### Why is it important for Cloud Security?

Monitoring running processes helps security engineers detect suspicious activities, investigate incidents, and understand what is happening on a Linux server.

### What will I study next?

Next, I will learn Linux networking fundamentals and understand how Linux systems communicate over a network.

## Next Step

Linux Networking Fundamentals

---

# Day 6

## Topic

Linux Networking Fundamentals

## Objective

Understand the fundamental networking concepts in Linux and learn how to inspect network configuration, routing information, and listening ports.

## Commands

| Command | Description | Example |
|----------|-------------|---------|
| `ip addr` | Displays network interfaces and IP addresses. | `ip addr` |
| `ip route` | Displays the routing table. | `ip route` |
| `hostname` | Displays the system hostname. | `hostname` |
| `hostname -I` | Displays the assigned IP address(es). | `hostname -I` |
| `ping` | Tests network connectivity to another host. | `ping 8.8.8.8` |
| `ss -tuln` | Displays listening TCP and UDP ports. | `ss -tuln` |

## Hands-on Lab

Run the following commands.

```bash
ip addr

ip route

hostname

hostname -I

ping 8.8.8.8

ss -tuln
```

## What I Learned

- Every Linux system can have one or more network interfaces.
- IP addresses identify devices on a network.
- The routing table determines where network traffic is sent.
- The `ping` command is useful for testing network connectivity.
- The `ss` command displays listening ports and active network sockets.

## Security Perspective

Understanding Linux networking is fundamental for Cloud Security.

Security engineers analyze network interfaces, routing information, and listening ports when investigating incidents, securing servers, and troubleshooting connectivity issues.

## Reflection

### What did I learn today?

Today I learned how to inspect network interfaces, routing tables, IP addresses, and listening ports using basic Linux networking commands.

### Why is it important for Cloud Security?

Cloud servers communicate through networks. Understanding networking fundamentals helps identify connectivity issues, detect exposed services, and secure Linux systems.

### What will I study next?

Next, I will review everything I learned during Week 1 and summarize the key concepts before moving on to Linux System Administration.

## Next Step

Week 1 Summary & Review

---

# Week 1 Summary & Review

## Week Summary

This week I learned the fundamentals of Linux, including basic commands, directory structure, file permissions, users and groups, processes, and networking.

These concepts form the foundation of Linux system administration and are essential for building Cloud Security skills.

## Challenges

This week, I focused on understanding the differences between Linux concepts such as processes and services, file permissions, and users versus groups.

Repeated hands-on practice helped me understand how these concepts work in real Linux environments.

## Key Takeaways

- Linux permissions follow the Principle of Least Privilege.
- Users and groups simplify access control.
- Processes can be monitored and managed using Linux commands.
- Networking fundamentals are essential for understanding cloud infrastructure.
- Consistent hands-on practice is the best way to improve Linux skills.

## Reflection

### What did I accomplish this week?

I successfully completed my first week of Linux study and built a strong foundation in Linux fundamentals.

### What was the most important lesson?

I realized that understanding Linux concepts is more valuable than simply memorizing commands.

### What will I study next week?

Next week, I will begin learning Linux System Administration, including SSH, package management, shell environments, log files, and automation.

## Next Week Goal

Learn practical Linux administration skills used in real-world server environments.

---

# Vocabulary

| Term | Meaning |
|------|---------|
| Configuration File | A file that stores system settings. |
| Daemon | A background process running without direct user interaction. |
| Default Gateway | The router that forwards traffic to other networks. |
| Directory | A folder used to organize files. |
| Execute | Permission to run a file or program. |
| File | A collection of data stored on disk. |
| GID | Group Identifier. |
| Group | A collection of users who share permissions. |
| Home Directory | A user's personal working directory. |
| Hostname | The name assigned to a computer on a network. |
| IP Address | A unique address assigned to a device on a network. |
| Network Interface | A hardware or virtual interface used for network communication. |
| Owner | The user who owns a file or directory. |
| Permission | Controls access to files and directories. |
| PID | Process Identifier. |
| Ping | A utility used to test network connectivity. |
| Port | A communication endpoint used by network services. |
| Process | A running instance of a program. |
| Process Monitoring | Observing running processes to maintain system health and security. |
| Root Directory | The top-level directory in Linux. |
| Root User | The superuser with unrestricted privileges. |
| Routing Table | A table that determines how network packets are forwarded. |
| Service | A background program managed by the operating system. |
| Socket | An endpoint for network communication. |
| sudo | Executes commands with administrator privileges. |
| Terminal | A command-line interface used to interact with Linux. |
| TCP | A reliable connection-oriented network protocol. |
| UDP | A connectionless network protocol with low overhead. |
| UID | User Identifier. |
