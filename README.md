# Linux Notes

> 🚀 This repository documents my Linux learning journey toward becoming a Cloud Security Engineer.
> My goal is to build strong Linux fundamentals through hands-on practice, continuous learning, and real-world projects.
> Each topic includes hands-on labs, security perspectives, personal reflections, and key vocabulary to reinforce practical understanding.

---

# Goal

- Learn Linux fundamentals, system administration, and security.
- Build practical troubleshooting and security analysis skills.
- Develop a strong foundation for Cloud Security.
- Practice through hands-on labs and real-world security exercises.
- Apply learned skills through small projects and Linux security audits.
- Document my learning journey and technical growth on GitHub.
- Continuously improve technical and problem-solving skills.

---

# Learning Roadmap

> 📅 This roadmap represents my one-year Linux learning journey toward becoming a Cloud Security Engineer.

## Week 1 - Linux Fundamentals

### Goal

- Understand Linux fundamentals.
- Build practical Linux administration skills.
- Develop a strong foundation for Cloud Security.

| Status | Day    | Topic                                  |
| ------ | ------ | -------------------------------------- |
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

| Status | Day    | Topic                                  |
| ------ | ------ | -------------------------------------- |
| ✅ | Day 8 | SSH and Remote Access |
| ✅ | Day 9 | Package Management |
| ✅ | Day 10 | Shell and Environment Variables |
| ✅ | Day 11 | File Search and Text Processing |
| ✅ | Day 12 | Log Files |
| ✅ | Day 13 | Cron Jobs |
| ✅ | Day 14 | Weekly Summary & Review |

---

## Week 3 - Linux Security Fundamentals

### Goal

- Understand fundamental Linux security concepts.
- Learn how authentication, privileges, and network controls protect Linux systems.
- Build practical security skills for managing cloud-based Linux servers.

| Status | Day    | Topic                                  |
| ------ | ------ | -------------------------------------- |
| ✅ | Day 15 | sudo and Privilege Management      |
| ✅ | Day 16 | Linux Authentication and PAM       |
| ✅ | Day 17 | Linux Firewall Fundamentals        |
| ✅ | Day 18 | SSH Hardening                      |
| ✅ | Day 19 | File Integrity and Hashing         |
| ✅ | Day 20 | Basic Linux Security Auditing      |
| ✅ | Day 21 | Weekly Summary & Review            |

---

## Week 4 - Linux Troubleshooting and Security Operations

### Goal

- Learn how to troubleshoot common Linux system and network problems.
- Develop basic Linux security investigation skills.
- Apply Linux knowledge through practical system and security analysis.

| Status | Day    | Topic                                  |
| ------ | ------ | -------------------------------------- |
| ✅ | Day 22 | System Resource Monitoring             |
| ⏳ | Day 23 | Network Troubleshooting                |
| ⏳ | Day 24 | Service Troubleshooting with systemd   |
| ⏳ | Day 25 | Security Log Analysis                  |
| ⏳ | Day 26 | Bash Scripting Fundamentals            |
| ⏳ | Day 27 | Linux Security Audit Mini Project      |
| ⏳ | Day 28 | Monthly Summary & Review               |

---

# Why I'm Learning Linux

Linux is one of the most important skills for Cloud Security Engineers.

This repository is not just a collection of notes.
It documents my learning process, hands-on practice, and security-focused knowledge while preparing for an international Cloud Security career.

---

# Day 1

## Topic

Linux Basic Commands

### Objective

Become familiar with basic Linux commands and navigate the file system.

### Commands

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

### Hands-on Lab

- Navigate directories using `pwd`, `ls`, and `cd`
- Create directories using `mkdir`
- Create files using `touch`
- Copy, move, rename, and delete files

### What I Learned

- Linux commands are case-sensitive.
- The terminal is the primary interface for Linux administration.
- File management is performed through command-line tools.

### Security Perspective

Understanding basic Linux commands is essential because Cloud Security engineers frequently manage Linux servers through the command line.

### Next Step

Linux Directory Structure

---

# Day 2

## Topic

Linux Directory Structure

### Objective

Understand the purpose of the major Linux directories.

### Commands

| Command | Description | Example |
|----------|-------------|---------|
| `pwd` | Displays the current working directory. | `pwd` |
| `ls` | Lists directory contents. | `ls /etc` |
| `cd` | Changes directories. | `cd /var/log` |

### Hands-on Lab

Explore the following directories.

- `/`
- `/home`
- `/etc`
- `/var`
- `/usr`
- `/tmp`

### What I Learned

- `/` is the root directory.
- `/home` stores user home directories.
- `/etc` stores system configuration files.
- `/var` stores logs and variable data.
- `/usr` contains user applications and system utilities.
- `/tmp` stores temporary files.

### Security Perspective

Knowing where configuration files and log files are stored is important for troubleshooting, incident response, and Linux hardening.

### Next Step

Linux File Permissions

---

# Day 3

## Topic

Linux File Permissions

### Objective

Learn how Linux controls access to files and directories.

### Commands

| Command | Description | Example |
|----------|-------------|---------|
| `ls -l` | Displays detailed file permissions. | `ls -l` |
| `chmod` | Changes file permissions. | `chmod 644 file.txt` |

### Hands-on Lab

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

### What I Learned

- Linux permissions consist of Read, Write, and Execute.
- Permissions are assigned to Owner, Group, and Others.
- Different files require different permission levels.
- `chmod` modifies file permissions.

### Security Perspective

Applying the Principle of Least Privilege helps reduce security risks by granting only the permissions required for each file.

### Next Step

Linux Users and Groups

---

# Day 4

## Topic

Linux Users and Groups

### Objective

Understand how Linux manages users and groups for access control.

### Commands

| Command | Description | Example |
|----------|-------------|---------|
| `whoami` | Displays the currently logged-in user. | `whoami` |
| `id` | Displays the user's UID, GID, and group information. | `id` |
| `groups` | Lists the groups the current user belongs to. | `groups` |
| `sudo` | Executes commands with administrator privileges. | `sudo apt update` |
| `passwd` | Changes a user's password. | `passwd` |

### Hands-on Lab

Run the following commands.

```bash
whoami
id
groups
cat /etc/passwd
```

Observe the relationship between users and groups.

### What I Learned

- Every Linux user has a unique UID.
- Users can belong to one or more groups.
- Groups simplify permission management.
- The root user has unrestricted privileges.

### Security Perspective

Linux users and groups are conceptually similar to AWS IAM identities.
Proper user and group management is fundamental to implementing the Principle of Least Privilege.

### Next Step

Linux Processes and Services

---

# Day 5

## Topic

Linux Processes and Services

### Objective

Understand how Linux manages running processes and learn basic process management commands.

### Commands

| Command | Description | Example |
|----------|-------------|---------|
| `ps` | Displays currently running processes. | `ps` |
| `ps -ef` | Displays all running processes in full format. | `ps -ef` |
| `top` | Displays real-time system and process information. | `top` |
| `htop` | Displays an interactive process viewer (if installed). | `htop` |
| `kill` | Terminates a running process using its PID. | `kill 1234` |
| `kill -9` | Forcefully terminates a running process. | `kill -9 1234` |
| `grep` | Searches for specific text in command output. | `ps -ef \| grep sleep` |

### Hands-on Lab

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

### What I Learned

- A process is a running instance of a program.
- Every process has its own Process ID (PID).
- The `ps` command displays process information.
- The `top` command monitors processes in real time.
- The `kill` command terminates running processes.
- The `grep` command searches specific text from command output.

### Security Perspective

Monitoring running processes is one of the most important tasks in Linux security.

Security engineers use process monitoring to identify suspicious applications, investigate malware, and troubleshoot abnormal system behavior.

### Reflection

#### What did I learn today?

Today I learned how Linux manages running processes and how to monitor them using commands such as `ps`, `top`, and `grep`.

#### Why is it important for Cloud Security?

Monitoring running processes helps security engineers detect suspicious activities, investigate incidents, and understand what is happening on a Linux server.

#### What will I study next?

Next, I will learn Linux networking fundamentals and understand how Linux systems communicate over a network.

### Next Step

Linux Networking Fundamentals

---

# Day 6

## Topic

Linux Networking Fundamentals

### Objective

Understand the fundamental networking concepts in Linux and learn how to inspect network configuration, routing information, and listening ports.

### Commands

| Command | Description | Example |
|----------|-------------|---------|
| `ip addr` | Displays network interfaces and IP addresses. | `ip addr` |
| `ip route` | Displays the routing table. | `ip route` |
| `hostname` | Displays the system hostname. | `hostname` |
| `hostname -I` | Displays the assigned IP address(es). | `hostname -I` |
| `ping` | Tests network connectivity to another host. | `ping 8.8.8.8` |
| `ss -tuln` | Displays listening TCP and UDP ports. | `ss -tuln` |

### Hands-on Lab

Run the following commands.

```bash
ip addr

ip route

hostname

hostname -I

ping 8.8.8.8

ss -tuln
```

### What I Learned

- Every Linux system can have one or more network interfaces.
- IP addresses identify devices on a network.
- The routing table determines where network traffic is sent.
- The `ping` command is useful for testing network connectivity.
- The `ss` command displays listening ports and active network sockets.

### Security Perspective

Understanding Linux networking is fundamental for Cloud Security.

Security engineers analyze network interfaces, routing information, and listening ports when investigating incidents, securing servers, and troubleshooting connectivity issues.

### Reflection

#### What did I learn today?

Today I learned how to inspect network interfaces, routing tables, IP addresses, and listening ports using basic Linux networking commands.

#### Why is it important for Cloud Security?

Cloud servers communicate through networks. Understanding networking fundamentals helps identify connectivity issues, detect exposed services, and secure Linux systems.

#### What will I study next?

Next, I will review everything I learned during Week 1 and summarize the key concepts before moving on to Linux System Administration.

### Next Step

Week 1 Summary & Review

---

# Day 7

## Topic

Week 1 Summary & Review

### Objective

Review the Linux fundamentals covered during Week 1 and understand how basic Linux concepts work together as the foundation for system administration and Cloud Security.

### Week 1 Topics

| Day | Topic |
|---|---|
| Day 1 | Linux Basic Commands |
| Day 2 | Linux Directory Structure |
| Day 3 | Linux File Permissions |
| Day 4 | Linux Users and Groups |
| Day 5 | Linux Processes and Services |
| Day 6 | Linux Networking Fundamentals |

