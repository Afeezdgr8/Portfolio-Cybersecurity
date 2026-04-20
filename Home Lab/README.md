# The Architect’s Sandbox (Enterprise Lab)

## 📌 Overview
This repository documents the foundation of my security research environment. This lab is a segmented virtual network designed to mimic a corporate environment for testing threat detection and incident response workflows.

## 💻 Host System Specs
- **Hardware:** Custom 5-GPU Rig (Optimized for AI Inference and parallel processing).
- **Hypervisor:** Oracle VirtualBox.

## 🌐 Network Architecture
- **Network Mode:** NAT Network (Segmented).
- **Network Name:** `SOC LAB`.
- **Subnet:** `10.0.2.0/24`.

### VM Inventory
| VM Name | Role | OS | IP Address |
| :--- | :--- | :--- | :--- |
| **Ubuntu-SOC** | Log Server / Analyst | Ubuntu 24.04 | 10.0.2.4 |
| **Kali-Attack** | Offensive Testing | Kali Linux | 10.0.2.15 |

## ✅ Connectivity Verification
To ensure the virtual "plumbing" was functional, I performed an ICMP echo request (ping) between the nodes.
- **Source:** Ubuntu-SOC (10.0.2.4)
- **Target:** Kali-Attack (10.0.2.15)
- **Result:** **Success.**

## 📸 Proof of Work
<img width="3024" height="4032" alt="GPU 1" src="https://github.com/user-attachments/assets/e0e03681-f368-46f4-9784-cc0939c7a661" />


<img width="4032" height="3024" alt="GPU 2" src="https://github.com/user-attachments/assets/6f790389-0460-4f5e-8b99-f5bef425fead" />


<img width="419" height="169" alt="image" src="https://github.com/user-attachments/assets/2711055d-2f8a-4328-af1a-cb2f6ebd5446" />

<img width="1023" height="437" alt="image" src="https://github.com/user-attachments/assets/3d94dd61-e42f-429c-867b-63a72bf1cd84" />

<img width="629" height="427" alt="image" src="https://github.com/user-attachments/assets/afe5be87-f153-4e16-ab50-73a558e3aba0" />

<img width="401" height="346" alt="image" src="https://github.com/user-attachments/assets/67f8ab18-921f-45b3-820f-9d81bc4cf851" />



