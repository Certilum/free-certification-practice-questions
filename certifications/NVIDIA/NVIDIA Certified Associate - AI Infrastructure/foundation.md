<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/NVIDIA/NVIDIA-Certified%20Professional%3A%20AI%20Infrastructure" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>NVIDIA Certified Associate - AI Infrastructure</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [AI Infrastructure](#ai-infrastructure) (12 questions)
- [AI Operations](#ai-operations) (7 questions)
- [Essential AI Knowledge](#essential-ai-knowledge) (11 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:31.609Z |
| Domains | 3 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| AI Infrastructure | 12 |
| AI Operations | 7 |
| Essential AI Knowledge | 11 |

---

### **AI Infrastructure**

### 1. What is the primary purpose of NVLink in an AI infrastructure cluster?

- [ ] **A)** Inter-node cluster management protocol
- [ ] **B)** High-bandwidth, low-latency intra-node GPU interconnect
- [ ] **C)** Network-attached storage protocol
- [ ] **D)** GPU virtualization hypervisor

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> NVLink is a high-bandwidth, low-latency interconnect for GPU-to-GPU communication within a node, not for management, storage, or virtualization.
 
 
</details>

### 2. Which fabric types are recognized for their RDMA capabilities in AI clusters?

- [ ] **A)** NVLink
- [ ] **B)** InfiniBand
- [ ] **C)** Ethernet
- [ ] **D)** PCIe

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, C**
 
> 💡  **Explanation** 
> 
> Both InfiniBand and Ethernet can support RDMA, while NVLink is a GPU interconnect and PCIe is a local bus, not a network fabric.
 
 
</details>

### 3. An engineer issues the command shown to inspect GPU health. What class of error is being queried?

```bash
nvidia-smi --query-gpu=ecc.errors.corrected.volatile.total --format=csv
```

- [ ] **A)** CRC errors on InfiniBand links
- [ ] **B)** ECC memory errors
- [ ] **C)** PCIe training errors
- [ ] **D)** GPU thermal throttling

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The query reads corrected ECC error counters, so it monitors GPU memory reliability rather than fabrics or thermal state.
 
 
</details>

### 4. What is the function of the NVIDIA Collective Communications Library (NCCL)?

- [ ] **A)** It orchestrates communication between GPUs
- [ ] **B)** It manages Kubernetes resource scheduling
- [ ] **C)** It performs storage replication
- [ ] **D)** It provides GPU power management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NCCL is the software layer that coordinates GPU communication, and its diagnostics focus on timeouts and ring/tree topologies.
 
 
</details>

### 5. Which of the following are documented common traps when troubleshooting AI infrastructure?

- [ ] **A)** Confusing GPU utilization with GPU throughput
- [ ] **B)** Blaming the algorithm when the root cause is an NCCL topology
- [ ] **C)** Ignoring the physical layer, such as unseated cables
- [ ] **D)** Calling GPUDirect RDMA a CPU-based transfer mechanism

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The playbook lists utilization/throughput confusion, blaming the algorithm, and ignoring physical-layer issues as common traps.
 
 
</details>

### 6. The output shown is from an InfiniBand link diagnostic. What type of problem does this status indicate?

```text
State: Down
Physical state: Disabled
```

- [ ] **A)** Link-state error
- [ ] **B)** Ethernet congestion-induced latency
- [ ] **C)** NCCL timeout caused by environment variables
- [ ] **D)** GPU ECC error

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A Down state with a disabled physical state corresponds to a link-state error in the InfiniBand fabric, not congestion or memory errors.
 
 
</details>

### 7. What is a primary benefit of GPUDirect RDMA in AI clusters?

- [ ] **A)** It increases GPU core clock speeds
- [ ] **B)** It allows data to move between GPU memory and network adapters without CPU involvement
- [ ] **C)** It replaces NVLink with Ethernet
- [ ] **D)** It eliminates the need for InfiniBand subnet managers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> GPUDirect RDMA enables direct transfers between GPU memory and network adapters, bypassing the CPU to reduce latency.
 
 
</details>

### 8. Which indicators are associated with physical-layer link problems in AI infrastructure?

- [ ] **A)** ECC errors on GPU memory
- [ ] **B)** CRC errors on InfiniBand links
- [ ] **C)** PCIe training errors
- [ ] **D)** Higher application-level checkpoint frequency

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The playbook lists ECC errors, InfiniBand CRC errors, and PCIe training errors as signs of faulty cabling, loose connections, or failing transceivers.
 
 
</details>

### 9. An administrator runs the command shown to inspect GPU communication paths. Which interconnect is being validated?

```bash
nvidia-smi topo -m
```

- [ ] **A)** InfiniBand fabric routing
- [ ] **B)** NVLink/NVSwitch topology
- [ ] **C)** Ethernet VLAN configuration
- [ ] **D)** PCIe power management

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The nvidia-smi topology command displays GPU connectivity, including NVLink links and switches, to detect broken or incorrectly detected topologies.
 
 
</details>

### 10. What does the trap 'confusing throughput with latency' describe?