### Key Commands Reviewed

| Area | Commands |
|---|---|
| Basic Navigation | `pwd`, `ls`, `cd` |
| File Management | `touch`, `mkdir`, `cp`, `mv`, `rm` |
| File Inspection | `cat`, `less`, `head`, `tail` |
| Permissions | `chmod`, `chown`, `chgrp` |
| Users & Groups | `whoami`, `id`, `groups`, `getent` |
| Processes | `ps`, `top`, `pgrep`, `kill` |
| Services | `systemctl` |
| Networking | `ip`, `ping`, `ss`, `curl` |

### Fundamentals Review Lab

I reviewed the basic state of my Linux environment using commands learned during Week 1.

```bash
pwd
ls -la

whoami
id
groups

ps aux
systemctl --type=service --state=running

ip addr
ip route
ss -tuln
```

I also reviewed file permissions and ownership.

```bash
ls -l

touch review-file.txt

chmod 640 review-file.txt

ls -l review-file.txt
```

### Concept Review

During Week 1, I learned how several fundamental Linux concepts are connected.

```text
Linux System
     │
     ├── Files and Directories
     │        │
     │        └── Permissions
     │
     ├── Users and Groups
     │        │
     │        └── Access Control
     │
     ├── Processes
     │        │
     │        └── Services
     │
     └── Networking
              │
              ├── IP Address
              ├── Routes
              └── Listening Ports
```

Understanding these relationships is more important than simply memorizing individual commands.

### Security Perspective

Linux fundamentals are closely related to system security.

File permissions and ownership control who can access resources, while users and groups provide the foundation for access management.

Processes and services help identify what is running on a system, and networking commands provide visibility into network interfaces, routes, and listening services.

These concepts provide the foundation for applying the Principle of Least Privilege and understanding Linux security.

### Challenges

This week, I focused on understanding the differences between Linux concepts such as processes and services, file permissions, and users versus groups.

Repeated hands-on practice helped me understand how these concepts work in real Linux environments.

### Week 1 Key Takeaways

- Linux commands provide tools for interacting with and managing the operating system.
- The Linux directory structure organizes system files according to their purpose.
- File permissions and ownership control access to system resources.
- Linux permissions support the Principle of Least Privilege.
- Users and groups simplify access control and permission management.
- Processes represent running programs, while services provide background system functionality.
- Networking fundamentals are essential for understanding Linux servers and cloud infrastructure.
- Hands-on practice is essential for developing practical Linux skills.

### Reflection

#### What did I accomplish this week?

I successfully completed my first week of Linux study and built a strong foundation in Linux fundamentals.

#### What was the most important lesson?

I realized that understanding how Linux concepts are connected is more valuable than simply memorizing commands.

#### What was difficult?

I focused on understanding the differences between processes and services, file permissions, and users versus groups.

Repeated hands-on practice helped reinforce these concepts.

#### Why is it important for Cloud Security?

Linux is widely used for cloud workloads and servers.

Understanding Linux permissions, users, processes, services, and networking provides an essential foundation for secure system administration and Cloud Security.

#### What will I study next?

Next, I will begin Linux System Administration, including SSH, package management, shell environments, file searching, log analysis, and task scheduling.

### Next Step

Linux System Administration — SSH and Remote Access

---

# Day 8

## Topic

SSH and Remote Access

### Objective

Understand how SSH provides secure remote access to Linux systems and learn the fundamentals of SSH key-based authentication.

### Commands

| Command | Description | Example |
|---|---|---|
| `ssh -V` | Displays the installed SSH client version. | `ssh -V` |
| `systemctl status ssh` | Checks the status of the SSH service. | `systemctl status ssh` |
| `cat /etc/ssh/sshd_config` | Displays the SSH server configuration. | `cat /etc/ssh/sshd_config` |
| `ls -la ~/.ssh` | Displays SSH-related files and keys. | `ls -la ~/.ssh` |
| `ssh-keygen` | Generates a new SSH key pair. | `ssh-keygen -t ed25519` |

### Hands-on Lab

I inspected the SSH client and server configuration and created an SSH key pair.

```bash
ssh -V

systemctl status ssh

grep -E "Port|PermitRootLogin|PasswordAuthentication|PubkeyAuthentication" /etc/ssh/sshd_config

ls -la ~/.ssh

ssh-keygen -t ed25519 -C "learning-ssh"

ls -la ~/.ssh
```

### What I Learned

- SSH provides encrypted remote access to Linux systems.
- SSH commonly uses TCP port 22.
- An SSH client initiates a connection to an SSH server.
- Public key authentication uses a public and private key pair.
- The private key must remain secret.
- The public key can be registered on remote systems for authentication.

### Security Perspective

SSH is widely used to administer Linux servers and cloud infrastructure.

Key-based authentication can provide stronger security than password-only authentication when keys are managed properly. Private keys must be protected carefully because exposure of a private key may allow unauthorized access to systems that trust the corresponding public key.

### Reflection

#### What did I learn today?

Today I learned how SSH enables secure remote access and how public and private keys are used for authentication.

#### Why is it important for Cloud Security?

Cloud infrastructure frequently relies on secure remote administration. Understanding SSH authentication and key management helps reduce the risk of unauthorized server access.

#### What will I study next?

Next, I will learn how Linux package management works and how software packages are installed, updated, and removed.

### Next Step

Package Management

---

# Day 9

## Topic

Linux Package Management

### Objective

Understand how Linux package management works and learn how to search, install, inspect, update, and remove software packages using APT and dpkg.

### Commands

| Command | Description | Example |
|---|---|---|
| `apt update` | Updates the local package index from configured repositories. | `sudo apt update` |
| `apt search` | Searches available packages. | `apt search tree` |
| `apt show` | Displays detailed information about a package. | `apt show tree` |
| `apt install` | Installs a package and its dependencies. | `sudo apt install tree` |
| `apt remove` | Removes an installed package. | `sudo apt remove tree` |
| `apt purge` | Removes a package and its package-managed configuration files. | `sudo apt purge tree` |
| `apt list --upgradable` | Displays packages for which upgrades are available. | `apt list --upgradable` |
| `dpkg -l` | Lists installed Debian packages. | `dpkg -l` |
| `dpkg -L` | Lists files installed by a package. | `dpkg -L tree` |

### Hands-on Lab

I inspected the configured package repository and practiced searching, installing, inspecting, and removing a Linux package.

```bash
cat /etc/apt/sources.list

sudo apt update

apt list --upgradable

apt search tree

apt show tree

sudo apt install tree

tree --version

dpkg -l | grep tree

dpkg -L tree

sudo apt remove tree
```

### What I Learned

- APT is a package management tool used by Debian-based Linux distributions.
- Package repositories provide software packages and package metadata.
- `apt update` refreshes the local package index rather than upgrading installed packages.
- APT can resolve package dependencies during software installation.
- `dpkg` can inspect installed Debian packages and their files.
- Package management is important for maintaining secure and reliable Linux systems.

### Security Perspective

Keeping software packages appropriately patched helps reduce exposure to known vulnerabilities.

Packages should come from trusted repositories, and unnecessary software should be avoided to reduce the system's attack surface.

Understanding package sources and dependencies is also important when considering software supply-chain security.

### Reflection

#### What did I learn today?

Today I learned how Linux package management works and practiced managing software using APT and dpkg.

#### Why is it important for Cloud Security?

Cloud servers depend on many software packages. Understanding how packages are installed, updated, and removed helps maintain secure systems and reduce exposure to vulnerable or unnecessary software.

#### What will I study next?

Next, I will learn about the Linux shell and environment variables.

### Next Step

Shell and Environment Variables

---

# Day 10

## Topic

Shell and Environment Variables

### Objective

Understand how the Linux shell works and learn how shell variables, environment variables, and the PATH variable affect command execution and processes.

### Commands

| Command | Description | Example |
|---|---|---|
| `echo` | Displays text or the value of a variable. | `echo $HOME` |
| `env` | Displays environment variables. | `env` |
| `export` | Exports a variable so that child processes can inherit it. | `export CLOUD="AWS"` |
| `unset` | Removes a shell variable or environment variable. | `unset CLOUD` |
| `which` | Shows the executable that would be found through PATH for a command. | `which python3` |
| `ps -p $$` | Displays information about the current shell process. | `ps -p $$` |

### Important Environment Variables

| Variable | Description |
|---|---|
| `HOME` | The current user's home directory. |
| `USER` | The current username. |
| `SHELL` | The user's configured login shell. |
| `PATH` | Directories searched when resolving executable commands. |
| `LANG` | Language and locale configuration. |

### Hands-on Lab

I inspected my shell environment and practiced creating, exporting, and removing variables.

```bash
echo $SHELL
ps -p $$

echo $HOME
echo $USER
echo $PATH

which ls
which git
which python3
which ssh

env
env | grep PATH

MY_NAME="Insoo"
echo $MY_NAME

CLOUD="AWS"
echo $CLOUD

export CLOUD="AWS"
echo $CLOUD

unset CLOUD
```

I also tested the difference between a shell variable and an exported environment variable by creating a child shell.

### What I Learned

- A shell interprets commands entered by the user.
- Environment variables provide configuration information to processes.
- `PATH` determines where the shell searches for executable commands.
- Shell variables are not automatically inherited by child processes.
- `export` makes a variable available to child processes.
- Shell configuration files can be used to define persistent environment settings.

### Security Perspective

Environment variables are frequently used to provide application configuration and sometimes sensitive information.

Secrets such as API keys and credentials should never be committed to a public Git repository.

Using environment variables does not automatically make secrets secure, so secret management and access control are still necessary.

### Reflection

#### What did I learn today?

Today I learned how the Linux shell handles variables and how environment variables affect command execution and child processes.

#### Why is it important for Cloud Security?

Cloud applications and automation tools depend heavily on environment configuration. Understanding environment variables helps prevent configuration mistakes and accidental exposure of sensitive credentials.

#### What will I study next?

Next, I will learn how to search for files and process text efficiently in Linux.

### Next Step

File Search and Text Processing

---

# Day 11

## Topic

File Search and Text Processing

### Objective

Learn how to search for files and efficiently process text and log data using common Linux command-line tools.

### Commands

