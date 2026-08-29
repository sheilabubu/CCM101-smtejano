# Infrastructure Report

## Cloud Server Information

This report documents the information gathered from the Linux cloud server using the KillerCoda Playground.

| Information | Result |
|---|---|
| Operating System | Ubuntu 24.04.4 LTS |
| Kernel Version | 6.8.0-138-generic |
| CPU Model | Intel Xeon E312xx (Sandy Bridge, IBRS update) |
| Number of CPU Cores | 1 |
| Total RAM | 1.9 GiB |
| Disk Capacity | 19G |
| Hostname | ubuntu |
| IP Address | 172.30.1.2, 172.17.0.1 |

## Mounted File Systems

The mounted file systems were checked using the `df -h` command.

| File System | Size | Used | Available | Mounted On |
|---|---:|---:|---:|---|
| tmpfs | 191M | 100K | 190M | /run |
| /dev/vda1 | 19G | 5.4G | 13G | / |
| tmpfs | 952M | 84K | 952M | /dev/shm |
| tmpfs | 5.0M | 0 | 5.0M | /run/lock |
| /dev/vda16 | 881M | 703M | 178M | /boot |
| /dev/vda15 | 105M | 6.2M | 99M | /boot/efi |

## Linux Commands Used

The following commands were used to investigate the cloud server:

```bash
cat /etc/os-release
uname -r
lscpu | grep "Model name"
nproc
free -h
df -h /
df -h
hostname
hostname -I
