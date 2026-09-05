<table width="100%">
  <tr>
    <td align="center" valign="middle" width="50%">
      <p align="center"><img src="https://pub-6a9f8dede1194a7786cba69e7dcdad9f.r2.dev/certifications/EC-Council/Computer%20Hacking%20Forensic%20Investigator.png" width="50%"></p>
    </td>
    <td align="center" valign="middle" width="50%">
      <h1>Computer Hacking Forensic Investigator</h1>
    </td>
  </tr>
</table>

## 📑 Table of Contents

- [Cloud/IoT Forensics](#cloud-iot-forensics) (2 questions)
- [Digital Evidence](#digital-evidence) (3 questions)
- [Digital Forensics](#digital-forensics) (5 questions)
- [Forensic Science](#forensic-science) (2 questions)
- [Forensics Investigation Process](#forensics-investigation-process) (4 questions)
- [Malware Forensics](#malware-forensics) (3 questions)
- [Network Forensics](#network-forensics) (3 questions)
- [Procedures and Methodology](#procedures-and-methodology) (3 questions)
- [Reporting and Testimony](#reporting-and-testimony) (1 questions)
- [Tools/Systems/Programs](#tools-systems-programs) (4 questions)

## 📋 Exam Information

| Field | Value |
|-------|-------|
| Total Questions | 30 |
| Level | Foundation |
| Exported At | 2026-09-04T23:44:35.106Z |
| Domains | 10 |

## 📊 Domain Distribution

| Domain | Questions |
|--------|-----------|
| Cloud/IoT Forensics | 2 |
| Digital Evidence | 3 |
| Digital Forensics | 5 |
| Forensic Science | 2 |
| Forensics Investigation Process | 4 |
| Malware Forensics | 3 |
| Network Forensics | 3 |
| Procedures and Methodology | 3 |
| Reporting and Testimony | 1 |
| Tools/Systems/Programs | 4 |

---

### **Cloud/IoT Forensics**

### 1. During a live forensic response, which action must be performed first to preserve the most ephemeral data?

- [ ] **A)** Capture the contents of RAM
- [ ] **B)** Pull the power plug to protect the hard drive
- [ ] **C)** Create a bit-stream image of the internal SSD
- [ ] **D)** Photograph and document the physical hardware

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Volatile evidence in RAM is lost when power is removed; it is the highest priority in the Order of Volatility.
 
 
</details>

### 2. Select all of the following that are examples of non-volatile evidence.

- [ ] **A)** Solid-state drive (SSD)
- [ ] **B)** USB flash drive
- [ ] **C)** RAM
- [ ] **D)** CPU cache

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Non-volatile evidence persists without power; SSDs and USB flash drives retain data. RAM and CPU cache are volatile and lose data when power is removed.
 
 
</details>


---

### **Digital Evidence**

### 3. In a digital forensic investigation, which of the following statements correctly describes volatile evidence that must be collected first?

- [ ] **A)** Lost when power is removed
- [ ] **B)** Remains on a hard drive after shutdown
- [ ] **C)** Hidden within image files
- [ ] **D)** Physical hardware used in crime

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Volatile evidence resides in temporary storage such as RAM, CPU registers, and cache, so it is lost when power is removed.
 
 
</details>

### 4. Which of the following items are examples of non-volatile evidence that remain intact after the system is powered down? Select all that apply.

- [ ] **A)** Solid-state drive (SSD)
- [ ] **B)** Optical media
- [ ] **C)** Random Access Memory (RAM)
- [ ] **D)** USB flash drive

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Non-volatile evidence remains intact after power is removed; SSDs, optical media, and USB drives persist, while RAM is volatile.
 
 
</details>

### 5. During a forensic acquisition, an examiner runs the command shown in the exhibit. What is the primary purpose of this command?

```bash
sha256sum original.dd forensic.dd
```

