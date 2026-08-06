# Computer Systems, Networking & Cloud Fundamentals

## 1. Fundamentals of Computing

Every modern computing system—from a smartphone to a cloud data center—operates on three foundational pillars:

1. COMPUTATION
2. MEMORY
3. NETWORK


## 2. Computation & Specialized Hardware

Computation is the execution of instructions and mathematical operations. Modern computing relies on specialized processors tailored for different workloads.

### Specialized Processors
* **CPU (Central Processing Unit):** The general-purpose "brain" of the computer. It executes instructions sequentially via the *Fetch-Decode-Execute* cycle using its ALU (Arithmetic Logic Unit), CU (Control Unit), and Registers.
* **GPU (Graphics Processing Unit):** Optimized for massive parallel processing. Designed originally for rendering images, now heavily used for deep learning and parallel math operations.
* **TPU (Tensor Processing Unit):** A proprietary ASIC designed by Google specifically to accelerate matrix math for deep learning frameworks (e.g., TensorFlow).
* **NPU (Neural Processing Unit):** Low-power hardware built into modern consumer devices (e.g., smartphones, laptops) to handle local AI tasks like facial recognition and voice processing.
* **OPU (Optical/Optical-Neural Processing Unit):** An emerging processor class that uses light particles (photons) instead of electricity to compute matrix multiplications at ultra-high speeds with minimal power.
* **DPU (Data Processing Unit):** Offloads network data transfer, encryption, and storage management tasks away from the CPU in data centers.

### Processor Architectures
Processors are designed around specific instruction set architectures (ISA):
* **RISC (Reduced Instruction Set Computer):** Uses simple, uniform instructions that execute in a single clock cycle. Focuses on energy efficiency and speed. *Examples:* ARM (iPhones, Apple M-series), RISC-V.
* **CISC (Complex Instruction Set Computer):** Uses broad, complex instructions capable of multi-step operations within a single command. *Examples:* x86 / x86-64 (Intel Core, AMD Ryzen).
  
## 3. Memory & Storage Architecture
Data must be accessed quickly while program execution occurs, then saved permanently.
### Primary Memory (Volatile)
* **Registers:** Tiny, ultra-fast memory locations directly inside the CPU core.
* **Cache:** High-speed static memory (L1, L2, L3) sitting between the CPU and main memory to hold frequently accessed data.
* **RAM (Random Access Memory):** The main working space holding open applications and data currently in use. Erased when powered off.

### Secondary Memory (Non-Volatile)
* Permanent storage devices like **SSDs (Solid State Drives)**, **HDDs (Hard Disk Drives)**, and external media that retain data without electricity.

## 4. Operating Systems & Execution Spaces

An **Operating System (OS)** manages system hardware and abstracts hardware controls for application software. *Examples:* Linux (Ubuntu, Debian), Windows, macOS.

### Kernel Space vs. User Space
To ensure system stability and security, OS memory is split into two distinct regions:

* **Kernel Space:** Highly privileged memory where the core OS (Kernel) runs. Has direct control over hardware, memory management, and device drivers. A failure here causes a system crash (Kernel Panic/BSOD).
* **User Space:** Sandboxed memory space where standard applications (browsers, scripts, apps) execute. Cannot directly touch hardware; must request services from the kernel via **System Calls (Syscalls)**.


## 5. Computer Networks & Communication

Networking allows isolated computing units to transfer data across distances.

### The Network Interface Card (NIC)
A **NIC** is the hardware component (chip or physical board) that connects a computing device to a network.
* Asserts a unique physical address called a **MAC Address**.
* **Smart NICs** contain onboard processing power to handle firewalls, encryption, and virtualization directly on the card to free up CPU cycles.

### IP Addressing (Internet Protocol)
An **IP Address** is a logical address assigned to a device on a network so packets know where to travel.

* **IPv4 vs. IPv6:** IPv4 uses 32-bit numbers (`192.168.1.1`), whereas IPv6 uses 128-bit hexadecimal strings to solve address exhaustion.
* **Public IP:** Globally unique address assigned by an **ISP (Internet Service Provider)**. Reachable from anywhere on the public internet.
* **Private IP:** Internal address assigned within a local network (LAN) by a router (e.g., `192.168.x.x` or `10.x.x.x`). Invisible to the external internet.

## 6. Software Architecture, Virtualization & Cloud

Modern computing applications rarely run on bare physical hardware; they are abstracted into scalable environments.

### System Interfaces & Protocols
* **API (Application Programming Interface):** A set of defined rules allowing different software applications to communicate with each other over the web or locally.
* **Torrent (Peer-to-Peer / P2P):** A decentralized networking protocol where files are shared directly between user devices (peers) instead of downloading from a centralized server.

### Virtualization & Cloud Infrastructure
* **Server:** A specialized high-performance computer designed to run continuous services and respond to requests from client devices over a network.
* **Linux / Ubuntu:** Linux is the dominant open-source kernel used for world servers. **Ubuntu** is one of its most widely deployed server distributions.
* **VM (Virtual Machine):** Software-based emulation of a physical computer running its own isolated OS, powered by a **Hypervisor** on host hardware.
* **Cloud Computing:** On-demand delivery of computing power, servers, database storage, and APIs over the internet (e.g., AWS, Google Cloud, Azure) paying only for consumed resources.
#### Essential AWS Services:
* **AWS EC2 (Elastic Compute Cloud):** On-demand Virtual Machines (VMs) configurable with custom CPUs, memory, and OS options (e.g., Ubuntu Server).
* **AWS VPC (Virtual Private Cloud):** Isolated virtual networks within AWS where users define their own IP address ranges, subnets, and routing tables.
* **AWS ENI (Elastic Network Interface):** Virtual NICs attached to EC2 instances that manage public and private IP assignments, security group configurations, and network traffic within the cloud.

