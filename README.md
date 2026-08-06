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
* 
