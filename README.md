# NetworkWalks Cybersecurity Internship - Week 1: Lab Setup

## 📖 Project Overview
This repository documents the successful setup of an isolated virtual cybersecurity lab for Week 1 of the NetworkWalks internship. The goal was to build a safe, sandboxed environment for future penetration testing exercises, ensuring all practical work remains contained and does not affect the host machine[reference:7].

## 🏗️ Lab Architecture
*   **Hypervisor:** Oracle VirtualBox
*   **Virtual Network:** NAT Network
*   **Attack VM:** Kali Linux (`10.0.0.2/24`)
*   **Network Gateway:** `10.0.0.1`
*   **DNS Server:** `8.8.8.8`

## ✅ Key Tasks Completed
*   [x] Installed and configured Oracle VirtualBox.
*   [x] Imported and configured Kali Linux VM with 5GB RAM.
*   [x] Created a dedicated NAT Network for isolation.
*   [x] Verified network connectivity.

## 🧠 Key Learnings & Challenges
*   **The Learning Curve:** The most valuable part was troubleshooting the network configuration. Understanding the interaction between VirtualBox's NAT Network, the VM adapter settings, and Kali's internal `nmcli` commands was a fantastic hands-on exercise in networking fundamentals.
*   **Overcoming a Challenge:** I initially had no internet access in Kali. I diagnosed the issue by checking the VM's network adapter settings and found it was set to 'NAT' instead of 'NAT Network'. After correcting this, I reconfigured the static IP, and connectivity was restored.*

## 🛠️ Tools & Technologies
*   Oracle VirtualBox
*   Kali Linux
*   Linux Command Line (`nmcli`, `ping`)

## 📸 Evidence
All configuration screenshots and successful ping tests are available in the `/screenshots` folder.

---
**Disclaimer:** This lab was created for educational purposes only. All security testing should only be performed on systems you own or have explicit permission to test.
