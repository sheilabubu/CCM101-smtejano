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

<img width="1053" height="111" alt="killercoda-terminal3" src="https://github.com/user-attachments/assets/479573bd-62fd-4446-a652-eac33af98f17" />


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

<img width="1366" height="189" alt="killercoda-terminal4" src="https://github.com/user-attachments/assets/ae31af54-962f-4b56-b0e1-f9d994667486" />


---

# Cloud Migration Options

If this Linux server were migrated to the cloud, it could be hosted using a virtual machine service from AWS, Microsoft Azure, or Google Cloud.

| Cloud Provider | Cloud Service | Purpose |
|---|---|---|
| AWS | Amazon EC2 | Hosts Linux virtual machines |
| Microsoft Azure | Azure Virtual Machines | Hosts Linux virtual machines |
| Google Cloud | Compute Engine | Hosts Linux virtual machines |

