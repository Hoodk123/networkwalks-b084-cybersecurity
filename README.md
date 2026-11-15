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
  <img src="https://img.shields.io/badge/Network-10.0.0.0%2F24-20252d?style=for-the-badge" alt="10.0.0.0/24 network" />
</p>

[**Repository**](https://github.com/Hoodk123/networkwalks-b084-cybersecurity) · [**LinkedIn**](https://www.linkedin.com/in/kevin-shyaka-94080a319)

</div>

---

## 📌 1. Project Overview

This project documents my first practical cybersecurity lab setup as part of the **NetworkWalks B084 cybersecurity programme**.

I prepared a virtual environment using **Oracle VirtualBox and Kali Linux**, configured a dedicated NAT Network, assigned the Kali virtual machine its required IP address, tested connectivity, and created a snapshot of the lab.

The goal is to build a repeatable environment where I can learn Linux, understand virtual networking, and practise cybersecurity tasks safely.

## 🎯 2. Project Objectives

- Set up a virtual machine for cybersecurity practice.
- Install and launch Kali Linux in VirtualBox.
- Create a NAT Network using the **10.0.0.0/24** subnet.
- Configure Kali Linux with the static IP address **10.0.0.2/24**.
- Enable clipboard and drag-and-drop integration.
- Configure a shared host folder for file exchange.
- Verify network connectivity and Internet access.
- Create a VM snapshot as a recovery point.

## 🧰 3. Tools and Technologies

| Tool | Purpose |
| --- | --- |
| **Oracle VirtualBox** | Runs the Kali Linux virtual machine. |
| **Kali Linux** | Guest operating system for cybersecurity practice. |
| **NAT Network** | Provides networking for the virtual lab. |
| **Terminal** | Used to inspect network settings and test connectivity. |
| **GitHub** | Stores this documentation and setup evidence. |

## 🏗️ 4. Lab Architecture

The lab uses a host computer running VirtualBox, with Kali Linux running as a guest virtual machine connected to a custom NAT Network.

```text
                 HOST COMPUTER
                       |
                Oracle VirtualBox
                       |
                 Kali Linux VM
                 10.0.0.2/24
                       |
                 NAT Network
                 10.0.0.0/24
                       |
             Network / Internet access
```

## ⚙️ 5. Lab Configuration

| Component | Configuration |
| --- | --- |
| Virtualization platform | Oracle VirtualBox |
| Guest operating system | Kali Linux |
| Network attachment | NAT Network |
| Network subnet | **10.0.0.0/24** |
| Kali Linux IPv4 address | **10.0.0.2/24** |
| Planned VM address range | **10.0.0.2 – 10.0.0.99** |
| Gateway reference | **10.0.0.1** |
| Shared host folder | `/downloads` |
| Clipboard | Enabled |
| Drag and drop | Enabled |
| Internet connectivity | Required |

The subnet and Kali IP address follow the Week 1 Project Module 1 lab requirements. The gateway value **10.0.0.1** is the reference suggested in the lab guide if Internet connectivity needs troubleshooting.

## 🪜 6. Setup Procedure

### Step 1 — Prepare the Virtualization Environment

I prepared Oracle VirtualBox to host the Kali Linux virtual machine. Virtualization allows a separate operating system to run inside the host computer.

### Step 2 — Install and Import Kali Linux

I installed and launched Kali Linux inside VirtualBox. Kali Linux is the guest operating system used for the practical cybersecurity exercises.

### Step 3 — Create the NAT Network

I configured a custom NAT Network in VirtualBox using the required subnet:

```text
Network: NAT Network
Subnet:  10.0.0.0/24
```

A NAT Network allows virtual machines connected to the same virtual network to communicate while providing network address translation for external connectivity.

### Step 4 — Configure Kali Linux Networking

I configured the Kali Linux virtual machine to use the required static IPv4 address:

```text
IP address: 10.0.0.2/24
Subnet:     255.255.255.0
Gateway:    10.0.0.1 (lab guide reference)
```

### Step 5 — Enable VM Integration Features

I configured the VirtualBox integration features required for the lab:

- Shared clipboard
- Drag and drop
- Shared host folder: `/downloads`

These features make it easier to exchange text and files between the host computer and the Kali Linux virtual machine.

### Step 6 — Verify Network Connectivity

I used the Kali Linux terminal to test network connectivity. The successful ping test captured during setup confirmed that the tested destination responded.

Example command:

```bash
ping -c 4 10.0.0.1
```

A successful ping displays replies from the destination. Internet access can also be checked by testing an external reachable IP address and DNS resolution.

### Step 7 — Create a VM Snapshot

After completing the setup and connectivity checks, I created a VirtualBox snapshot. This gives me a restore point if future experiments change the VM configuration.

---

## 🖼️ 7. Screenshots and Lab Evidence

The following screenshots were captured during my setup process. They document the virtual machine preparation, network configuration, connectivity test, and saved lab state.

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

## 🔎 8. Verification Summary

| Check | Expected / recorded configuration |
| --- | --- |
| Kali Linux installed and launched | Completed |
| NAT Network created | 10.0.0.0/24 |
| Kali Linux IP configured | 10.0.0.2/24 |
| Clipboard and drag-and-drop | Enabled as required |
| Shared folder | /downloads |
| Connectivity test | Successful ping recorded |
| VM snapshot | Created |

## 🧠 9. What I Learned

- **Virtualization:** A physical computer can run another operating system inside a virtual machine.
- **Host and guest systems:** The host is the main computer; the guest is the operating system running inside VirtualBox.
- **NAT Network:** Virtual machines can share a virtual network and communicate with one another.
- **IPv4 addressing:** I practised configuring an IP address and understanding a subnet.
- **Connectivity testing:** Ping helps check whether a destination can be reached.
- **Snapshots:** A saved VM state provides a useful recovery point before future experiments.
- **Lab documentation:** Recording configurations and screenshots makes technical work easier to review and reproduce.

## 🛡️ 10. Safe and Responsible Practice

This environment is for education and authorized security testing. I will use cybersecurity tools only against virtual machines, systems I own, or systems for which I have explicit permission to test.

Before adding other lab machines, I will verify their network configuration and ensure that testing remains within the intended lab environment.

## 🔗 11. Resources

- [Oracle VirtualBox Downloads](https://www.virtualbox.org/wiki/Downloads)
- [Kali Linux — Get Kali](https://www.kali.org/get-kali/)
- [Kali Linux Documentation](https://www.kali.org/docs/)
- [NetworkWalks](https://www.networkwalks.com/)

## 👤 12. About the Author

**Kevin Shyaka**  
Cybersecurity Learner · NetworkWalks B084

- **LinkedIn:** [linkedin.com/in/kevin-shyaka-94080a319](https://www.linkedin.com/in/kevin-shyaka-94080a319)
- **GitHub:** [github.com/Hoodk123](https://github.com/Hoodk123)

---

<div align="center">

**NETWORKWALKS · B084 · WEEK 01**

*Build the lab. Understand the network. Practise responsibly.*

</div>
