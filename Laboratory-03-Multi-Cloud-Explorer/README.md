# Checkpoint 7 – Linux Environment and Cloud Hosting

## Linux Environment

The Linux environment was inspected using the following commands:

```bash
cat /etc/os-release
lscpu
free -h
df -h
```

### Operating System

The KillerCoda environment is running:

* **Operating System:** Ubuntu 24.04.4 LTS
* **Version:** 24.04
* **Version Codename:** Noble Numbat
* **Architecture:** x86-64

### CPU Information

The system has the following CPU configuration:

* **Architecture:** x86-64
* **CPU:** Intel Xeon E312xx (Sandy Bridge, IBRS update)
* **CPU(s):** 1
* **Thread(s) per core:** 6
* **Core(s) per socket:** 1
* **Virtualization Type:** KVM

### Memory Information

According to the `free -h` command:

* **Total Memory:** 1.9 GiB
* **Used Memory:** 411 MiB
* **Free Memory:** 869 MiB
* **Available Memory:** 1.5 GiB
* **Swap:** 0 B

### Disk Space

According to the `df -h` command:

* **Filesystem:** `/dev/vda1`
* **Total Size:** 19G
* **Used:** 5.4G
* **Available:** 13G
* **Usage:** 30%
* **Mounted on:** `/`

## Cloud Hosting Options

The Linux environment can be hosted on any of the three major cloud platforms using their virtual machine services.

| Cloud Provider              | Virtual Machine Service |
| --------------------------- | ----------------------- |
| Amazon Web Services (AWS)   | Amazon EC2              |
| Microsoft Azure             | Azure Virtual Machines  |
| Google Cloud Platform (GCP) | Compute Engine          |

These virtual machine services can host Linux operating systems such as Ubuntu. They provide the computing resources needed to run applications, websites, databases, and other workloads in the cloud.

## Evidence

The following screenshots provide evidence of the Linux environment:

* `linux-os.png` – Operating system information
* `linux-cpu.png` – CPU information
* `linux-memory.png` – Memory information
* `linux-disk.png` – Disk space information
