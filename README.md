 **Project 3: Linux System Administration** 
 
 Lesson 1: Linux Package Management

## Project Overview
This project documents practical Linux system administration and package management exercises performed using Ubuntu 24.04.5 LTS running on an Android mobile device via Termux and proot-distro. It highlights software updates, package installation, version verification, and command-line maintenance.

## Learning Objectives
 * Understand Linux package management using the Advanced Package Tool (apt).
 * Update local package repositories and upgrade installed software packages.
 * Check system software availability and install missing tools like curl.
 * Verify package installations and review version information.
## Lab Environment
| Component | Details |
|---|---|
| **Device** | Android smartphone |
| **Terminal** | Termux |
| **Linux Distribution** | Ubuntu 24.04.5 LTS |
| **Installation Method** | proot-distro |
| **Shell** | Bash |

## Practical Exercises & Execution Workflow
### Step 1 — Update Package Information
Fetch the latest package lists from the Ubuntu repositories:
```bash
apt update

```
### Step 2 — Upgrade Installed Packages
Safely upgrade all currently installed system packages to their latest versions:
```bash
apt upgrade -y

```
### Step 3 & 4 — Check and Install curl
Check if the curl data transfer tool is installed, and install it if missing:
```bash
curl --version
apt install curl -y

```
### Step 5 — Verify the Installation
Confirm that curl is correctly installed and operational:
```bash
curl --version

```
## Skills Demonstrated
 * Linux software repository synchronization (apt update).
 * System package upgrades and maintenance (apt upgrade).
 * Dependency resolution and tool installation (apt install).
 * Command-line version verification and diagnostics.
## Project Evidence & Screenshots
### 1. Successful Package Update
 * **Description:** Captures the execution of apt update, successfully fetching repository index files and checking for upgradable packages in the Ubuntu environment.
### 2. Successful Package Upgrade
 * **Description:** Shows the execution of apt upgrade -y, processing package upgrades such as libpcre2-8-0 and completing system-level updates.
### 3. Curl Installation & Version Verification
 * **Description:** Demonstrates the successful installation of curl and libcur14t64, followed by executing curl --version to display the active build details and supported protocols (aarch64-unknown-linux-gnu).
## Author
 * **Emih Benjamin Nwabuenu**
 * **GitHub:** benji-infosec
 * **Career Focus:** IT Support | Linux Administration | Cybersecurity
### **Next Steps:**
 1. Create a new GitHub repository named **linux-system-administration**.
 2. Create a folder named **screenshots** and upload your 3 screenshots, naming them:
   * pkg_update.png
   * pkg_upgrade.png
   * curl_version.png
 