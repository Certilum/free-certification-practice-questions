<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/NVIDIA/NVIDIA%20Certified%20Professional%20-%20AI%20Operations.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>NVIDIA Certified Professional - AI Operations</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [AI Cluster Installation and Deployment Skills](#ai-cluster-installation-and-deployment-skills) (9 questions)
- [Cluster Administration](#cluster-administration) (7 questions)
- [Troubleshooting and Optimization](#troubleshooting-and-optimization) (7 questions)
- [Workload Management](#workload-management) (7 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:45:36.742Z |
| Domains | 4 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| AI Cluster Installation and Deployment Skills | 9 |
| Cluster Administration | 7 |
| Troubleshooting and Optimization | 7 |
| Workload Management | 7 |

---

### **AI Cluster Installation and Deployment Skills**

### 1. Where must the NVIDIA driver be installed on a cluster to support GPU workloads in containers?

- [ ] **A)** Host machine
- [ ] **B)** Inside the container image
- [ ] **C)** In the Docker daemon
- [ ] **D)** On a remote driver server

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The NVIDIA driver must be installed on the host OS; containers use it through the NVIDIA Container Toolkit.
 
 
</details>

### 2. Which statements about the installation and runtime location of the NVIDIA driver for GPU containers are correct?

- [ ] **A)** Driver must be on the host OS.
- [ ] **B)** Container image should include kernel driver.
- [ ] **C)** GPU containers depend on the host driver.
- [ ] **D)** Driver can be loaded only inside the container.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> GPU containers rely on the host-installed NVIDIA driver at runtime; the image only needs user-space CUDA libraries.
 
 
</details>

### 3. The Dockerfile shown attempts to install the NVIDIA driver inside the image. What is the primary problem with this approach?

```dockerfile
FROM nvidia/cuda:12.0-runtime
RUN apt-get install -y nvidia-driver-535
CMD ["nvidia-smi"]

```

- [ ] **A)** Driver must reside on the host machine.
- [ ] **B)** Use latest tag instead.
- [ ] **C)** Docker provides full security isolation.
- [ ] **D)** Container cannot run because it lacks a scheduler.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The NVIDIA driver must reside on the host machine; installing it inside the Docker image does not enable GPU access.
 
 
</details>

### 4. Why is relying on the 'latest' tag risky for GPU container images in AI cluster deployments?

- [ ] **A)** Latest always points to a stable release.
- [ ] **B)** The tag can move to a newer version.
- [ ] **C)** Latest cannot be used with CUDA images.
- [ ] **D)** Latest prevents checkpointing from working.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The 'latest' tag is volatile and can point to a different image version over time, causing inconsistent deployments.
 
 
</details>

### 5. Which two practices help avoid image tag volatility when deploying AI containers in a cluster?

- [ ] **A)** Pin images by digest.
- [ ] **B)** Use immutable version tags.
- [ ] **C)** Always use the latest tag.
- [ ] **D)** Remove tags after building.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Pinning by digest or using immutable version tags ensures the exact image content is used for reproducible deployments.
 
 
</details>

### 6. The Dockerfile references an image tag in its base image instruction. Which deployment concern does this introduce?

```dockerfile
FROM nvidia/cuda:latest
ENTRYPOINT ["nvidia-smi"]

```

- [ ] **A)** Missing host driver
- [ ] **B)** Image tag volatility
- [ ] **C)** Unsecured multi-tenant boundary
- [ ] **D)** Insufficient GPU scheduling

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Using a mutable tag such as 'latest' creates image tag volatility because the referenced image can change unexpectedly.
 
 
</details>

### 7. Why is Docker not considered a complete security boundary for container workloads in multi-tenant AI clusters?

- [ ] **A)** Same isolation as a hypervisor.
- [ ] **B)** Containers share the host kernel.
- [ ] **C)** Docker prevents all host-level access.
- [ ] **D)** Docker automatically isolates tenants.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> Docker containers share the host kernel, so additional security controls are required for isolation in multi-tenant clusters.
 
 
</details>

### 8. Which additional Kubernetes security measures are needed to enforce full multi-tenant isolation in containerized AI clusters?

- [ ] **A)** Enforce Pod Security Standards.
- [ ] **B)** Use Kubernetes namespaces.
- [ ] **C)** Run containers without privilege escalation.
- [ ] **D)** Trust Docker's default isolation only.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Multi-tenant clusters require namespace isolation, pod security standards, and non-privileged containers because Docker's default isolation is insufficient.
 
 
</details>

### 9. The Kubernetes manifest runs a privileged container. In a shared AI cluster, why is this a concern despite Docker's isolation?

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: tenant-a
spec:
  containers:
  - name: ml
    image: tensorflow/tensorflow:latest
    securityContext:
      privileged: true