- [ ] **A)** Verifying acquisition integrity by hashing
- [ ] **B)** Encrypting evidence for confidentiality
- [ ] **C)** Creating a compressed evidence archive
- [ ] **D)** Generating file system metadata

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The command compares hash values; matching hashes prove the forensic copy is an exact, unaltered duplicate of the original.
 
 
</details>


---

### **Digital Forensics**

### 6. Which category of digital evidence is permanently lost as soon as a computer loses power?

- [ ] **A)** Volatile evidence
- [ ] **B)** Non-volatile evidence
- [ ] **C)** Latent evidence
- [ ] **D)** Physical evidence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Volatile evidence resides in temporary storage such as RAM, CPU registers, and cache, and is lost when power is removed.
 
 
</details>

### 7. Which of the following are examples of non-volatile evidence? Select all that apply.

- [ ] **A)** Hard disk drive
- [ ] **B)** Solid-state drive
- [ ] **C)** RAM contents
- [ ] **D)** CPU cache

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Hard disk drives and SSDs are non-volatile storage. RAM and CPU cache are volatile and lose data when power is removed.
 
 
</details>

### 8. The provided code block shows a live system acquisition. Why is the RAM dump captured before any disk acquisition?

```bash
#!/bin/bash
echo "Preserving live system data..."
sudo dd if=/dev/mem of=/evidence/ram_dump.mem bs=512 conv=noerror,sync
sudo sha256sum /evidence/ram_dump.mem > /evidence/ram_hash.txt
echo "RAM captured."
```

- [ ] **A)** Because RAM is volatile and would be lost during shutdown
- [ ] **B)** Because the hard drive is less important
- [ ] **C)** Because RAM contains only metadata
- [ ] **D)** Because the Order of Volatility requires disk capture first

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> RAM is volatile and contains active processes, network connections, and encryption keys. It must be captured before power loss.
 
 
</details>

### 9. Which principle requires continuous and chronological documentation of evidence movement?

- [ ] **A)** Chain of Custody
- [ ] **B)** Write Blocking
- [ ] **C)** Bit-stream Imaging
- [ ] **D)** Hash Verification

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Chain of custody is a continuous chronological log that tracks evidence movement, handling, and control. Any gap can invalidate evidence.
 
 
</details>

### 10. Which statements accurately describe bit-stream imaging? Select all that apply.

- [ ] **A)** It creates a sector-by-sector, bit-for-bit copy
- [ ] **B)** It captures deleted files and unallocated space
- [ ] **C)** It only copies active user files
- [ ] **D)** It updates access timestamps on the original drive

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> Bit-stream imaging copies the entire physical drive sector-by-sector, including hidden and deleted data in unallocated space.
 
 
</details>


---

### **Forensic Science**

### 11. Which type of evidence is lost when power is removed from a device?

- [ ] **A)** Volatile evidence
- [ ] **B)** Non-volatile evidence
- [ ] **C)** Latent evidence
- [ ] **D)** Physical evidence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Volatile evidence resides in temporary storage such as RAM and CPU registers. It is irrecoverably lost when power is removed, so it must be captured first.
 
 
</details>

### 12. Which of the following are classified as non-volatile evidence? Select all that apply.

- [ ] **A)** Solid-state drive
- [ ] **B)** Optical disc
- [ ] **C)** RAM contents
- [ ] **D)** USB flash drive

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Non-volatile evidence includes data on hard drives, SSDs, optical media, and USB flash drives. RAM is volatile because it requires continuous power to retain data.
 
 
</details>


---

### **Forensics Investigation Process**

### 13. What type of evidence is lost when power is removed from a device?

- [ ] **A)** Volatile evidence
- [ ] **B)** Non-volatile evidence
- [ ] **C)** Latent evidence
- [ ] **D)** Physical evidence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Volatile evidence resides in RAM, CPU registers, and cache, and is permanently lost when power is removed.
 
 
</details>

### 14. Which items are examples of volatile evidence? Select all that apply.