- [ ] **A)** Assuming lower bandwidth always reduces accuracy
- [ ] **B)** Replacing low latency with high throughput
- [ ] **C)** Assuming a high-bandwidth link is healthy even when latency is high
- [ ] **D)** Using throughput to estimate GPU utilization

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: C**
 
> 💡  **Explanation** 
> 
> High bandwidth can mask high latency, and in AI training, latency can be more damaging than reduced throughput.
 
 
</details>

### 11. Which statements about NVLink are correct?

- [ ] **A)** It is used as a long-haul inter-node fabric
- [ ] **B)** It is intended for intra-node GPU communication
- [ ] **C)** It is based on IEEE Ethernet standards
- [ ] **D)** It is a high-bandwidth, low-latency interconnect

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B, D**
 
> 💡  **Explanation** 
> 
> NVLink is an intra-node GPU interconnect with high bandwidth and low latency; NVSwitch scales it within the node.
 
 
</details>

### 12. The environment variables shown are being set before launching a distributed job. Which software layer are they configuring?

```bash
export NCCL_DEBUG=INFO
export NCCL_P2P_LEVEL=PHB
```

- [ ] **A)** NCCL communication between GPUs
- [ ] **B)** InfiniBand subnet manager behavior
- [ ] **C)** Kubernetes pod scheduling
- [ ] **D)** GPU thermal limits

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> These variables control NCCL debug output and peer-to-peer level, so they affect NCCL communication and topology detection.
 
 
</details>


---

### **AI Operations**

### 13. What is the primary purpose of NVLink and NVSwitch in an AI infrastructure?

- [ ] **A)** Provide high-bandwidth, low-latency intra-node GPU communication
- [ ] **B)** Connect GPUs to remote storage arrays
- [ ] **C)** Manage container orchestration
- [ ] **D)** Replace Ethernet for inter-node traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NVLink and NVSwitch enable high-bandwidth, low-latency interconnect for intra-node GPU communication, supporting optimal peer-to-peer memory access.
 
 
</details>

### 14. Which two of the following are typical InfiniBand fabric troubleshooting areas?

- [ ] **A)** Link-state errors
- [ ] **B)** Subnet manager issues
- [ ] **C)** VLAN misconfiguration
- [ ] **D)** Ethernet congestion collapse

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Link-state errors and subnet manager issues are common InfiniBand concerns. VLAN and Ethernet congestion are associated with Ethernet environments, not InfiniBand.
 
 
</details>

### 15. Review the displayed command and identify what it is used to troubleshoot.

```bash
nvidia-smi topo -m
```

- [ ] **A)** NVLink topology detection
- [ ] **B)** Ethernet packet loss measurement
- [ ] **C)** Kernel module loading
- [ ] **D)** Memory bandwidth benchmarking

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command displays GPU peer-to-peer topology, which is used to detect NVLink connections and verify correct topology detection.
 
 
</details>

### 16. What capability does GPUDirect RDMA primarily enable?

- [ ] **A)** Direct data transfer between GPU memory and network adapters
- [ ] **B)** CPU-side encryption of network traffic
- [ ] **C)** Virtual GPU memory overcommit
- [ ] **D)** Automatic GPU driver updates

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> GPUDirect RDMA allows GPUs to exchange data directly with network adapters, bypassing the CPU and reducing latency.
 
 
</details>

### 17. Which error detection mechanisms can identify faulty cabling or failing transceivers?

- [ ] **A)** ECC errors
- [ ] **B)** CRC errors on InfiniBand links
- [ ] **C)** PCIe training errors
- [ ] **D)** Hypervisor migration logs

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> ECC, CRC, and PCIe training errors are physical-layer indicators. Hypervisor migration logs are not used to detect physical-layer failures.
 
 
</details>

### 18. The given command reports GPU interconnect status. Which tool is being used?

```bash
nvidia-smi nvlink -s
```

- [ ] **A)** nvidia-smi nvlink -s
- [ ] **B)** ibstatus
- [ ] **C)** nvtop
- [ ] **D)** nvcc

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command 'nvidia-smi nvlink -s' queries NVLink status and is part of the NVIDIA System Management Interface.
 
 
</details>

### 19. Which trap is described by assuming a high-bandwidth link works well despite high latency?

- [ ] **A)** Confusing Throughput with Latency
- [ ] **B)** Blaming the Algorithm
- [ ] **C)** Ignoring the Physical Layer
- [ ] **D)** Misinterpreting MIG

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> High latency can be more damaging than lower throughput in AI training. This trap confuses throughput with latency.
 
 
</details>


---

### **Essential AI Knowledge**

### 20. Which statement best describes the primary purpose of NVLink and NVSwitch in an AI infrastructure?

- [ ] **A)** Enabling communication between GPUs inside one server
- [ ] **B)** Connecting GPUs across separate data centers
- [ ] **C)** Connecting storage devices to the network
- [ ] **D)** Scheduling AI workload containers

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NVLink and NVSwitch are high-bandwidth, low-latency interconnects designed for intra-node GPU communication, not inter-node or storage networking.
 
 
</details>