| Command | Description | Example |
|---|---|---|
| `find` | Searches for files and directories based on specified conditions. | `find . -name "*.log"` |
| `grep` | Searches file contents for matching text patterns. | `grep "ERROR" app.log` |
| `head` | Displays the beginning of a file. | `head -n 5 app.log` |
| `tail` | Displays the end of a file. | `tail -n 5 app.log` |
| `wc` | Counts lines, words, and bytes. | `wc -l app.log` |
| `sort` | Sorts lines of text. | `sort users.txt` |
| `uniq` | Removes or counts adjacent duplicate lines. | `sort users.txt \| uniq -c` |
| `\|` | Passes the output of one command to another command. | `grep "ERROR" app.log \| wc -l` |

### Hands-on Lab

I created sample files and logs and practiced searching and analyzing them.

```bash
mkdir -p ~/day11-lab/logs
cd ~/day11-lab

touch notes.txt
touch config.conf
touch logs/app.log
touch logs/security.log

find .
find . -name "*.log"
find . -type f

grep "ERROR" logs/app.log
grep -i "error" logs/app.log
grep -n "ERROR" logs/app.log

head -n 3 logs/app.log
tail -n 2 logs/app.log

grep "ERROR" logs/app.log | wc -l

sort users.txt
sort users.txt | uniq -c
```

### Log Analysis Practice

I also created a sample security log and used text-processing commands to identify repeated failed login attempts.

```bash
grep "FAILED" logs/security.log

grep "FAILED" logs/security.log | wc -l

grep "10.0.0.5" logs/security.log | wc -l
```

### What I Learned

- `find` searches for files and directories.
- `grep` searches for patterns inside files.
- Pipes allow multiple commands to be combined.
- `head` and `tail` help inspect portions of large files.
- `wc` can count matching log events.
- `sort` and `uniq` can help identify repeated values and patterns.
- Linux command-line tools can be combined to perform simple log analysis.

### Security Perspective

Searching and processing text is an important skill for security investigations.

System and application logs can contain information about failed authentication attempts, suspicious requests, configuration errors, and other security events.

Command-line tools such as `grep`, `find`, `sort`, `uniq`, and `wc` allow security engineers to quickly investigate large amounts of text data.

However, repeated log entries alone do not prove that an attack occurred. Security events should be analyzed together with additional context.

### Reflection

#### What did I learn today?

Today I learned how to search Linux files and analyze text and log data using common command-line tools.

#### Why is it important for Cloud Security?

Cloud workloads generate large amounts of logs and configuration data. Being able to quickly search and analyze this information helps with troubleshooting, incident investigation, and security monitoring.

#### What will I study next?

Next, I will learn about Linux log files and how the operating system records important system events.

### Next Step

Log Files

---

# Day 12

## Topic

Linux Log Files

### Objective

Understand how Linux records system and service events and learn how to inspect and analyze logs using `/var/log` and `journalctl`.

### Commands

| Command | Description | Example |
|---|---|---|
| `ls /var/log` | Displays available traditional log files and directories. | `ls -lah /var/log` |
| `journalctl` | Displays logs collected by the systemd journal. | `journalctl` |
| `journalctl -b` | Displays logs from the current boot. | `journalctl -b` |
| `journalctl -u` | Displays logs for a specific systemd unit. | `journalctl -u ssh` |
| `journalctl -p` | Filters journal entries by priority. | `journalctl -p err` |
| `journalctl --since` | Displays logs after a specified time. | `journalctl --since today` |
| `journalctl -f` | Follows new journal entries in real time. | `journalctl -f` |
| `dmesg` | Displays kernel-related messages. | `dmesg` |

### Hands-on Lab

I inspected Linux log locations and practiced filtering system and service logs.

```bash
ls -lah /var/log

tail /var/log/dpkg.log

grep -i "install" /var/log/dpkg.log

journalctl -n 20

journalctl -b

journalctl -b -n 30

journalctl -u ssh

journalctl --since today

journalctl -b -p err

journalctl -k
```

I also combined journal output with Linux text-processing commands.

```bash
journalctl -b | grep -i "error"

journalctl -b | grep -i "failed"

journalctl -b | grep -i "failed" | wc -l
```

### Log Analysis Practice

I created a sample authentication log and investigated repeated failed login events.

```bash
grep "Failed" ~/day12-lab/auth.log

grep "Failed" ~/day12-lab/auth.log | wc -l

grep "10.0.0.5" ~/day12-lab/auth.log
```

### What I Learned

- Linux records important system, service, application, and kernel events in logs.
- Traditional log files can be stored under `/var/log`.
- Modern Linux systems commonly use the systemd journal for centralized system logging.
- `journalctl` can filter logs by boot, service, time, and priority.
- Linux text-processing commands can be combined with log data for investigation.
- Repeated events can indicate suspicious activity, but logs must be interpreted in context.

### Security Perspective

Logs are essential for security monitoring, troubleshooting, and incident investigation.

Security engineers use logs to understand what happened, when it happened, which user or system was involved, and whether an event is part of a larger pattern.

Logs stored only on the affected host can potentially be modified or deleted after a compromise. Centralized logging can improve visibility, retention, and investigation capabilities.

### Reflection

#### What did I learn today?

Today I learned where Linux logs are stored and how to investigate system and service events using `journalctl` and command-line text-processing tools.

#### Why is it important for Cloud Security?

Cloud servers generate logs that can reveal authentication failures, service errors, suspicious activity, and configuration changes. Understanding Linux logging provides a foundation for cloud monitoring and incident response.

#### What will I study next?

Next, I will learn how Linux scheduled tasks work using cron.

### Next Step

Cron Jobs

---

# Day 13

## Topic

Cron Jobs and Task Scheduling

### Objective

Understand how Linux schedules recurring tasks using cron and learn how to create, inspect, and securely manage cron jobs.

### Commands

| Command | Description | Example |
|---|---|---|
| `systemctl status cron` | Checks the status of the cron service. | `systemctl status cron` |
| `crontab -l` | Lists the current user's cron jobs. | `crontab -l` |
| `crontab -e` | Opens the current user's crontab for editing. | `crontab -e` |
| `journalctl -u cron` | Displays logs generated by the cron service. | `journalctl -u cron` |
| `cat /etc/crontab` | Displays the system-wide crontab configuration. | `cat /etc/crontab` |
| `ls /etc/cron.*` | Displays system cron directories. | `ls -la /etc/cron.*` |
| `git show` | Displays details and changes from a Git commit. | `git show <commit-id>` |

### Cron Schedule Format

```text
* * * * * command
│ │ │ │ │
│ │ │ │ └─ Day of Week
│ │ │ └─── Month
│ │ └───── Day of Month
│ └─────── Hour
└───────── Minute
```

For example:

```text
30 2 * * *
```

represents a task scheduled every day at 02:30.

### Hands-on Lab

I created a simple shell script that records the execution time to a log file.

```bash
mkdir -p ~/day13-lab
```

```bash
#!/bin/bash

echo "Cron executed at $(date)" >> ~/day13-lab/cron.log
```

I then made the script executable and tested it manually.

```bash
chmod +x ~/day13-lab/cron-test.sh

~/day13-lab/cron-test.sh

cat ~/day13-lab/cron.log
```

After confirming that the script worked correctly, I temporarily scheduled it using `crontab`.

```bash
crontab -e
```

Example test schedule:

```cron
* * * * * /home/<username>/day13-lab/cron-test.sh
```

After verifying the cron execution, I removed the test schedule.

### System Cron Inspection

I also inspected system-level scheduled tasks.

```bash
cat /etc/crontab

ls -la /etc/cron.*
```

### What I Learned

- Cron allows Linux to execute commands and scripts automatically according to a schedule.
- Each user can manage scheduled jobs using `crontab`.
- Cron expressions specify the minute, hour, day, month, and weekday of execution.
- Automated tasks should be manually tested before being scheduled.
- Cron jobs may run with a different environment from an interactive shell.
- Absolute paths help make scheduled jobs more predictable.
- System cron jobs and user cron jobs are managed differently.

### Security Perspective

Cron jobs are useful for automation, but they can also introduce security risks.

Attackers may use scheduled tasks as a persistence mechanism after compromising a system.

Security reviews should therefore inspect user crontabs, system cron configurations, scheduled scripts, and their file permissions.

Scripts executed with elevated privileges must not be writable by unauthorized users.

### Reflection

#### What did I learn today?

Today I learned how Linux schedules recurring tasks using cron and how to create, test, inspect, and remove scheduled jobs.

#### Why is it important for Cloud Security?

Automation is essential for system and cloud operations. Understanding scheduled tasks also helps security engineers identify unauthorized persistence and insecure automation configurations.

#### What will I study next?

Next, I will review the Linux System Administration topics covered during Week 2.

### Next Step

Week 2 Summary & Review

---

# Day 14

## Topic

Week 2 Summary & Review

### Objective

Review the Linux system administration topics covered during Week 2 and apply them together through a basic Linux administration and troubleshooting exercise.

### Week 2 Topics

| Day | Topic |
|---|---|
| Day 8 | SSH and Remote Access |
| Day 9 | Package Management |
| Day 10 | Shell and Environment Variables |
| Day 11 | File Search and Text Processing |
| Day 12 | Log Files |
| Day 13 | Cron Jobs |

### Key Commands Reviewed

| Area | Commands |
|---|---|
| SSH | `ssh`, `ssh-keygen`, `systemctl status ssh` |
| Packages | `apt`, `apt-cache` |
| Shell | `echo`, `env`, `export`, `which` |
| File Search | `find`, `grep` |
| Text Processing | `head`, `tail`, `wc`, `sort`, `uniq` |
| Logs | `journalctl`, `dmesg` |
| Scheduling | `crontab`, `cron` |
| Network | `ip`, `ss` |
| Services | `systemctl` |

### Administration Review Lab

I reviewed the basic state of my Linux environment using commands learned during Weeks 1 and 2.

```bash
hostname
uname -a
uptime

ps aux
systemctl --type=service --state=running

ip addr
ip route
ss -tuln

systemctl status ssh

journalctl -b -n 30
journalctl -b -p err
journalctl -u ssh -n 20

crontab -l
cat /etc/crontab
ls -la /etc/cron.d/
```

### Troubleshooting Approach

