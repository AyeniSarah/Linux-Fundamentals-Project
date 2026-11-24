# **Linux System Diagnostics & Network Connectivity Lab**

A hands-on Linux command-line project focused on system administration, hardware resource monitoring, and network connectivity troubleshooting within a Kali Linux virtual machine. The project demonstrates the use of essential Linux utilities to inspect system configurations, monitor available resources, and verify external network connectivity using ICMP and DNS resolution.

## **Table of Contents**

- Project Overview
- Network Topology
- Tools and Technologies
- Configuration Steps
- Results and Findings
- Author

## **Project Overview**

This project demonstrates foundational **Linux system administration** and **network troubleshooting** skills using a Kali Linux virtual environment.

The main objectives were to:

- Verify system identity, including the active username and hostname.
- Identify the current working directory.
- Inspect the Linux kernel version and system architecture.
- Monitor available system memory, swap allocation, and disk storage.
- Test external network connectivity using ICMP echo requests.
- Verify DNS resolution and domain reachability.

The exercise provides practical experience with Linux command-line utilities and foundational IT infrastructure diagnostics.

## **Network Topology**

The project used a virtualized Kali Linux environment to perform local system diagnostics and communicate with external network destinations.

**Network Components:**

- **Local Environment:** Kali Linux virtual machine.
- **Active User:** `kali`
- **Hostname:** `kali`
- **Working Directory:** `/home/kali`
- **External DNS Target:** `8.8.8.8` (Google Public DNS).
- **External Domain Target:** `google.com`.
- **Resolved IP Address:** `142.250.137.100`.
- **Connectivity Protocol:** ICMP (Internet Control Message Protocol).

The network tests involved sending ICMP echo requests to an external IP address and a domain name to evaluate connectivity and DNS resolution.

## **Tools and Technologies**

- **Operating System:** Kali Linux.
- **Kernel:** Linux `6.19.14+kali-amd64`.
- **System Identification:** `whoami`, `hostname`, `pwd`.
- **Kernel Inspection:** `uname -a`.
- **Memory Monitoring:** `free -h`.
- **Disk Space Monitoring:** `df -h`.
- **Network Diagnostics:** `ping`.
- **Virtualization:** Kali Linux virtual machine.
- **Network Protocol:** ICMP.
- **DNS:** Google Public DNS (`8.8.8.8`).

## **Configuration Steps**

1. **Verified System Identity**

   Used the following commands to identify the active user, hostname, and current working directory:
   ```
   whoami
   hostname
   pwd
   ```
2. **Inspected Linux Kernel and Architecture**

   Executed the following command to retrieve kernel information and system architecture:
   ```
   uname -a
   ```
3. **Monitored System Memory and Storage**

   Used the following commands to inspect RAM utilization, swap allocation, and disk space:
   ```
   free -h
   df -h
   ```
4. **Tested External IP Connectivity**

   Sent two ICMP echo requests to Google Public DNS to verify direct IP connectivity:
   ```
   ping -c 2 8.8.8.8
   ```
5. **Tested DNS Resolution and Domain Connectivity**

   Sent four ICMP echo requests to `google.com` to verify successful domain resolution and network reachability:
   ```
   ping -c 4 google.com
   ```

## **Results and Findings**

The project successfully demonstrated basic Linux system diagnostics and network connectivity testing.

**1. System Identification**

- Active username: `kali`.
- Hostname: `kali`.
- Working directory: `/home/kali`.

**2. Kernel and Architecture**

- Kernel version: `6.19.14+kali-amd64`.
- System architecture: `x86_64`.

**3. Memory and Storage**

- Total RAM: Approximately **1.96 GiB**.
- Available memory: Approximately **956 MiB**.
- Total swap allocation: **953 MiB**.
- Primary partition: `/dev/sda1`.
- Total disk capacity: **79 GB**.
- Available disk space: **59 GB**.

**4. Direct IP Connectivity – 8.8.8.8**

- Packets transmitted: 2.
- Packets received: 2.
- Packet loss: **0%**.
- Average round-trip time (RTT): **21.534 ms**.

**5. Domain Connectivity – google.com**

- Resolved IP address: `142.250.137.100`.
- Packets transmitted: 4.
- Packets received: 4.
- Packet loss: **0%**.
- Average round-trip time (RTT): **18.193 ms**.

**Key Findings**

- Successfully verified the Kali Linux system identity and configuration.
- Confirmed the Linux kernel version and system architecture.
- Assessed available memory, swap allocation, and disk utilization.
- Established successful external IP connectivity with zero packet loss.
- Verified DNS resolution and successful communication with `google.com`.
- Observed comparable network response times between direct IP and domain-based connectivity tests.

The results demonstrate successful execution of foundational Linux administration and network troubleshooting tasks.

## **Author**

- **GitHub:** [GitHub Profile](https://github.com/your-username?utm_source=chatgpt.com)
- **Area of Interest:** Linux Administration, Networking, Cybersecurity, and Governance, Risk & Compliance (GRC).