```

- [ ] **A)** Privileged containers can access host resources.
- [ ] **B)** The latest tag may change.
- [ ] **C)** The GPU driver is missing.
- [ ] **D)** Checkpointing is not enabled.

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A privileged container has broad access to host resources, weakening tenant isolation and increasing risk in shared clusters.
 
 
</details>


---

### **Cluster Administration**

### 10. In a GPU-accelerated container deployment, where must the NVIDIA kernel driver be installed for the GPUs to work?

- [ ] **A)** Inside the container image
- [ ] **B)** On the host operating system
- [ ] **C)** In a Kubernetes ConfigMap
- [ ] **D)** On a shared network filesystem

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> The NVIDIA driver must be installed on the host; containers use the driver through the container runtime instead of bundling the kernel driver.
 
 
</details>

### 11. Which practices help prevent reproducibility problems caused by the volatile 'latest' image tag in GPU workloads?

- [ ] **A)** Pin images to a specific version or digest
- [ ] **B)** Use an immutable registry that prevents tag overwrites
- [ ] **C)** Review image changes before allowing updates
- [ ] **D)** Always select images tagged 'latest' to get fixes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> The 'latest' tag is a mutable pointer; using a digest or fixed version and immutable registries ensures a deployment remains reproducible.
 
 
</details>

### 12. The command shown in the code block changes the number of running instances. Which operational concept does this represent?

```bash
kubectl scale deployment gpu-training --replicas=4

```

- [ ] **A)** Scaling
- [ ] **B)** Scheduling
- [ ] **C)** Checkpointing
- [ ] **D)** Preemption

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Scaling changes the number of replicas, while scheduling decides where those replicas are placed.
 
 
</details>

### 13. When running containers in a multi-tenant GPU cluster, why is Docker by itself not considered a strong security boundary?

- [ ] **A)** Containers share the host kernel and can be affected by privilege escalation
- [ ] **B)** Docker completely isolates all hardware resources
- [ ] **C)** Containers are virtual machines with hypervisor isolation
- [ ] **D)** Docker automatically encrypts inter-container traffic

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Containers share a host kernel; Docker alone does not enforce tenant isolation, so additional security controls are required.
 
 
</details>

### 14. Which conditions are necessary to make a GPU workload resumable after a node is preempted?

- [ ] **A)** The application supports checkpoint and restore
- [ ] **B)** Checkpoints are written to persistent or shared storage
- [ ] **C)** The workload uses the 'latest' image tag
- [ ] **D)** The GPU driver is installed only in the container

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The application must be able to save state, and that state must survive preemption on persistent storage, for resumption to work.
 
 
</details>

### 15. The command in the code block reports the connection layout of GPUs. Which administrative concern does it address?

```bash
nvidia-smi topo -m

```

- [ ] **A)** Hardware topology awareness
- [ ] **B)** Container image reproducibility
- [ ] **C)** Multi-tenant security isolation
- [ ] **D)** GPU driver installation path

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The nvidia-smi topo -m command displays GPU and NVLink/PCIe topology, helping the scheduler place jobs based on actual hardware connections.
 
 
</details>

### 16. Which component is responsible for loading the NVIDIA kernel driver on a GPU cluster node?

- [ ] **A)** Host OS kernel module
- [ ] **B)** Docker image layer
- [ ] **C)** Kubernetes dashboard plugin
- [ ] **D)** Container runtime plugin

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The host kernel module is loaded by the node's operating system. The NVIDIA container runtime depends on that host driver.
 
 
</details>


---

### **Troubleshooting and Optimization**

### 17. In a Kubernetes cluster with GPU nodes, where must the NVIDIA kernel driver be installed when running containerized AI workloads?

- [ ] **A)** On the host operating system
- [ ] **B)** Inside the container image
- [ ] **C)** In the container runtime's user namespace
- [ ] **D)** On a mounted network filesystem

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The NVIDIA driver is a kernel module that must match the host kernel. GPU containers only need CUDA libraries and the NVIDIA Container Toolkit.
 
 
</details>

### 18. Which two components are required on a host to run NVIDIA GPU containers with the NVIDIA Container Toolkit?

- [ ] **A)** NVIDIA driver installed on the host
- [ ] **B)** NVIDIA Container Toolkit configured
- [ ] **C)** The latest container image tag
- [ ] **D)** A hypervisor such as KVM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> The host needs the NVIDIA driver and the NVIDIA Container Toolkit. The container image can carry CUDA libraries, but the kernel driver and runtime integration belong on the host.
 
 
</details>

### 19. Review this Dockerfile. What is the main reason the installed driver package will not work as intended in a container?

```dockerfile
FROM nvidia/cuda:12.2-base
RUN apt-get update && apt-get install -y nvidia-driver-535
CMD ["nvidia-smi"]
```

- [ ] **A)** Kernel driver cannot load inside a container
- [ ] **B)** Container GPU memory is too small
- [ ] **C)** Image tag must be latest
- [ ] **D)** Driver requires internet access at runtime

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Container images share the host kernel, so a kernel driver package installed inside a container cannot load. The driver must be present on the host and matched to the host kernel.
 
 
</details>

### 20. Why is relying on an image tagged 'latest' risky for production NVIDIA GPU workloads in a shared cluster?

- [ ] **A)** It may point to a different image
- [ ] **B)** It always builds the smallest image
- [ ] **C)** It does not support CUDA
- [ ] **D)** It cannot run on Kubernetes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A mutable tag like 'latest' can move to a newer build, making the environment different from the one used during validation.
 
 
</details>

### 21. Which two practices help prevent reproducibility problems caused by mutable container tags in GPU deployments?

- [ ] **A)** Pin the image by digest
- [ ] **B)** Use a specific version tag
- [ ] **C)** Always use the latest tag
- [ ] **D)** Store images only in local cache

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Pinning to a digest or a specific version tag guarantees the same image is used. Mutable tags and local cache are not reliable for reproducibility.
 
 
</details>

### 22. This Kubernetes Deployment uses a mutable image reference for its GPU workload. Which risk should the operator identify?

```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: gpu-inference
spec:
  template:
    spec:
      containers:
      - name: cuda
        image: nvidia/cuda:latest
        resources:
          limits:
            nvidia.com/gpu: 1