Instead of immediately changing a configuration when a problem occurs, I learned to investigate the system step by step.

For example, when troubleshooting SSH connectivity:

```text
Service Status
      ↓
Listening Port
      ↓
Network Configuration
      ↓
SSH Configuration
      ↓
Authentication
      ↓
Logs
```

This approach helps identify the actual cause of a problem before making changes.

### Security Perspective

Linux administration and security are closely connected.

Processes, services, network connections, logs, scheduled tasks, users, and file permissions can all provide useful information when investigating suspicious activity.

I also learned that individual log events should not automatically be treated as proof of an attack. Security events should be analyzed together with additional context and evidence.

### Week 2 Key Takeaways

- SSH provides secure remote access to Linux systems.
- Package management helps maintain installed software.
- Shell and environment variables affect command and application behavior.
- `find` and `grep` are essential tools for locating files and information.
- Pipes allow Linux commands to be combined for efficient text processing.
- System logs are important for troubleshooting and security investigations.
- Cron provides scheduled automation but can also be relevant when investigating persistence.
- Linux administration requires understanding how multiple system components interact.

### Reflection

#### What did I learn this week?

During Week 2, I learned essential Linux administration skills including remote access, package management, shell environments, file searching, log analysis, and task scheduling.

More importantly, I started to understand how these individual Linux components interact during system administration and troubleshooting.

#### What was difficult?

I will continue reviewing the topics and commands that were difficult to understand or remember during the week.

#### Why is it important for Cloud Security?

Cloud workloads frequently run on Linux systems. Understanding Linux administration helps with secure configuration, troubleshooting, monitoring, incident investigation, and automation.

#### What will I study next?

Next, I will begin Linux Security Fundamentals, starting with sudo and privilege management.

### Next Step

Linux Security Fundamentals — sudo and Privilege Management

---

# Day 15

## Topic

sudo and Privilege Management

### Objective

Understand Linux privilege management, the role of the root account, and how sudo can be used to provide controlled administrative access.

### Commands

| Command | Description | Example |
|---|---|---|
| `id` | Displays user and group identity information. | `id root` |
| `sudo` | Executes an authorized command with another user's privileges, typically root. | `sudo apt update` |
| `sudo -l` | Lists sudo privileges available to the current user. | `sudo -l` |
| `groups` | Displays the groups associated with a user. | `groups securitylab` |
| `getent group` | Retrieves group information from configured system databases. | `getent group sudo` |
| `visudo` | Safely edits and validates sudoers configuration. | `sudo visudo` |
| `usermod -aG` | Adds a user to a supplementary group while preserving existing supplementary groups. | `sudo usermod -aG sudo securitylab` |
| `deluser` | Removes a user from a group on Debian-based systems. | `sudo deluser securitylab sudo` |

### Root and Privileges

The root account is the Linux superuser and normally has UID 0.

```bash
id root
```

Administrative privileges provide powerful control over a Linux system, but unnecessary elevated access increases both operational and security risks.

The Principle of Least Privilege recommends granting only the permissions required to perform a task.

### sudo

`sudo` allows authorized users to execute commands with elevated privileges without continuously operating from a root shell.

I inspected my current sudo privileges and group membership.

```bash
sudo -l

groups

getent group sudo
```

### sudoers

I inspected the sudo configuration and learned that `/etc/sudoers` controls important sudo authorization rules.

```bash
sudo less /etc/sudoers

sudo ls -la /etc/sudoers.d/
```

I also learned that `visudo` should be used when editing sudoers configuration because it can validate the configuration syntax.

```bash
sudo visudo
```

### Hands-on Lab

I created a temporary user to practice privilege management.

```bash
sudo useradd -m securitylab

id securitylab

groups securitylab
```

I then added the user to the sudo group.

```bash
sudo usermod -aG sudo securitylab

groups securitylab
```

After verifying the group membership, I removed the sudo privilege and cleaned up the test account.

```bash
sudo deluser securitylab sudo

groups securitylab

sudo userdel -r securitylab
```

### What I Learned

- The root account has highly privileged access to the Linux system.
- UID 0 identifies the superuser privilege context.
- `sudo` provides controlled access to elevated commands.
- sudo privileges can be inspected using `sudo -l`.
- Linux groups can be used as part of privilege management.
- `/etc/sudoers` and `/etc/sudoers.d/` define sudo authorization rules.
- `visudo` provides a safer method for editing sudoers configuration.
- Administrative privileges should follow the Principle of Least Privilege.

### Security Perspective

Privilege management is a fundamental Linux security control.

Users should not receive unrestricted administrative privileges unless they are required.

Overly permissive sudo configurations, insecure privileged scripts, and other privilege-related misconfigurations can increase the risk of privilege escalation.

Security reviews should therefore examine privileged accounts, sudo permissions, group memberships, and privileged configuration carefully.

### Reflection

#### What did I learn today?

Today I learned how Linux manages administrative privileges using the root account, sudo, groups, and sudoers configuration.

#### Why is it important for Cloud Security?

Linux servers are commonly used for cloud workloads. Restricting administrative privileges reduces the impact of compromised accounts, configuration mistakes, and unauthorized activity.

The same Least Privilege principle is also fundamental to cloud IAM security.

#### What will I study next?

Next, I will learn how Linux authentication works and understand the role of PAM.

### Next Step

Linux Authentication and PAM

---

# Day 16

## Topic

Linux Authentication and PAM

### Objective

Understand how Linux manages user authentication and learn the basic role of PAM (Pluggable Authentication Modules) in providing a common authentication framework for Linux applications and services.

### Authentication vs Authorization

Authentication verifies the identity of a user.

```text
Who are you?
```

Authorization determines what an authenticated user is allowed to do.

```text
What are you allowed to do?
```

Both concepts are fundamental to Linux and Cloud Security.

### Important Authentication Files

| File | Description |
|---|---|
| `/etc/passwd` | Stores general user account information such as UID, GID, home directory, and login shell. |
| `/etc/shadow` | Stores protected password-related authentication and password aging information. |
| `/etc/pam.d/` | Contains PAM configuration used by applications and services. |

### Commands

| Command | Description | Example |
|---|---|---|
| `getent passwd` | Retrieves user account information. | `getent passwd "$(whoami)"` |
| `passwd -S` | Displays password status information for an account. | `sudo passwd -S "$(whoami)"` |
| `chage -l` | Displays password aging information. | `sudo chage -l "$(whoami)"` |
| `ls -l` | Displays permissions and ownership information. | `ls -l /etc/shadow` |
| `journalctl` | Displays system logs that may contain authentication-related events. | `journalctl -b` |

### `/etc/passwd` and `/etc/shadow`

I inspected the Linux account databases and compared their permissions.

```bash
getent passwd "$(whoami)"

ls -l /etc/passwd
ls -l /etc/shadow
```

`/etc/passwd` contains general account information and is normally readable by users.

Sensitive password-related information is separated into `/etc/shadow`, which has more restrictive access.

I learned that Linux does not normally store user passwords as plaintext in `/etc/shadow`.

### Password and Account Information

I inspected the password status and aging information for my account.

```bash
sudo passwd -S "$(whoami)"

sudo chage -l "$(whoami)"
```

These commands can provide information about password status, password expiration, and account expiration.

### PAM

PAM stands for Pluggable Authentication Modules.

It provides a common authentication framework that can be used by Linux applications and services such as login, sudo, su, and SSH-related components.

I inspected the available PAM configuration.

```bash
ls -la /etc/pam.d/

cat /etc/pam.d/sudo

cat /etc/pam.d/common-auth
```

### PAM Module Types

| Type | Purpose |
|---|---|
| `auth` | Handles authentication-related operations. |
| `account` | Checks account-related conditions and restrictions. |
| `password` | Handles password and credential updates. |
| `session` | Performs tasks associated with starting and ending sessions. |

### Hands-on Lab

I investigated the authentication configuration of my Linux environment without modifying the authentication settings.

```bash
whoami
id

getent passwd "$(whoami)"

ls -l /etc/passwd
ls -l /etc/shadow

sudo passwd -S "$(whoami)"
sudo chage -l "$(whoami)"

ls -la /etc/pam.d/

cat /etc/pam.d/sudo
cat /etc/pam.d/common-auth
```

I also reviewed authentication-related system logs.

```bash
journalctl -b | grep -i "authentication"

journalctl -b | grep -i "failed"
```

### What I Learned

- Authentication verifies a user's identity.
- Authorization determines what an authenticated user can access or perform.
- `/etc/passwd` stores general Linux account information.
- `/etc/shadow` protects password-related authentication information.
- Passwords are not normally stored as plaintext.
- PAM provides a common authentication framework for Linux applications and services.
- PAM configurations are stored under `/etc/pam.d/`.
- PAM uses different module types for authentication, account management, password management, and sessions.
- Authentication events can provide important information during security investigations.

### Security Perspective

Authentication is one of the fundamental security controls of a Linux system.

Sensitive authentication data must be protected from unauthorized access, and authentication policies should be configured carefully.

PAM configuration changes can affect login and administrative access, so authentication settings should be tested and modified cautiously.

Authentication logs are also important for identifying failed login attempts and investigating suspicious access activity.

### Reflection

#### What did I learn today?

Today I learned how Linux stores account and password-related information and how PAM provides a common authentication framework for Linux applications and services.

#### Why is it important for Cloud Security?

Authentication is the first step in controlling access to Linux and cloud resources.

Understanding the difference between authentication and authorization helps with designing secure access controls and investigating unauthorized access.

#### What will I study next?

Next, I will learn how Linux firewalls control network traffic and reduce unnecessary network exposure.

### Next Step

Linux Firewall Fundamentals

---

# Day 17

## Topic

Linux Firewall Fundamentals

### Objective

Understand how Linux firewalls control network traffic and learn how firewall rules, listening ports, and network services work together to reduce unnecessary network exposure.

### Firewall Fundamentals

A firewall controls network traffic according to defined security rules.

Firewall decisions can be based on information such as:

- Source and destination addresses
- Network protocols
- Source and destination ports
- Traffic direction
- Connection state

A listening port does not automatically mean that a service is reachable from an external network.

Network access may also be restricted by host firewalls, cloud security controls, routing, and other network components.

### Important Concepts

