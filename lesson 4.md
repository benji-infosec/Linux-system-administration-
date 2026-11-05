# Lesson 4: Monitoring Processes & Access Control

## 🎯 Objective
Learn how to use interactive process viewers, filter active processes using pattern matching, inspect shell Process IDs (PIDs), and manage basic file and directory permissions in a Linux environment.

## 💻 Execution Workflow
Open your Termux terminal, log into Ubuntu 
```bash
proot-distro login ubuntu

```
and execute the following commands:
### Step 1 — Display All Running Processes
List all active processes running on the system with detailed user and CPU/memory statistics:
```bash
ps aux

```
### Step 2 — Search for a Specific Process or Service
Use ps aux combined with grep to filter and find lines matching a specific process (such as bash):
```bash
ps aux | grep bash

```
### Step 3 — Monitor Processes in Real-Time
Open the interactive process viewer to monitor active task and resource consumption continuously:
```bash
top

```
*(To exit the top monitor, press q)*. *(Note: If top is unavailable, you can install it using apt update && apt install procps -y)*.
### Step 4 — Check Your Current Shell Process ID
Display the Process ID (PID) of your active Bash shell session:
```bash
echo $$

```
### Step 5 — Manage File & Directory Permissions
Inspect file permission strings and modify access control using chmod:
```bash
# View file permissions in long listing format
ls -l

# Restrict file access to owner read/write only
chmod 600 sensitive_config.txt

# Set directory permissions (owner full control, others read/execute)
chmod 755 project_dir/

