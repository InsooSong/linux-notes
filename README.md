# Linux Notes

> 🚀 This repository documents my Linux learning journey for Cloud Security.  
> My goal is to build strong Linux fundamentals and prepare for a Cloud Security Engineer role in Australia or Canada.

---

# Goal

- Learn Linux fundamentals.
- Build practical Linux skills for Cloud Security.
- Practice Linux administration through hands-on labs.
- Document my learning journey with GitHub.
- Prepare for Cloud Security Engineer roles in Australia or Canada.

---

# Learning Progress

| Status | Day | Topic |
|--------|-----|-----------------------------|
| ✅ | Day 1 | Linux Basic Commands |
| ✅ | Day 2 | Linux Directory Structure |
| ✅ | Day 3 | Linux File Permissions |
| ✅ | Day 4 | Linux Users and Groups |
| ⏳ | Day 5 | Linux Processes and Services |
| ⏳ | Day 6 | SSH and Remote Access |
| ⏳ | Day 7 | Weekly Review |

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
