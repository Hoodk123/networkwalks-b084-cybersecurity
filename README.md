<div align="center">

<img src="https://capsule-render.vercel.app/api?type=venom&color=0:090d12,100:7f1d1d&height=220&section=header&text=CYBERSECURITY%20LAB&fontSize=42&fontColor=ffffff&animation=fadeIn&fontAlignY=38&desc=NETWORKWALKS%20%7C%20B084%20%7C%20WEEK%2001&descAlignY=60&descSize=16" width="100%" alt="Cybersecurity Lab banner" />

# 🔐 Cybersecurity Lab Environment Setup

**A hands-on virtual lab built to practise cybersecurity fundamentals in a controlled environment.**

<p>
  <img src="https://img.shields.io/badge/Track-Cybersecurity-8b1e2d?style=for-the-badge&logo=kalilinux&logoColor=white" alt="Cybersecurity" />
  <img src="https://img.shields.io/badge/Batch-B084-20252d?style=for-the-badge" alt="Batch B084" />
  <img src="https://img.shields.io/badge/Week-01-20252d?style=for-the-badge" alt="Week 01" />
  <img src="https://img.shields.io/badge/Platform-VirtualBox-8b1e2d?style=for-the-badge&logo=virtualbox&logoColor=white" alt="VirtualBox" />
  <img src="https://img.shields.io/badge/Guest%20OS-Kali%20Linux-20252d?style=for-the-badge&logo=kalilinux&logoColor=white" alt="Kali Linux" />
</p>

[**Repository**](https://github.com/Hoodk123/networkwalks-b084-cybersecurity) · [**LinkedIn**](https://www.linkedin.com/in/kevin-shyaka-94080a319)

</div>

---

## 📌 1. Project Overview

This project documents my first practical cybersecurity lab setup as part of the **NetworkWalks B084 cybersecurity programme**.

I prepared a virtual environment using **Oracle VirtualBox and Kali Linux**, configured the virtual machine's network settings, tested connectivity, and created a snapshot of the lab after setup.

The goal was to build a repeatable environment where I can learn Linux, understand virtual networking, and practise cybersecurity tasks without experimenting on systems I do not own.

## 🎯 2. Project Objectives

- Set up a virtual machine for cybersecurity practice.
- Install and launch Kali Linux in VirtualBox.
- Configure the virtual machine's network settings.
- Understand how a virtual machine connects to a network.
- Test network connectivity from Kali Linux.
- Create a snapshot so the lab can be restored to a known state.
- Record the process with screenshots for future reference.

## 🧰 3. Tools and Technologies

| Tool | Purpose |
| --- | --- |
| **Oracle VirtualBox** | Runs the Kali Linux virtual machine. |
| **Kali Linux** | Provides the Linux environment and cybersecurity tools. |
| **Terminal** | Used to inspect network settings and run connectivity tests. |
| **GitHub** | Stores this documentation and the setup evidence. |

## 🏗️ 4. Lab Setup at a Glance

The lab uses a host computer running VirtualBox, with Kali Linux running as a guest virtual machine.

```text
                 HOST COMPUTER
                       |
                Oracle VirtualBox
                       |
                Kali Linux VM
                       |
              Virtual Network Setup
                       |
             Connectivity Verification
                       |
                Clean VM Snapshot
```

> **Configuration note:** The screenshots below are the evidence for my actual setup. I have not filled in hardware specifications, IP addresses, subnet, gateway, or DNS values that are not recorded in this repository. Those values should match the live VM configuration, not another student's lab.

## ⚙️ 5. Setup Procedure

### Step 1 — Prepare the Virtualization Environment

I prepared Oracle VirtualBox to host the Kali Linux virtual machine. Virtualization provides a separate guest operating system that can be managed independently from the host.

### Step 2 — Install and Launch Kali Linux

I installed and launched Kali Linux inside VirtualBox. Kali Linux is the guest operating system used for the practical cybersecurity exercises in this lab.

### Step 3 — Configure the Virtual Machine Network

I reviewed and configured the VM's network settings so Kali Linux could communicate through the selected virtual network.

Network settings matter because they determine how the guest machine communicates with the host, other virtual machines, and external networks.

### Step 4 — Verify Network Connectivity

I used the Kali Linux terminal to check connectivity. The successful ping test recorded during setup confirmed that the network was responding as expected at that stage.

Example command:

```bash
ping -c 4 <destination-ip-or-hostname>
```

Replace the placeholder with the actual gateway, IP address, or hostname you are testing. A successful ping should show replies; packet loss or an unreachable message indicates that further troubleshooting may be needed.

### Step 5 — Save a Virtual Machine Snapshot

After the setup and connectivity checks, I created a VirtualBox snapshot. A snapshot gives me a restore point, making it easier to return to the saved lab state if a future experiment changes the VM configuration.

---

## 🖼️ 6. Screenshots and Lab Evidence

The following screenshots were captured during my setup process. They document the progress from preparing the virtual machine through network configuration and the final saved state.

### 01 — Initial Lab Setup

![Initial lab setup](./Screenshot%202026-11-15%20164830.png)

### 02 — Virtual Machine Configuration

![Virtual machine configuration](./Screenshot%202026-11-15%20165222.png)

### 03 — Network Configuration

![Network configuration](./Screenshot%202026-11-15%20171229.png)

### 04 — Connectivity Verification

![Connectivity verification](./Screenshot%202026-11-15%20171332.png)

### 05 — Saved Lab State

![Virtual machine snapshot](./Screenshot%202026-11-15%20172116.png)

---

## 🔎 7. Verification Summary

| Check | Result recorded |
| --- | --- |
| Kali Linux installed and launched | Completed |
| Virtual machine network settings configured | Completed |
| Network connectivity tested | Successful ping recorded |
| Virtual machine snapshot created | Completed |

## 🧠 8. What I Learned

Working through this lab helped me understand several important foundations:

- **Virtualization:** A single physical computer can run another operating system inside a virtual machine.
- **Guest and host systems:** The host is the physical computer; the guest is the operating system running inside VirtualBox.
- **Virtual networking:** A VM needs a correctly configured network adapter to communicate.
- **Connectivity testing:** Ping helps check whether another IP address or host can be reached.
- **Snapshots:** A saved VM state provides a useful recovery point before trying new tools or configurations.
- **Technical documentation:** Screenshots and clear explanations make it easier to reproduce a setup and troubleshoot problems later.

## 🛡️ 9. Safe and Responsible Practice

This environment is for learning and authorized testing. I will use cybersecurity tools only against virtual machines, systems I own, or systems for which I have explicit permission to test.

When adding intentionally vulnerable machines in the future, I will review the network mode and isolation settings before running security exercises.

## 🔗 10. Official Resources

- [Oracle VirtualBox Downloads](https://www.virtualbox.org/wiki/Downloads)
- [Kali Linux — Get Kali](https://www.kali.org/get-kali/)
- [Kali Linux Documentation](https://www.kali.org/docs/)
- [GitHub Markdown Guide](https://guides.github.com/features/mastering-markdown/)

## 👤 11. About the Author

**Kevin Shyaka**  
Cybersecurity Learner · NetworkWalks B084

- **LinkedIn:** [linkedin.com/in/kevin-shyaka-94080a319](https://www.linkedin.com/in/kevin-shyaka-94080a319)
- **GitHub:** [github.com/Hoodk123](https://github.com/Hoodk123)

---

<div align="center">

**NETWORKWALKS · B084 · WEEK 01**

*Build the lab. Understand the network. Practise responsibly.*

</div>