| Concept | Description |
|---|---|
| Inbound Traffic | Network traffic entering a system. |
| Outbound Traffic | Network traffic leaving a system. |
| Accept | Allows matching network traffic. |
| Drop | Silently discards matching traffic. |
| Reject | Blocks matching traffic and may return an error response. |
| Default Deny | A security approach that blocks unnecessary traffic and explicitly allows required traffic. |
| Stateful Firewall | A firewall that can track connection state when applying security policies. |

### Linux Firewall Technologies

| Technology | Description |
|---|---|
| Netfilter | Linux kernel infrastructure used for network packet processing and filtering. |
| nftables | A modern Linux framework for configuring packet filtering rules. |
| iptables | A traditional command and rule system widely used for Linux firewall management. |
| UFW | A simplified frontend for managing firewall policies. |

### Commands

| Command | Description | Example |
|---|---|---|
| `ss -tuln` | Displays listening TCP and UDP sockets. | `ss -tuln` |
| `ss -tulpn` | Displays listening sockets with process information when permitted. | `sudo ss -tulpn` |
| `nft list ruleset` | Displays the current nftables ruleset. | `sudo nft list ruleset` |
| `iptables -L` | Lists iptables filter rules. | `sudo iptables -L -n -v` |
| `ufw status` | Displays UFW firewall status and rules. | `sudo ufw status verbose` |

### Hands-on Lab

I first identified the firewall tools available in my Linux environment.

```bash
which nft
which iptables
which ufw
```

I then inspected the current firewall configuration without modifying or deleting existing rules.

```bash
sudo nft list ruleset

sudo iptables -L -n -v
```

I also inspected listening network services.

```bash
ss -tuln

sudo ss -tulpn
```

### Listening Port Lab

I created a temporary local HTTP service to understand the relationship between an application and a listening port.

```bash
mkdir -p ~/day17-lab
cd ~/day17-lab

python3 -m http.server 8080 --bind 127.0.0.1
```

From another terminal, I verified the listening socket and tested the service.

```bash
ss -tuln | grep 8080

curl http://127.0.0.1:8080
```

After the test, I stopped the temporary HTTP server.

### Firewall Policy Exercise

I designed a basic firewall policy for a hypothetical Linux web server.

Required services:

```text
SSH    TCP/22
HTTP   TCP/80
HTTPS  TCP/443
```

Example security approach:

```text
SSH
→ Allow only from an administrative network

HTTP
→ Allow required client traffic

HTTPS
→ Allow required client traffic

Other unnecessary inbound traffic
→ Deny
```

This exercise demonstrated the Principle of Least Privilege at the network level.

### Cloud Security Connection

Linux host firewalls and cloud network security controls can work together.

```text
Internet
    ↓
Cloud Network Security Control
    ↓
Security Group
    ↓
Linux Host Firewall
    ↓
Listening Service
    ↓
Authentication
    ↓
Authorization
```

Using multiple security controls provides Defense in Depth and reduces reliance on a single protection mechanism.

### What I Learned

- Firewalls control network traffic according to security rules.
- A listening port does not necessarily mean that a service is externally reachable.
- Inbound and outbound traffic represent different traffic directions.
- Firewall rules can use addresses, protocols, ports, and connection state.
- Linux provides technologies such as Netfilter, nftables, and iptables for packet filtering.
- Unnecessary inbound network access should be restricted.
- Cloud-level and host-level network security controls can complement each other.
- Firewall configuration should follow the Principle of Least Privilege.

### Security Perspective

Exposing unnecessary network services increases the attack surface of a Linux server.

Security engineers should identify required services, inspect listening ports, review firewall policies, and restrict network access to only what is necessary.

Host firewalls should be considered together with cloud network controls, service configuration, authentication, and monitoring as part of a Defense in Depth strategy.

### Reflection

#### What did I learn today?

Today I learned how Linux firewalls control network traffic and how listening services, firewall rules, and network security controls interact.

#### Why is it important for Cloud Security?

Cloud workloads are frequently exposed to networks with different trust levels.

Understanding host firewalls and network access controls helps reduce unnecessary exposure and provides another security layer in addition to cloud network controls such as Security Groups.

#### What will I study next?

Next, I will apply the authentication, privilege, and firewall concepts from this week to secure SSH access.

### Next Step

SSH Hardening

---

# Day 18

## Topic

SSH Hardening

### Objective

Understand common SSH security risks and learn how to review SSH service configuration, authentication methods, network exposure, key permissions, and logs.

### SSH Hardening Fundamentals

SSH provides secure remote administration for Linux systems, but an exposed SSH service can also become part of the system's attack surface.

SSH hardening should consider multiple security controls rather than relying on a single configuration setting.

```text
Network Access
      ↓
SSH Service
      ↓
Authentication
      ↓
Linux User
      ↓
Privilege Management
      ↓
System Resources
```

### Important SSH Security Settings

| Setting | Purpose |
|---|---|
| `PermitRootLogin` | Controls whether root can authenticate directly through SSH. |
| `PasswordAuthentication` | Controls SSH password authentication. |
| `PubkeyAuthentication` | Controls public key authentication. |
| `PermitEmptyPasswords` | Controls whether accounts with empty passwords can authenticate. |
| `MaxAuthTries` | Limits authentication attempts within an SSH connection. |
| `AllowUsers` / `AllowGroups` | Can restrict SSH access to selected users or groups. |
| `X11Forwarding` | Controls SSH X11 forwarding functionality. |

### Commands

| Command | Description |
|---|---|
| `systemctl status ssh` | Checks the SSH service status. |
| `ss -tulpn` | Displays listening sockets and associated processes when permitted. |
| `sshd -t` | Checks the SSH server configuration for syntax errors. |
| `sshd -T` | Displays the effective SSH server configuration. |
| `journalctl -u ssh` | Displays logs associated with the SSH service. |
| `nft list ruleset` | Displays the current nftables ruleset. |

### Effective SSH Configuration

I inspected the SSH server configuration and compared configuration files with the effective configuration interpreted by sshd.

```bash
sudo less /etc/ssh/sshd_config

ls -la /etc/ssh/sshd_config.d/

sudo sshd -T
```

I reviewed several security-related settings.

```bash
sudo sshd -T | grep -E '^(permitrootlogin|passwordauthentication|pubkeyauthentication|permitemptypasswords|maxauthtries|x11forwarding)'
```

This helped me understand the difference between reading a configuration file and verifying the configuration actually interpreted by the service.

### SSH Key Security

I reviewed the permissions of my SSH directory and key files.

```bash
ls -ld ~/.ssh
ls -la ~/.ssh
```

Private keys should be protected from unauthorized access.

Public keys are designed to be shared with systems where authentication is required, while private keys must remain protected by their owner.

### Hands-on Security Review

I performed a basic SSH security review without making unnecessary configuration changes.

```bash
systemctl status ssh

sudo ss -tulpn | grep ':22'

sudo sshd -T | grep -E '^(permitrootlogin|passwordauthentication|pubkeyauthentication|permitemptypasswords|maxauthtries|x11forwarding)'

ls -ld ~/.ssh
ls -la ~/.ssh

sudo nft list ruleset

journalctl -u ssh -n 30
```

I reviewed the following areas:

```text
SSH Service Status
        ↓
Listening Port
        ↓
Effective Configuration
        ↓
Authentication Methods
        ↓
SSH Key Permissions
        ↓
Firewall Exposure
        ↓
Logs
```

### Safe Configuration Changes

I learned that SSH configuration changes should be validated before they are applied.

```bash
sudo sshd -t
```

A safer operational workflow is:

```text
Understand / Backup
        ↓
Modify
        ↓
Validate Syntax
        ↓
Review Effective Configuration
        ↓
Apply Change
        ↓
Test a New SSH Connection
        ↓
Close Existing Session Only After Verification
```

This reduces the risk of accidentally losing remote administrative access.

### Cloud Security Connection

SSH security in a cloud environment involves multiple security layers.

```text
Internet
    ↓
Cloud Network Control
    ↓
Security Group
    ↓
Linux Host Firewall
    ↓
SSH Service
    ↓
Authentication
    ↓
Privilege Management
```

Restricting SSH at the network level and applying secure host configuration provides Defense in Depth.

### What I Learned

- SSH is an important administrative service and also part of a server's attack surface.
- Running SSH does not automatically mean that it is reachable from every network.
- Effective configuration should be verified rather than relying only on configuration file contents.
- Direct root access should be carefully controlled.
- Public key authentication can reduce reliance on reusable passwords when properly implemented.
- SSH private keys must be protected.
- Network restrictions can reduce unnecessary SSH exposure.
- SSH logs provide useful evidence for troubleshooting and security investigations.
- Configuration changes should be validated before being applied.
- Hardening should balance security with operational requirements.

### Security Perspective

SSH hardening requires more than changing the SSH port or disabling a single option.

A secure design combines network restrictions, strong authentication, Least Privilege, secure key management, configuration validation, and monitoring.

These controls reduce the attack surface and limit the impact of compromised credentials or configuration mistakes.

### Reflection

#### What did I learn today?

Today I learned how to perform a basic SSH security review by examining the service status, listening ports, effective configuration, authentication methods, SSH key permissions, firewall exposure, and logs.

#### Why is it important for Cloud Security?

SSH is commonly used to administer Linux-based cloud workloads.

Understanding how to restrict and monitor administrative access is important for protecting cloud servers from unauthorized access.

#### What will I study next?

Next, I will learn how cryptographic hashing can be used to verify file integrity and identify unexpected file changes.

### Next Step

File Integrity and Hashing

---

# Day 19

## Topic

File Integrity and Hashing

### Objective

Understand how cryptographic hashing can be used to verify file integrity and detect unexpected changes to important Linux files.

### File Integrity

File integrity refers to maintaining confidence that data has not been modified in an unauthorized or unexpected way.

Cryptographic hashes can be used to compare the current state of a file with a previously trusted state.

```text
Trusted File
     ↓
SHA-256
     ↓
Baseline Hash

Current File
     ↓
SHA-256
     ↓
Current Hash

Compare
  │
  ├── Same → No detected content change
  │
  └── Different → File changed
```

A hash difference indicates that the file contents changed, but it does not by itself prove malicious activity.

### Hashing vs Encryption

| Concept | Primary Purpose |
|---|---|
| Encryption | Protect data confidentiality using cryptographic keys. |
| Hashing | Produce a fixed-size representation that can be used for integrity verification and other security purposes. |