- [ ] **A)** Active network connections
- [ ] **B)** Decrypted passwords in RAM
- [ ] **C)** CPU registers
- [ ] **D)** Files on an SSD

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Active network connections, decrypted passwords, and CPU registers are volatile. Files on an SSD are non-volatile and persist after power loss.
 
 
</details>

### 15. Review the Python code block. What will happen to the hash output if a single bit changes in evidence.bin?

```python
import hashlib

def hash_file(path):
    h = hashlib.sha256()
    with open(path, 'rb') as f:
        for chunk in iter(lambda: f.read(4096), b''):
            h.update(chunk)
    return h.hexdigest()

print(hash_file('evidence.bin'))
```

- [ ] **A)** A completely different hash is produced
- [ ] **B)** Only one character of the hash changes
- [ ] **C)** The hash remains identical
- [ ] **D)** The hash algorithm returns an error

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Hashing exhibits the avalanche effect: any small input change produces a drastically different digest.
 
 
</details>

### 16. Which category of evidence remains intact even after the system is powered down?

- [ ] **A)** Non-volatile evidence
- [ ] **B)** Volatile evidence
- [ ] **C)** Network connections
- [ ] **D)** Running processes

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Non-volatile evidence, such as hard drives and SSDs, persists after power removal and provides long-term history.
 
 
</details>


---

### **Malware Forensics**

### 17. Which category of digital evidence is lost as soon as power is removed from a device?

- [ ] **A)** Volatile evidence
- [ ] **B)** Non-volatile evidence
- [ ] **C)** Latent evidence
- [ ] **D)** Physical evidence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Volatile evidence resides in RAM, caches, and CPU registers and is permanently lost when power is removed; therefore it must be captured first.
 
 
</details>

### 18. Which of which of these are examples of non-volatile evidence? Select all that apply.

- [ ] **A)** Hard drives
- [ ] **B)** SSDs
- [ ] **C)** USB flash drives
- [ ] **D)** RAM

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Non-volatile evidence remains intact after power-off; hard drives, SSDs, and USB flash drives persist, while RAM is volatile and loses data.
 
 
</details>

### 19. Examine the file listing in the code block. Which metadata category includes the date and time displayed?

```bash
-rw-r--r-- 1 alice staff 1024 Jan 12 10:23 report.docx
```

- [ ] **A)** MAC timestamp
- [ ] **B)** Exif data
- [ ] **C)** Cryptographic hash
- [ ] **D)** File ownership

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The date and time in a file listing correspond to MAC (Modified, Accessed, Created) timestamps, not hash values or file ownership.
 
 
</details>


---

### **Network Forensics**

### 20. According to the Order of Volatility, which type of evidence must be captured first when investigating a live system?

- [ ] **A)** Volatile evidence stored in RAM
- [ ] **B)** Non-volatile evidence on the hard drive
- [ ] **C)** Latent evidence in unallocated space
- [ ] **D)** Physical evidence such as a router

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Volatile evidence, such as RAM contents, is lost when power is removed, so it must be collected first according to the Order of Volatility.
 
 
</details>

### 21. Which of the following are examples of volatile evidence that exist in temporary storage? (Select all that apply)

- [ ] **A)** Data in RAM
- [ ] **B)** CPU registers
- [ ] **C)** Cache memory
- [ ] **D)** Data on an SSD

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, C**
 
> 💡  **Explanation** 
> 
> Volatile evidence resides in RAM, CPU registers, and cache, and it is lost when power is removed. SSDs retain data after power-off.
 
 
</details>

### 22. Examine the file listing shown in the code block. Which forensic metadata category is represented by the output?

```bash
$ stat /evidence/suspect.txt
  File: /evidence/suspect.txt
  Size: 1024        Blocks: 8          IO Block: 4096   regular file
Access: 2024-05-01 10:15:30.000000000 +0000
Modify: 2024-05-01 09:12:45.000000000 +0000
Change: 2024-05-01 09:15:02.000000000 +0000
```