### 21. Which statements correctly describe architectural differences between InfiniBand and Ethernet fabrics for RDMA? Select all that apply.

- [ ] **A)** InfiniBand uses a subnet manager for fabric control.
- [ ] **B)** Ethernet can experience congestion-induced latency.
- [ ] **C)** Ethernet is inherently lossless for RDMA.
- [ ] **D)** InfiniBand depends on TCP/IP for flow control.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> InfiniBand fabrics require a subnet manager, and Ethernet RDMA can suffer from congestion-induced latency. TCP/IP is not part of InfiniBand flow control.
 
 
</details>

### 22. Examine the initialization log in the code block. Which software component is being initialized?

```bash
NCCL version 2.12.7
NCCL_0 pid=1234 rank=0 nranks=4
NCCL_0 net#0 using device mlx5_0

```

- [ ] **A)** NCCL
- [ ] **B)** NVSwitch
- [ ] **C)** GPUDirect RDMA
- [ ] **D)** Ethernet fabric

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The log shows NCCL version and initialization messages, indicating the NVIDIA Collective Communications Library is the software being initialized.
 
 
</details>

### 23. What does GPUDirect RDMA enable in high-performance AI clusters?

- [ ] **A)** Direct data transfer between GPU memory and network adapters
- [ ] **B)** Replacing network adapters with NVLink switches
- [ ] **C)** Increasing GPU core clock speed
- [ ] **D)** Managing Kubernetes pods automatically

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> GPUDirect RDMA allows direct data transfer between GPU memory and network adapters, reducing latency by bypassing the CPU.
 
 
</details>

### 24. Which of the following are physical-layer error detection mechanisms mentioned in the playbook? Select all that apply.

- [ ] **A)** Monitoring ECC errors
- [ ] **B)** Checking CRC errors on InfiniBand links
- [ ] **C)** Detecting PCIe training errors
- [ ] **D)** Measuring GPU clock speed only

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The playbook lists ECC errors, CRC errors on InfiniBand links, and PCIe training errors as physical-layer detection mechanisms.
 
 
</details>

### 25. The code block shows output listing multiple GPU links. Which interconnect is being checked?

```bash
GPU 0: A100-SXM4-40GB
  Link 0: 25.78 GB/s
  Link 1: 25.78 GB/s
  Link 2: 25.78 GB/s
  Link 3: 25.78 GB/s

```

- [ ] **A)** NVLink
- [ ] **B)** InfiniBand
- [ ] **C)** Ethernet
- [ ] **D)** PCIe

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The per-GPU link bandwidth output is typical of NVLink status checks, such as nvidia-smi nvlink -s.
 
 
</details>

### 26. According to the playbook, what is a primary diagnostic focus for NCCL?

- [ ] **A)** Resolving NCCL errors like timeouts or incorrect ring/tree topologies
- [ ] **B)** Adjusting GPU voltage and fan curves
- [ ] **C)** Replacing NVLink cables
- [ ] **D)** Resizing Kubernetes nodes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NCCL troubleshooting focuses on resolving errors such as timeouts and incorrect ring/tree topologies caused by configuration or network mismatches.
 
 
</details>

### 27. Which statements correctly identify intra-node and inter-node interconnect technologies? Select all that apply.

- [ ] **A)** NVLink is used for intra-node GPU communication.
- [ ] **B)** NVLink is an inter-node fabric technology.
- [ ] **C)** InfiniBand is commonly used for inter-node fabric communication.
- [ ] **D)** InfiniBand is used inside a single GPU package.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> NVLink connects GPUs within one node, while InfiniBand is an inter-node fabric used for RDMA-based communication between servers.
 
 
</details>

### 28. The code block contains a connection log line. Which fabric is NCCL using?

```bash
NCCL INFO network.cc:1396 Connecting to 10.0.0.4:45231 via NET/IB

```

- [ ] **A)** InfiniBand
- [ ] **B)** Ethernet
- [ ] **C)** NVLink
- [ ] **D)** PCIe

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> NET/IB in the NCCL log indicates the InfiniBand fabric is being used for communication.
 
 
</details>

### 29. Why can a high-bandwidth link still harm AI training performance, according to the playbook?

- [ ] **A)** High latency can be more damaging than lower throughput
- [ ] **B)** Bandwidth never affects distributed training
- [ ] **C)** High bandwidth always means low latency
- [ ] **D)** Latency is irrelevant to collective operations

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The playbook warns that confusing throughput with latency is a trap: high latency can hurt AI training more than lower bandwidth.
 
 
</details>

### 30. Which actions are part of troubleshooting physical-layer and peer-to-peer connectivity? Select all that apply.

- [ ] **A)** Identifying broken NVLink links
- [ ] **B)** Monitoring ECC errors
- [ ] **C)** Verifying PCIe peer-to-peer support
- [ ] **D)** Blaming the model architecture

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Broken NVLink links, ECC errors, and PCIe peer-to-peer verification are physical-layer or connectivity checks. Blaming the algorithm is a common trap.
 
 
</details>