Cryptographic hashing is not designed to be reversed like encryption.

### Commands

| Command | Description | Example |
|---|---|---|
| `sha256sum` | Calculates the SHA-256 hash of a file. | `sha256sum important.txt` |
| `sha256sum -c` | Verifies files against previously stored SHA-256 values. | `sha256sum -c hashes.sha256` |
| `stat` | Displays detailed file metadata and timestamps. | `stat important.txt` |
| `ls -l` | Displays file permissions, ownership, size, and modification information. | `ls -l important.txt` |

### Hands-on Lab

I created a test file and calculated its SHA-256 hash.

```bash
mkdir -p ~/day19-lab
cd ~/day19-lab

echo "Cloud Security Study" > important.txt

sha256sum important.txt
```

I then created a trusted hash baseline.

```bash
sha256sum important.txt > hashes.sha256

cat hashes.sha256

sha256sum -c hashes.sha256
```

After modifying the file, I performed the integrity check again.

```bash
echo "Modified content" >> important.txt

sha256sum -c hashes.sha256
```

The verification detected that the file no longer matched the trusted baseline.

### Multiple File Integrity Check

I also created a baseline for multiple files.

```bash
echo "SSH configuration test" > ssh-config.txt
echo "Firewall configuration test" > firewall.txt
echo "Cron configuration test" > cron.txt

sha256sum ssh-config.txt firewall.txt cron.txt > baseline.sha256

sha256sum -c baseline.sha256
```

After modifying one file, the integrity check identified which file had changed.

### File Metadata

I inspected file metadata using:

```bash
stat important.txt
```

File timestamps and metadata can provide additional context when investigating a detected change.

A cryptographic hash and file metadata provide different types of evidence and can be analyzed together.

### File Integrity Monitoring

A simplified File Integrity Monitoring workflow can be represented as:

```text
Important Files
      ↓
Create Trusted Baseline
      ↓
Monitor Current State
      ↓
Compare
      ↓
Change Detected
      ↓
Investigate
```

The integrity baseline itself must also be protected and trusted.

### Security Perspective

Important Linux files may include account, privilege, remote access, and scheduled task configuration.

Examples include:

```text
/etc/passwd
/etc/shadow
/etc/sudoers
/etc/ssh/sshd_config
/etc/crontab
```

Unexpected modifications to sensitive files should be investigated.

However, a changed hash does not automatically indicate an attack.

Legitimate software updates, administrator actions, configuration changes, and automation can also modify files.

Security analysis therefore requires additional context such as timestamps, logs, users, processes, and change history.

### Python Practice

I used Python's `hashlib` module to calculate the SHA-256 hash of a file.

```python
import hashlib

filename = "important.txt"

with open(filename, "rb") as file:
    data = file.read()

file_hash = hashlib.sha256(data).hexdigest()

print("SHA-256:", file_hash)
```

This demonstrated how file integrity checking can later be automated using Python.

### What I Learned

- Integrity is one of the fundamental security properties in the CIA Triad.
- Cryptographic hashes can be used to identify file content changes.
- SHA-256 produces a 256-bit hash value.
- A trusted baseline can be used to verify files later.
- `sha256sum -c` can automatically compare files against stored hashes.
- File metadata provides additional investigation context.
- A changed hash proves that the checked content differs from the baseline, not why it changed.
- File Integrity Monitoring can help identify unexpected changes to security-sensitive files.
- Integrity baselines must themselves be protected from unauthorized modification.
- Python can be used to automate file integrity checks.

### Reflection

#### What did I learn today?

Today I learned how cryptographic hashes can be used to create trusted file baselines and detect changes to Linux files.

I also learned that detecting a change is only the beginning of a security investigation.

#### Why is it important for Cloud Security?

Cloud workloads depend on operating system, application, and security configuration files.

Detecting unexpected changes can help identify configuration drift, unauthorized modifications, and suspicious activity.

#### What will I study next?

Next, I will learn how to perform basic Linux security auditing by combining information about users, privileges, services, networking, and system configuration.

### Next Step

Basic Linux Security Auditing

---

# Day 20

## Topic

Basic Linux Security Auditing

### Objective

Perform a basic Linux security audit by combining previously learned concepts such as user management, privileges, file permissions, services, networking, firewalls, SSH, scheduled tasks, logging, and file integrity.

The goal of this exercise is not only to execute commands, but also to interpret system information from a security perspective.

### Security Audit Methodology

A basic security audit can follow the process:

```text
Collect
   ↓
Analyze
   ↓
Identify Findings
   ↓
Evaluate Risk
   ↓
Recommend
   ↓
Document
```

Security findings should be evaluated in context rather than automatically classified as vulnerabilities.

### Audit Areas

| Area | Security Objective |
|---|---|
| System Information | Identify the system being reviewed. |
| User Accounts | Identify unexpected or unnecessary accounts. |
| Privileges | Review administrative access and Least Privilege. |
| File Permissions | Identify unnecessarily permissive access. |
| SUID Files | Review executables that may run with elevated effective privileges. |
| Services | Identify unnecessary running or enabled services. |
| Network | Identify listening services and network exposure. |
| Firewall | Review network filtering controls. |
| SSH | Review secure remote administration configuration. |
| Scheduled Tasks | Identify privileged or unnecessary automated tasks. |
| Authentication | Review account and authentication configuration. |
| Logs | Identify events that may require investigation. |
| File Integrity | Detect unexpected changes to important files. |

### System Information

I identified the Linux system being reviewed.

```bash
hostnamectl
uname -a
cat /etc/os-release
uptime
```

Understanding the target system provides important context for a security assessment.

### User and Privilege Audit

I reviewed Linux accounts and privileged access.

```bash
getent passwd

awk -F: '$7 !~ /(nologin|false)$/ {print $1, $3, $7}' /etc/passwd

awk -F: '$3 == 0 {print $1}' /etc/passwd

sudo -l

getent group sudo
```

UID 0 accounts and administrative privileges should be reviewed to identify unnecessary or unexpected privileged access.

### File Permission Audit

I reviewed permissions on security-sensitive Linux files.

```bash
stat -c '%A %a %U %G %n' \
/etc/passwd \
/etc/shadow \
/etc/sudoers \
/etc/ssh/sshd_config
```

Sensitive files should only be accessible to users and groups that require access.

### World-Writable File Lab

I created test files with different permissions.

```bash
mkdir -p ~/day20-lab
cd ~/day20-lab

touch normal.txt
touch insecure.txt

chmod 600 normal.txt
chmod 666 insecure.txt
```

I identified world-writable files using:

```bash
find . -type f -perm -0002 -ls
```

A world-writable file can be modified by any local user.

The security impact depends on the purpose of the file and whether its contents influence privileged or security-sensitive operations.

### SUID Audit

I identified SUID executables on the local filesystem.

```bash
find / -xdev -type f -perm -4000 -print 2>/dev/null
```

The presence of a SUID executable does not automatically indicate a vulnerability.

SUID files should be reviewed to determine whether they are expected, required, and securely configured.

### Service Audit

I reviewed running and enabled services.

```bash
systemctl --type=service --state=running

systemctl list-unit-files --type=service --state=enabled
```

Unnecessary services can increase a system's attack surface.

### Network Audit

I reviewed listening network services.

```bash
sudo ss -tulpn
```

For each listening service, security reviews should consider:

```text
Which process owns the port?
        ↓
Is the service required?
        ↓
Which interface is it listening on?
        ↓
Is network access restricted?
```

### Firewall Audit

I reviewed the available host firewall configuration.

```bash
sudo nft list ruleset
```

Depending on the environment, firewall configuration may also be reviewed using tools such as `iptables` or `ufw`.

### SSH Security Audit

I reviewed the SSH service and effective SSH configuration.

```bash
systemctl status ssh

sudo ss -tulpn | grep ':22'

sudo sshd -T | grep -E \
'^(permitrootlogin|passwordauthentication|pubkeyauthentication|permitemptypasswords|maxauthtries|x11forwarding)'
```

SSH security should be evaluated together with authentication methods, privileges, firewall restrictions, and logging.

### Scheduled Task Audit

I reviewed scheduled tasks.

```bash
cat /etc/crontab

ls -la /etc/cron.d/

crontab -l
```

Privileged scheduled tasks should not depend on files or scripts that can be modified by unauthorized users.

### Authentication Audit

I reviewed account and authentication information.

```bash
sudo passwd -S "$(whoami)"

sudo chage -l "$(whoami)"

ls -la /etc/pam.d/
```

Authentication configuration should be reviewed carefully because incorrect changes can affect system access.

### Log Audit

I reviewed system and SSH-related events.

```bash
journalctl -p warning -b

journalctl -u ssh -n 50

journalctl -b | grep -i 'failed'

journalctl -b | grep -i 'sudo'
```

Security-related log events require context before they can be classified as malicious or benign.

### File Integrity

I reviewed file integrity using a previously created SHA-256 baseline.

```bash
sha256sum -c hashes.sha256
```

A changed hash indicates that file contents differ from the trusted baseline, but additional investigation is required to determine why the change occurred.

### Finding Workflow

I practiced documenting a security finding using the following structure:

```text
Finding
   ↓
Evidence
   ↓
Risk
   ↓
Recommendation
   ↓
Remediation
   ↓
Verification
```

Example:

**Finding**

A world-writable test file was identified.

**Evidence**

```bash
find ~/day20-lab -type f -perm -0002 -ls
```

**Risk**

A world-writable file can be modified by any local user. The security impact depends on how the file is used.

**Recommendation**

Restrict write permissions to only the users or groups that require them.

**Remediation**

```bash
chmod 640 ~/day20-lab/insecure.txt
```

**Verification**

```bash
find ~/day20-lab -type f -perm -0002 -ls
```

### Security Audit Checklist

```text
[ ] System information
[ ] User accounts
[ ] UID 0 accounts
[ ] sudo privileges
[ ] Sensitive file permissions
[ ] World-writable files
[ ] SUID files
[ ] Running services
[ ] Enabled services
[ ] Listening ports
[ ] Firewall configuration
[ ] SSH configuration
[ ] Scheduled tasks
[ ] Authentication configuration
[ ] Security-related logs
[ ] File integrity
```

### What I Learned

