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
| ✅ | Day 8 | SSH and Remote Access |
| ✅ | Day 9 | Package Management |
| ✅ | Day 10 | Shell and Environment Variables |
| ✅ | Day 11 | File Search and Text Processing |
| ✅ | Day 12 | Log Files |
| ✅ | Day 13 | Cron Jobs |
| ⏳ | Day 14 | Weekly Summary & Review |

---

## Week 3 - Linux Security Fundamentals

### Goal

- Understand fundamental Linux security concepts.
- Learn how authentication, privileges, and network controls protect Linux systems.
- Build practical security skills for managing cloud-based Linux servers.

| Status | Day    | Topic                              |
| ------ | ------ | ---------------------------------- |
| ⏳      | Day 15 | sudo and Privilege Management      |
| ⏳      | Day 16 | Linux Authentication and PAM       |
| ⏳      | Day 17 | Linux Firewall Fundamentals        |
| ⏳      | Day 18 | SSH Hardening                      |
| ⏳      | Day 19 | File Integrity and Hashing         |
| ⏳      | Day 20 | Basic Linux Security Auditing      |
| ⏳      | Day 21 | Weekly Summary & Review            |

---

## Week 4 - Linux Troubleshooting and Security Operations

### Goal

- Learn how to troubleshoot common Linux system and network problems.
- Develop basic Linux security investigation skills.
- Apply Linux knowledge through practical system and security analysis.

| Status | Day    | Topic                                  |
| ------ | ------ | -------------------------------------- |
| ⏳      | Day 22 | System Resource Monitoring             |
| ⏳      | Day 23 | Network Troubleshooting                |
| ⏳      | Day 24 | Service Troubleshooting with systemd   |
| ⏳      | Day 25 | Security Log Analysis                  |
| ⏳      | Day 26 | Bash Scripting Fundamentals            |
| ⏳      | Day 27 | Linux Security Audit Mini Project      |
| ⏳      | Day 28 | Monthly Summary & Review               |

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

# Vocabulary

| Term | Meaning |
|------|---------|
| Absolute Path | The complete path to a file or directory starting from the root directory. |
| APT | A package management tool commonly used on Debian-based Linux systems. |
| Audit Log | A record used to track important actions and changes for accountability and investigation. |
| Authentication | The process of verifying the identity of a user or system. |
| Centralized Logging | Collecting logs from multiple systems into a central location for monitoring and analysis. |
| Child Process | A process created by another process that can inherit parts of its environment. |
| Configuration File | A file that stores system settings. |
| Cron | A Linux service used to execute scheduled commands and scripts. |
| Crontab | A configuration that defines scheduled cron jobs for a user or system. |
| Daemon | A background process running without direct user interaction. |
| Default Gateway | The router that forwards traffic to other networks. |
| Dependency | Software required by another program or package to function correctly. |
| Directory | A folder used to organize files. |
| Environment Variable | A named value used to provide configuration information to processes. |
| Execute | Permission to run a file or program. |
| Export | Makes a shell variable available to child processes. |
| File | A collection of data stored on disk. |
| GID | Group Identifier. |
| Grep | A command-line tool used to search text for matching patterns. |
| Group | A collection of users who share permissions. |
| Home Directory | A user's personal working directory. |
| Hostname | The name assigned to a computer on a network. |
| IP Address | A unique address assigned to a device on a network. |
| Journal | The systemd logging system that stores and manages system events. |
| Log | A record of an event generated by a system, service, or application. |
| Log Retention | The period of time logs are stored before deletion or archival. |
| Network Interface | A hardware or virtual interface used for network communication. |
| Owner | The user who owns a file or directory. |
| Package | A bundled collection of software and related metadata. |
| Package Repository | A source from which software packages can be downloaded and installed. |
| Patch | An update intended to fix bugs, vulnerabilities, or other software issues. |
| PATH | An environment variable containing directories used to locate executable commands. |
| Permission | Controls access to files and directories. |
| Persistence | A technique used to maintain access to a system over time. |
| PID | Process Identifier. |
| Ping | A utility used to test network connectivity. |
| Pipe | A mechanism that passes the output of one command as input to another command. |
| Port | A communication endpoint used by network services. |
| Priority | A severity level assigned to a log event. |
| Private Key | A secret cryptographic key that must be protected by its owner. |
| Process | A running instance of a program. |
| Process Monitoring | Observing running processes to maintain system health and security. |
| Public Key | A cryptographic key that can be shared and used with its corresponding private key. |
| Root Directory | The top-level directory in Linux. |
| Root User | The superuser with unrestricted privileges. |
| Routing Table | A table that determines how network packets are forwarded. |
| Scheduled Task | A command or program configured to run automatically at a specified time or interval. |
| Service | A background program managed by the operating system. |
| Shell | A program that interprets commands and interacts with the operating system. |
| Shell Variable | A variable that exists within the current shell and is not automatically inherited by child processes. |
| Socket | An endpoint for network communication. |
| SSH Client | A program that initiates an SSH connection to a remote system. |
| SSH Server | A service that accepts and manages incoming SSH connections. |
| SSH | Secure Shell, a protocol used for encrypted remote access. |
| Standard Input | Data received by a command or process. |
| Standard Output | Data produced by a command or process. |
| sudo | Executes commands with administrator privileges. |
| Supply Chain Security | The practice of protecting software and its dependencies throughout the development and distribution process. |
| Terminal | A command-line interface used to interact with Linux. |
| TCP | A reliable connection-oriented network protocol. |
| UDP | A connectionless network protocol with low overhead. |
| UID | User Identifier. |
| Wildcard | A symbol used to represent one or more characters when matching file names. |
