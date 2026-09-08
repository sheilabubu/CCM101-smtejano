# Laboratory 03 – Multi-Cloud Explorer

## Linux Server Investigation

I launched an Ubuntu Linux Playground using KillerCoda and used Linux commands to identify the operating system, CPU information, memory, and disk space of the server.

## 1. Operating System

**Command used:**

```bash
cat /etc/os-release
```

**Result:**

- Operating System: Ubuntu 24.04.4 LTS
- Version: 24.04
- Codename: Noble Numbat

The Linux server is running Ubuntu 24.04.4 LTS.

### Screenshot

<img width="1366" height="404" alt="killercoda-terminal1" src="https://github.com/user-attachments/assets/47352c2f-cc95-4694-934a-9b0a492ee05f" />


---

## 2. CPU Information

**Command used:**

```bash
lscpu
```

**Result:**

- Architecture: x86_64
- CPU Model: Intel Xeon E312xx (Sandy Bridge)
- Number of CPUs: 1
- CPU Frequency: 2.0 GHz

The server has one CPU based on an Intel Xeon E312xx processor.

### Screenshot

<img width="1366" height="683" alt="killercoda-terminal2" src="https://github.com/user-attachments/assets/8bb82e9c-b206-48de-939f-cc0a3122d8e8" />



<img width="1366" height="678" alt="killercoda-terminal2 1" src="https://github.com/user-attachments/assets/db5b2560-9b21-4bd2-a64f-39a50cec9836" />

---

## 3. Memory

**Command used:**

```bash
free -h
```

**Result:**

- Total Memory: 1.9 GiB
- Used Memory: 418 MiB
- Free Memory: 862 MiB
- Available Memory: 1.5 GiB
- Swap: 1.0 GiB

The Linux server has approximately 1.9 GiB of total memory.

### Screenshot

![Memory Information](screenshots/memory-information.png)

---

## 4. Disk Space

**Command used:**

```bash
df -h
```

**Result:**

- Root Filesystem Size: 19 GiB
- Used Space: 5.4 GiB
- Available Space: 13 GiB
- Usage: 30%

The main root filesystem has 19 GiB of storage, with approximately 13 GiB available.

### Screenshot

![Disk Space](screenshots/disk-information.png)

---

# Cloud Migration Options

If this Linux server were migrated to the cloud, it could be hosted using a virtual machine service from AWS, Microsoft Azure, or Google Cloud.

| Cloud Provider | Cloud Service | Purpose |
|---|---|---|
| AWS | Amazon EC2 | Hosts Linux virtual machines |
| Microsoft Azure | Azure Virtual Machines | Hosts Linux virtual machines |
| Google Cloud | Compute Engine | Hosts Linux virtual machines |

## AWS – Amazon EC2

Amazon EC2 could host this Linux server as a virtual machine. CPU, memory, storage, and other resources can be configured based on the server's requirements.

## Microsoft Azure – Azure Virtual Machines

Azure Virtual Machines could host this Linux server because Azure supports Linux operating systems. A VM size with suitable CPU and memory resources can be selected.

## Google Cloud – Compute Engine

Google Compute Engine could host this Linux server as a virtual machine. It supports Linux operating systems and provides configurable computing and storage resources.

## Conclusion

The Linux server can be migrated to AWS, Microsoft Azure, or Google Cloud because all three cloud providers offer virtual machine services that support Linux.

Based on the current server requirements of approximately 1 CPU, 1.9 GiB memory, and 19 GiB disk space, a small cloud virtual machine would be suitable for a similar basic workload. The exact VM size should depend on the application's actual resource requirements.

## References

- Amazon Web Services – AWS Documentation: https://docs.aws.amazon.com/
- Microsoft Azure – Azure Documentation: https://learn.microsoft.com/en-us/azure/
- Google Cloud – Google Cloud Documentation: https://cloud.google.com/docs