- Security auditing requires both information collection and analysis.
- A security-related configuration does not automatically represent a vulnerability.
- Privileged accounts should follow the Principle of Least Privilege.
- Sensitive file permissions should be reviewed regularly.
- SUID executables require contextual security analysis.
- Unnecessary services and listening ports can increase the attack surface.
- SSH security depends on multiple controls including network restrictions, authentication, privileges, and logging.
- Scheduled privileged tasks should use securely protected files and scripts.
- Logs provide important context during security investigations.
- File integrity monitoring can identify unexpected changes.
- Findings should include evidence, risk, and actionable recommendations.
- Remediation should be followed by verification.

### Security Perspective

A Linux security audit should evaluate multiple layers of the system rather than relying on a single security control.

```text
Accounts
    ↓
Authentication
    ↓
Privileges
    ↓
Services
    ↓
Network
    ↓
Firewall
    ↓
Applications
    ↓
Logs / Monitoring
```

Combining these areas provides a more complete view of the security posture of a Linux workload.

### Reflection

#### What did I learn today?

Today I learned how to combine Linux administration and security concepts into a structured basic security audit.

Instead of only executing commands, I practiced interpreting system information, identifying potential findings, evaluating their security context, and recommending remediation.

#### Why is it important for Cloud Security?

Cloud workloads frequently run on Linux systems.

Cloud-level security controls such as IAM and Security Groups do not replace operating system security.

Understanding Linux security auditing helps identify risks inside cloud workloads and supports a Defense in Depth security strategy.

#### What will I study next?

Next, I will review the Linux Security Fundamentals topics from this week and summarize the most important security concepts and practical lessons.

### Next Step

Week 3 Security Summary & Review

---

# Day 21

## Topic

Week 3 Security Summary & Review

### Objective

Review the Linux Security Fundamentals covered during Week 3 and apply them together through a structured Linux security review.

The goal of this review is to understand how authentication, privileges, network controls, remote access, file integrity, logging, and security auditing work together to protect a Linux system.

### Week 3 Topics

| Day | Topic |
|---|---|
| Day 15 | sudo and Privilege Management |
| Day 16 | Linux Authentication and PAM |
| Day 17 | Linux Firewall Fundamentals |
| Day 18 | SSH Hardening |
| Day 19 | File Integrity and Hashing |
| Day 20 | Basic Linux Security Auditing |

### Security Concepts Reviewed

| Area | Security Focus |
|---|---|
| Privilege Management | Least Privilege and controlled administrative access |
| Authentication | Identity verification and PAM |
| Firewall | Network access control and attack-surface reduction |
| SSH | Secure remote administration |
| File Integrity | Detection of unexpected file changes |
| Security Auditing | Structured security assessment and documentation |
| Logging | Evidence collection and investigation |

### Integrated Security Review

I performed a basic review of my Linux environment using the security concepts learned during Week 3.

```bash
hostnamectl
uname -a

whoami
id

awk -F: '$3 == 0 {print $1}' /etc/passwd

sudo -l
getent group sudo

ls -l /etc/passwd
ls -l /etc/shadow

sudo ss -tulpn
sudo nft list ruleset

systemctl status ssh

sudo sshd -T | grep -E \
'^(permitrootlogin|passwordauthentication|pubkeyauthentication|permitemptypasswords|maxauthtries|x11forwarding)'

crontab -l
cat /etc/crontab

find / -xdev -type f -perm -4000 -print 2>/dev/null

journalctl -b -p warning
journalctl -u ssh -n 30
```

### Security Review Approach

During the review, I practiced following a structured investigation process.

```text
Identify the Asset
        ↓
Collect Evidence
        ↓
Understand the Configuration
        ↓
Evaluate Security Context
        ↓
Identify Findings
        ↓
Recommend Remediation
        ↓
Verify the Result
```

Security settings should not automatically be classified as vulnerabilities without understanding their purpose and operating context.

### Authentication and Privilege

I learned that authentication and authorization represent different security functions.

```text
Authentication
"Who are you?"
        ↓
Authorization
"What are you allowed to do?"
        ↓
Privileged Action
```

PAM provides an authentication framework for Linux applications, while sudo and permissions help control privileged operations.

### Network and SSH Security

Network security requires multiple layers of control.

```text
Network
    ↓
Cloud / Network Control
    ↓
Host Firewall
    ↓
Listening Service
    ↓
SSH Configuration
    ↓
Authentication
    ↓
Privilege Management
```

A listening port does not automatically mean that a service is reachable from every network.

SSH security should therefore be evaluated together with network exposure, authentication methods, key management, privileges, and logs.

### File Integrity

I reviewed how SHA-256 hashes can be used to compare the current state of a file with a trusted baseline.

```text
Trusted Baseline
        ↓
Current File
        ↓
Hash Comparison
        ↓
Change Detected?
        ↓
Investigation
```

A changed hash indicates that file contents changed but does not explain why the change occurred.

Additional evidence is required to distinguish authorized changes from suspicious activity.

### Security Auditing

I practiced documenting security observations using:

```text
Finding
   ↓
Evidence
   ↓
Risk
   ↓
Recommendation
   ↓
Remediation
   ↓
Verification
```

This helped me understand that a security audit is more than executing commands.

The important part is interpreting the information and explaining the security impact.

### Week 3 Key Takeaways

- Administrative privileges should follow the Principle of Least Privilege.
- Authentication and authorization are separate security functions.
- PAM provides a common authentication framework for Linux applications.
- Unnecessary network exposure increases the attack surface.
- Host firewalls and cloud network controls can provide Defense in Depth.
- SSH hardening requires secure configuration, strong authentication, network restrictions, and monitoring.
- Cryptographic hashes can help detect unexpected file changes.
- A changed file does not automatically indicate malicious activity.
- SUID files and other privileged configurations require contextual analysis.
- Security audits should collect evidence before drawing conclusions.
- Findings should include clear risks and actionable recommendations.
- Remediation should always be followed by verification.

### Security Perspective

Linux security is created by multiple controls working together.

```text
Identity
    ↓
Authentication
    ↓
Authorization
    ↓
Network Access
    ↓
Services
    ↓
System and File Integrity
    ↓
Logging and Monitoring
    ↓
Security Auditing
```

A weakness in one layer can increase risk, while multiple security controls can reduce the impact of individual failures.

This is an important example of Defense in Depth.

### Reflection

#### What did I accomplish this week?

I completed my first dedicated Linux Security Fundamentals week.

I learned how to review privileges, authentication, firewalls, SSH configuration, file integrity, and system security settings from a security perspective.

#### What was the most important lesson?

The most important lesson was that identifying a security-related configuration is not the same as proving that a vulnerability exists.

Security analysis requires evidence, context, risk evaluation, and verification.

#### What was difficult?

I will continue reviewing any Linux security concepts or configuration results that were difficult to interpret during the hands-on exercises.

#### Why is it important for Cloud Security?

Cloud workloads often run on Linux systems.

Cloud-level security controls cannot fully protect a workload if the operating system has insecure privileges, exposed services, weak authentication, or insecure configuration.

Understanding Linux security provides an important foundation for Defense in Depth in cloud environments.

#### What will I study next?

Next, I will begin Linux Troubleshooting and Security Operations by learning how to monitor system resources and identify abnormal system behavior.

### Next Step

Linux Troubleshooting and Security Operations — System Resource Monitoring

---

# Day 22

## Topic

System Resource Monitoring

### Objective

Learn how to monitor Linux system resources and investigate performance problems using CPU, memory, load, disk, and process information.

The goal is to develop a structured troubleshooting approach based on evidence rather than immediately changing system configuration or restarting services.

### Troubleshooting Methodology

A basic troubleshooting process can follow:

```text
Problem
   ↓
Observe
   ↓
Collect Evidence
   ↓
Identify Resource
   ↓
Identify Process
   ↓
Investigate Cause
   ↓
Take Action
   ↓
Verify
```

Stopping a problematic process may remove a symptom, but additional investigation may still be required to identify the root cause.

### System Load

I reviewed system uptime and load average.

```bash
uptime
```

Load average represents system load over approximately 1, 5, and 15 minute periods.

It should be interpreted together with CPU count, CPU utilization, workload characteristics, and other system information.

```bash
nproc
lscpu
```

Load average is not the same as CPU utilization.

### CPU and Process Monitoring

I used `top` to monitor system and process activity.

```bash
top
```

Important information includes:

- Load average
- CPU utilization
- Memory usage
- Swap usage
- Process ID
- Process owner
- CPU usage
- Memory usage
- Command

I also identified processes consuming the most CPU and memory.

```bash
ps aux --sort=-%cpu | head

ps aux --sort=-%mem | head
```

### Memory Monitoring

I reviewed system memory usage.

```bash
free -h
```

Linux may use available memory for caching, so low `free` memory alone does not necessarily indicate memory exhaustion.

The `available` value and overall system behavior should also be considered.

I also reviewed swap configuration.

```bash
swapon --show
```

### Process Investigation

After identifying a process of interest, I reviewed additional process information.

```bash
ps -fp <PID>

cat /proc/<PID>/status

readlink -f /proc/<PID>/exe

tr '\0' ' ' < /proc/<PID>/cmdline

ps -o pid,ppid,user,%cpu,%mem,cmd -p <PID>
```

Process information should be evaluated together with its owner, executable, command line, parent process, resource usage, and operational context.

### `/proc` Filesystem

I explored the Linux `/proc` virtual filesystem.

```bash
echo $$

ls /proc/$$

cat /proc/$$/status

tr '\0' ' ' < /proc/$$/cmdline

readlink -f /proc/$$/exe
```

The `/proc` filesystem exposes information about running processes and the Linux kernel.

### CPU Troubleshooting Lab

I created a temporary CPU-intensive process.

```bash
yes > /dev/null
```

From another terminal, I identified the process using:

```bash
top

ps aux --sort=-%cpu | head
```

After identifying its PID, I collected additional evidence.

```bash
ps -fp <PID>

cat /proc/<PID>/status

readlink -f /proc/<PID>/exe

tr '\0' ' ' < /proc/<PID>/cmdline
```

I then terminated the test process.

```bash
kill <PID>
```

Finally, I verified that the process was no longer running and reviewed the system state again.

```bash
ps -p <PID>

top

uptime
```

This demonstrated the troubleshooting process:

```text
Detect
   ↓
Identify
   ↓
Investigate
   ↓
Remediate
   ↓
Verify
```

### Disk Monitoring

I performed basic disk and inode checks.

```bash
df -h

df -i
```

Disk exhaustion can affect applications, databases, logging, and other system services.

### Security Perspective

High resource usage does not automatically indicate malicious activity.

Unexpected CPU, memory, disk, or process activity should be investigated using additional context.

```text
Resource Anomaly
       ↓
Identify Process
       ↓
Process Owner
       ↓
Executable
       ↓
Command Line
       ↓
Parent Process
       ↓
Logs / Network Activity
       ↓
Expected or Unexpected?
```

This approach helps distinguish normal workload behavior, operational problems, misconfiguration, and potentially suspicious activity.

### System Resource Checklist

```text
[ ] System uptime
[ ] Load average
[ ] CPU count
[ ] CPU utilization
[ ] Memory usage
[ ] Swap usage
[ ] Disk space
[ ] Inode usage
[ ] High CPU processes
[ ] High memory processes
[ ] Process owner
[ ] Process executable
[ ] Process command line
[ ] Parent process
```

### Python Practice

I used Python to retrieve information about the running Python process from `/proc`.

```python
import os

pid = os.getpid()

print("Python PID:", pid)

status_file = f"/proc/{pid}/status"

with open(status_file, "r") as file:
    for line in file:
        if line.startswith(("Name:", "Pid:", "PPid:", "VmRSS:")):
            print(line.strip())
```

This demonstrated how Python can be used to collect Linux process information for future security and monitoring automation.

### Cloud Security Connection

Cloud monitoring and operating system monitoring provide different layers of visibility.

```text
Cloud Monitoring
       ↓
Instance Metrics
       ↓
Linux System
       ↓
Process Investigation
       ↓
Root Cause Analysis
```

Understanding both layers is useful when investigating performance or security issues affecting cloud workloads.

### What I Learned

- Troubleshooting should begin with observation and evidence collection.
- Load average and CPU utilization represent different system characteristics.
- CPU count should be considered when interpreting system load.
- Linux memory usage should not be evaluated using only the `free` value.
- `top` and `ps` can identify resource-intensive processes.
- `/proc` provides detailed information about processes and the kernel.
- Process owner, executable, command line, and parent process provide useful investigation context.
- Disk and inode exhaustion can cause application and system problems.
- High resource usage does not automatically indicate malicious activity.
- Terminating a process may remove a symptom without identifying the root cause.
- Remediation should be followed by verification.

### Reflection

#### What did I learn today?

Today I learned how to monitor Linux system resources and investigate high resource usage using system and process information.

I also practiced identifying a CPU-intensive process, collecting evidence about it, terminating it, and verifying the result.

#### Why is it important for Cloud Security?

Performance anomalies can result from normal workloads, configuration problems, software defects, or potentially suspicious activity.

Understanding Linux resource and process monitoring helps investigate problems inside cloud workloads instead of relying only on cloud-level metrics.

#### What will I study next?

Next, I will learn how to troubleshoot disk usage, filesystems, and storage-related problems.

### Next Step

Disk and Filesystem Troubleshooting

---

# Vocabulary

| Term | Meaning |
|------|---------|
| Absolute Path | The complete path to a file or directory starting from the root directory. |
| APT | A package management tool commonly used on Debian-based Linux systems. |
| Attack Surface | The systems, services, interfaces, and other entry points that could potentially be targeted by an attacker. |
| Attack Surface Reduction | The practice of reducing unnecessary services, access paths, and functionality that could potentially be targeted. |
| Audit Log | A record used to track important actions and changes for accountability and investigation. |
| Authentication | The process of verifying the identity of a user or system. |
| Authorization | The process of determining what an authenticated identity is allowed to access or perform. |
| Baseline | A trusted reference state used for later comparison. |
| Bottleneck | A resource or component that limits overall system performance. |
| Centralized Logging | Collecting logs from multiple systems into a central location for monitoring and analysis. |
| Checksum | A value used to help verify data integrity; cryptographic hashes can serve this role when cryptographic properties are required. |
| Child Process | A process created by another process that can inherit parts of its environment. |
| Configuration Drift | A change in a system's configuration from its intended or approved state. |
| Configuration File | A file that stores system settings. |
| Configuration Validation | The process of checking a configuration for correctness before applying it. |
| CPU Utilization | The proportion of CPU capacity being used for processing work. |
| Cron | A Linux service used to execute scheduled commands and scripts. |
| Crontab | A configuration that defines scheduled cron jobs for a user or system. |
| Cryptographic Hash | A fixed-size value produced from input data by a cryptographic hash function. |
| Daemon | A background process running without direct user interaction. |
| Default Deny | A security approach that blocks access by default and explicitly permits required traffic. |
| Default Gateway | The router that forwards traffic to other networks. |
| Defense in Depth | A security strategy that uses multiple layers of controls instead of relying on a single protection mechanism. |
| Dependency | Software required by another program or package to function correctly. |
| Directory | A folder used to organize files. |
| Effective Configuration | The configuration actually interpreted and applied by a service after its configuration sources are processed. |
| Environment Variable | A named value used to provide configuration information to processes. |
| Evidence | Information used to support a security finding or investigation. |
| Execute | Permission to run a file or program. |
| Export | Makes a shell variable available to child processes. |
| File | A collection of data stored on disk. |
| File Integrity Monitoring | The process of monitoring files for unexpected changes. |
| Firewall | A security control that permits or blocks network traffic according to defined rules. |
| GID | Group Identifier. |
| Grep | A command-line tool used to search text for matching patterns. |
| Group | A collection of users who share permissions. |
| Hardening | The process of reducing security risk by securely configuring a system and disabling or restricting unnecessary functionality. |
| Home Directory | A user's personal working directory. |
| Hostname | The name assigned to a computer on a network. |
| Inbound Traffic | Network traffic entering a system or network. |
| Integrity | The security property of maintaining confidence that data has not been improperly modified. |
| Investigation | The process of examining system information and evidence to understand an event or problem. |
| IP Address | A unique address assigned to a device on a network. |
| Journal | The systemd logging system that stores and manages system events. |
| Least Privilege | A security principle that grants only the permissions required to perform a task. |
| Load Average | A Linux metric representing the average system load over a period of time. |
| Log | A record of an event generated by a system, service, or application. |
| Log Retention | The period of time logs are stored before deletion or archival. |
| Network Interface | A hardware or virtual interface used for network communication. |
| Outbound Traffic | Network traffic leaving a system or network. |
| Owner | The user who owns a file or directory. |
| Package | A bundled collection of software and related metadata. |
| Package Repository | A source from which software packages can be downloaded and installed. |
| PAM | Pluggable Authentication Modules, a framework used by Linux applications and services for authentication and related account operations. |
| Password Hash | A derived representation used as part of password verification instead of storing the plaintext password. |
| Patch | An update intended to fix bugs, vulnerabilities, or other software issues. |
| PATH | An environment variable containing directories used to locate executable commands. |
| Permission | Controls access to files and directories. |
| Persistence | A technique used to maintain access to a system over time. |
| PID | A unique process identifier assigned to a running process. |
| Ping | A utility used to test network connectivity. |
| Pipe | A mechanism that passes the output of one command as input to another command. |
| Port | A communication endpoint used by network services. |
| PPID | The process identifier of a process's parent. |
| Priority | A severity level assigned to a log event. |
| Private Key | A secret cryptographic key that must be protected by its owner. |
| Privilege Escalation | The process of gaining permissions beyond those originally authorized. |
| Process | A running instance of a program. |
| Process Monitoring | Observing running processes to maintain system health and security. |
| Public Key | A cryptographic key that can be shared and used with its corresponding private key. |
| Public Key Authentication | An authentication method that verifies possession of a corresponding private key. |
| Remediation | An action taken to correct or reduce an identified security risk. |
| Resource Monitoring | The process of observing CPU, memory, disk, and other system resources. |
| Root Cause | The underlying reason that caused a problem or abnormal condition. |
| Root Directory | The top-level directory in Linux. |
| Root User | The Linux superuser account with UID 0 and highly privileged system access. |
| Routing Table | A table that determines how network packets are forwarded. |
| Scheduled Task | A command or program configured to run automatically at a specified time or interval. |
| Security Assessment | A structured evaluation of a system's security controls, configuration, and potential risks. |
| Security Audit | A structured review of a system's configuration, controls, and security posture. |
| Security Context | The surrounding technical and operational information required to correctly interpret a security observation. |
| Security Finding | An observed condition that may require security review or remediation. |
| Security Posture | The overall state of an organization's or system's security controls and risks. |
| Service | A background program managed by the operating system. |
| Session | A period of interaction between an authenticated user and a system or service. |
| SHA-256 | A cryptographic hash function that produces a 256-bit hash value. |
| Shell | A program that interprets commands and interacts with the operating system. |
| Shell Variable | A variable that exists within the current shell and is not automatically inherited by child processes. |
| Socket | An endpoint for network communication. |
| SSH Client | A program that initiates an SSH connection to a remote system. |
| SSH Server | A service that accepts and manages incoming SSH connections. |
| SSH | Secure Shell, a protocol used for encrypted remote access. |
| Standard Input | Data received by a command or process. |
| Standard Output | Data produced by a command or process. |
| Stateful Firewall | A firewall that tracks connection state when applying traffic rules. |
| sudo | A mechanism that allows authorized users to execute commands with another user's privileges. |
| sudoers | Configuration that defines which users or groups can execute commands through sudo. |
| SUID | A special Linux permission that can cause an executable to run with the effective user ID of its file owner. |
| Superuser | A user account with highly privileged administrative access to a system. |
| Supply Chain Security | The practice of protecting software and its dependencies throughout the development and distribution process. |
| Terminal | A command-line interface used to interact with Linux. |
| TCP | A reliable connection-oriented network protocol. |
| Troubleshooting | A systematic process used to identify and resolve the cause of a technical problem. |
| UDP | A connectionless network protocol with low overhead. |
| UID | User Identifier. |
| Verification | The process of confirming that remediation or a security control works as intended. |
| Wildcard | A symbol used to represent one or more characters when matching file names. |
| World-Writable | A permission state that allows all users to modify a file or directory. |
| `/proc` | A Linux virtual filesystem that exposes process and kernel information. |