- [ ] **A)** MAC timestamps
- [ ] **B)** Exif data
- [ ] **C)** Email header information
- [ ] **D)** Cryptographic hash values

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The stat output shows Access, Modify, and Change times, which are the MAC timestamps used to build a forensic timeline.
 
 
</details>


---

### **Procedures and Methodology**

### 23. Which type of evidence disappears immediately when power is removed from a device?

- [ ] **A)** Volatile Evidence
- [ ] **B)** Non-Volatile Evidence
- [ ] **C)** Latent Evidence
- [ ] **D)** Physical Evidence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Volatile evidence resides in RAM, CPU registers, and cache. It is lost when power is removed, so it must be captured first.
 
 
</details>

### 24. Select TWO examples of volatile storage where data is lost when the system loses power.

- [ ] **A)** RAM
- [ ] **B)** CPU registers
- [ ] **C)** Hard disk
- [ ] **D)** Solid-state drive

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B**
 
> 💡  **Explanation** 
> 
> RAM and CPU registers are temporary storage; hard disks and SSDs retain data after power loss, making them non-volatile.
 
 
</details>

### 25. Review the acquisition script in the code block. Why is this procedure considered forensically unsound for preserving the original storage media?

```bash
#!/bin/bash
# Acquire evidence
dd if=/dev/mem of=/evidence/ram.bin
netstat -an > /evidence/net.txt
cp -r /mnt/evidence /evidence/copy
```

- [ ] **A)** It uses dd to capture RAM
- [ ] **B)** It performs a standard file copy instead of a bit-stream image
- [ ] **C)** It records network connections before RAM
- [ ] **D)** It writes the acquired data to the wrong directory

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: B**
 
> 💡  **Explanation** 
> 
> A standard file copy only stores active files and alters timestamps. A forensically sound duplicate requires bit-stream imaging of the entire physical drive.
 
 
</details>


---

### **Reporting and Testimony**

### 26. Which type of evidence is immediately lost when a device loses power?

- [ ] **A)** Volatile evidence
- [ ] **B)** Non-volatile evidence
- [ ] **C)** Latent evidence
- [ ] **D)** Physical evidence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Volatile evidence is stored in RAM, CPU registers, or cache and is destroyed when power is removed, making it the highest collection priority.
 
 
</details>


---

### **Tools/Systems/Programs**

### 27. Which type of evidence is permanently destroyed as soon as a device loses power?

- [ ] **A)** Volatile evidence
- [ ] **B)** Non-volatile evidence
- [ ] **C)** Latent evidence
- [ ] **D)** Physical evidence

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> Volatile evidence resides in RAM, CPU registers, and cache, so removing power destroys it instantly.
 
 
</details>

### 28. Which storage media qualify as non-volatile evidence sources? Select all that apply.

- [ ] **A)** Hard disk drive
- [ ] **B)** Solid-state drive
- [ ] **C)** Random access memory content
- [ ] **D)** USB flash drive

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A, B, D**
 
> 💡  **Explanation** 
> 
> Hard drives, SSDs, and USB flash drives retain data without power; RAM content is volatile.
 
 
</details>

### 29. Inspect the command-line snippet. Which forensic acquisition process is being performed?

```bash
dd if=/dev/sda of=/evidence/image.dd bs=4M conv=noerror,sync
```

- [ ] **A)** Bit-stream imaging
- [ ] **B)** File copy
- [ ] **C)** Write blocking
- [ ] **D)** Hash verification

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> The dd command with a raw device and a separate output creates a sector-by-sector bit-stream image.
 
 
</details>

### 30. What is the primary function of a hardware write blocker in forensic acquisitions?

- [ ] **A)** Prevents any writes to original media
- [ ] **B)** Encrypts the original drive
- [ ] **C)** Speeds up the imaging process
- [ ] **D)** Recovers deleted files

<details>
<summary> 🔍 Reveal Answer</summary>
   
#### **✅ Correct Answer: A**
 
> 💡  **Explanation** 
> 
> A certified hardware write blocker physically blocks all write operations, preserving the original evidence.
 
 
</details>
