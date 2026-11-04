# Lesson 2: Checking Disk Space, Memory, and System Resources
## 🎯 Objective
Learn how to monitor storage allocation, memory (RAM/swap) utilization, and hardware architecture parameters in a Linux environment to ensure system performance, stability, and resource availability.
## 💻 Execution Workflow
Open your Termux terminal, log into Ubuntu
```bash
proot-distro login ubuntu

```
and execute the following system resource commands:
### Step 1 — Check Filesystem Disk Space Usage
View disk space availability and partition utilization in a human-readable format (-h):
```bash
df -h

```
### Step 2 — Check Free and Used Memory
Inspect active RAM and swap memory consumption:
```bash
free -h

```
### Step 3 — Inspect CPU Architecture and Kernel Details
Check your Linux kernel version and hardware architecture specifications:
```bash
uname -r
lscpu

```
## 📸 Lesson 2 Evidence & Screenshots
When you take your screenshots during these exercises, save them inside your screenshots/ directory with these exact filenames to match your main portfolio structure:
 * **1. Disk Space Allocation (disk_space.png)**
   * **Description:** Captures the output of df -h, displaying total storage capacity, used space, available space, and mount points (/) across the containerized filesystem.
 * **2. Memory Utilization (memory_usage.png)**
   * **Description:** Shows the output of free -h, illustrating total physical RAM allocated, used memory, and available buffer/cache space in the mobile Linux environment.