```

- [ ] **A)** The image can change without a version change
- [ ] **B)** The container will not schedule on GPU nodes
- [ ] **C)** The Deployment will scale to zero
- [ ] **D)** The driver is installed in a sidecar

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The 'latest' tag is mutable, so a redeploy can pull a different version of the image, leading to unreproducible behavior.
 
 
</details>

### 23. Why is a Docker container not considered a strong security boundary for untrusted multi-tenant GPU workloads on shared infrastructure?

- [ ] **A)** Containers share the host kernel
- [ ] **B)** Containers have a separate kernel
- [ ] **C)** Images include security patches
- [ ] **D)** Docker blocks all host device access

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Docker containers use the host kernel. If a container escapes, the host kernel can be exposed, so stronger isolation is required for untrusted tenants.
 
 
</details>


---

### **Workload Management**

### 24. In a containerized GPU workload, where must the NVIDIA driver be installed for the container to access the GPU?

- [ ] **A)** On the host machine
- [ ] **B)** Inside the container image
- [ ] **C)** In the application code
- [ ] **D)** In the cluster network

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The NVIDIA driver must be installed on the host OS; the NVIDIA Container Toolkit enables the container to use the host driver.
 
 
</details>

### 25. Which statements about the container image tag 'latest' are correct when managing production AI workloads?

- [ ] **A)** It can change over time
- [ ] **B)** It is immutable
- [ ] **C)** Pinning a digest improves reproducibility
- [ ] **D)** It is always the stable release

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> 'latest' is a mutable tag that may move to newer builds. Pinning an image by digest or exact version provides stable, reproducible workloads.
 
 
</details>

### 26. Review the command in the code block. Where is the NVIDIA driver that supports this containerized GPU workload installed?

```bash
docker run --rm --gpus all nvidia/cuda:12.0-base-ubuntu20.04 nvidia-smi
```

- [ ] **A)** The NVIDIA driver
- [ ] **B)** The CUDA application
- [ ] **C)** The container registry
- [ ] **D)** The overlay network

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command starts a CUDA container that calls nvidia-smi. The host must provide the NVIDIA driver; the container uses it through the container toolkit.
 
 
</details>

### 27. What is a correct statement about Docker's security boundary in a shared multi-tenant AI environment?

- [ ] **A)** Containers share the host kernel
- [ ] **B)** Containers match hardware virtualization isolation
- [ ] **C)** Docker removes kernel security risk
- [ ] **D)** Containers each have their own kernel

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Docker containers share the host OS kernel, so a kernel or daemon vulnerability can affect all tenants. This is a critical security boundary consideration.
 
 
</details>

### 28. Select the activities that are characteristic of scheduling rather than scaling in a GPU cluster.

- [ ] **A)** Placing a job on a suitable GPU
- [ ] **B)** Adding a node to the cluster
- [ ] **C)** Assigning work to free GPUs
- [ ] **D)** Increasing replica count

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, C**
 
> 💡  **Explanation** 
> 
> Scheduling places individual workloads onto available resources. Scaling changes the total amount of resources or replicas by adding or removing nodes.
 
 
</details>

### 29. The command in the code block changes a deployment's replica count. Which workload management operation does it represent?

```bash
kubectl scale deployment inference-server --replicas=5
```

- [ ] **A)** Scaling
- [ ] **B)** Scheduling
- [ ] **C)** Checkpointing
- [ ] **D)** Preemption

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Changing the replica count changes capacity, so it is scaling. Scheduling would decide where each replica runs under resource constraints.
 
 
</details>

### 30. Why is checkpointing essential for deep learning workloads that may be preempted by a scheduler?

- [ ] **A)** It lets the workload resume from saved state
- [ ] **B)** It increases GPU clock speed
- [ ] **C)** It prevents scheduler preemption
- [ ] **D)** It removes the need for model weights

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Checkpointing periodically saves state so preempted workloads can restart from the last checkpoint, minimizing lost computation and allowing resumption.
 
 
</details>
