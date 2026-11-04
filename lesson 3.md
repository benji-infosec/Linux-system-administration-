Let's dive right into **Project 3, Lesson 3: Managing Running Processes & Services**!
In system administration and IT support, knowing how to inspect active tasks, track down resource hogs, and manage running services is an essential everyday skill.
# Lesson 3: Managing Running Processes & Services
## 🎯 Objective
Learn how to list active processes, monitor system execution in real-time, locate specific services using pattern matching, and safely terminate misbehaving or unnecessary processes.
## 💻 Execution Workflow
Open your Termux terminal, log into Ubuntu 
```bash
proot-distro login ubuntu

```
and run the following process management commands:
### Step 1 — View All Running Processes
List all active processes running on the system with detailed user and CPU/memory statistics:
```bash
ps aux

```
### Step 2 — Search for a Specific Process or Service
Use pgrep combined with ps or grep to find the Process ID (PID) of a specific service or command (for example, checking active bash shells):
```bash
pgrep -l bash

```
### Step 3 — Terminate a Process (Demonstration / Safe Practice)
*(Note: Do not kill your active shell session!)* If you need to stop a hanging or background process, you reference its Process ID (PID):
```bash
# General syntax to terminate a process gracefully (SIGTERM)
kill <PID>

# Force-terminate a stubborn process if necessary (SIGKILL)
kill -9 <PID>

```
## 📸 Lesson 3 Evidence & Screenshots
I take a screenshot showing the process monitoring command output and save it inside your screenshots/ folder:
 * **File Name:** process_list.png
 * **Description:** Captures the execution of ps aux and process identification commands, displaying active PIDs, user ownership, CPU/memory usage percentages, and command execution strings within the containerized Ubuntu environment.
