# Linux Notes

My personal Linux study notes and hands-on labs for Cloud Security.

---

## Goal

- Learn Linux fundamentals
- Practice Linux commands
- Build Cloud Security skills

---

## Learning Progress

- [x] Basic Linux commands
- [ ] Linux File System
- [ ] File Permissions
- [ ] Users & Groups
- [ ] Processes
- [ ] Services
- [ ] Networking
- [ ] Shell Scripting

---

## Commands Learned

| Command | Description |
|----------|-------------|
| pwd | Print current working directory |
| ls | List files and directories |
| cd | Change directory |
| mkdir | Create directory |
| touch | Create a file |
| cp | Copy files |
| mv | Move or rename files |
| rm | Remove files |
| cat | Display file contents |

---

## What I Learned Today

### Day 1

- Learned basic Linux commands.
- Created my first GitHub repository.
- Learned how to navigate directories.

### Day 2

- Learned the Linux directory structure.
- Understood the purpose of `/home`, `/etc`, `/var`, `/usr`, and `/tmp`.
- Practiced moving between directories.

---

## Directory Structure

| Directory | Purpose |
|-----------|----------|
| / | Root directory |
| /home | User home directories |
| /etc | System configuration files |
| /var | Logs and variable data |
| /usr | User applications |
| /tmp | Temporary files |

---

## Day 3

### Topic

Linux File Permissions

### Why File Permissions Matter

Linux file permissions control who can read, modify, or execute a file.
Proper permissions help prevent unauthorized access and accidental changes.

### Permission Types

- `r` — Read
- `w` — Write
- `x` — Execute

Permissions are assigned to:

- Owner
- Group
- Others

### Hands-on Lab

| File | Permission | Purpose |
|---|---:|---|
| `private.txt` | `600` | Only the owner can read and modify it |
| `shared.txt` | `644` | Everyone can read it, but only the owner can modify it |
| `script.sh` | `755` | Everyone can execute it, but only the owner can modify it |

### Commands Used

```bash
chmod 600 private.txt
chmod 644 shared.txt
chmod 755 script.sh
ls -l
