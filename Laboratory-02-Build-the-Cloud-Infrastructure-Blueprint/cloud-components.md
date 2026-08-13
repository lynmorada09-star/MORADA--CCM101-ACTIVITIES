# Cloud Infrastructure Components

1. Compute Resources

##Example in the Linux Environment

The Linux environment uses an Intel Xeon E312xx (Sandy Bridge, IBRS update) CPU with 1 CPU core and 1.9 GiB of RAM.

### Purpose

Compute resources provide the processing power needed to run applications, execute commands, and perform computing tasks.

### Importance in Cloud Computing

Compute resources are important in cloud computing because they allow users to run applications, services, and workloads without needing to manage physical servers directly. Cloud providers can allocate and scale compute resources based on workload requirements.

### Relation to the KillerCoda Linux Environment

The KillerCoda environment provides a virtual Linux server with an Intel Xeon CPU, 1 CPU core, and 1.9 GiB of RAM. These resources allow the Linux operating system and commands used in the laboratory to run.

---

## 2. Storage Resources

### Example in the Linux Environment

The Linux environment has a 20 GB virtual disk identified as `/dev/vda`. The main filesystem is `/dev/vda1` with a size of 19 GB.

### Purpose

Storage resources are used to store the operating system, applications, configuration files, and other data.

### Importance in Cloud Computing

Storage is important in cloud computing because applications and services need a reliable place to store and retrieve data. Cloud storage also allows data to be managed independently from the compute resources.

### Relation to the KillerCoda Linux Environment

The KillerCoda environment provides a virtual 20 GB disk. The main filesystem `/dev/vda1` is mounted at `/` and is used by the Linux operating system to store system files and other data.

---

## 3. Networking Resources

### Example in the Linux Environment

The main network interface is `enp1s0` with the IPv4 address `172.30.1.2/24`.

### Purpose

Networking resources allow computers, servers, applications, and users to communicate with each other.

### Importance in Cloud Computing

Networking is important in cloud computing because cloud resources need to communicate with users, applications, databases, and other services. It also enables access to cloud-hosted applications and services.

### Relation to the KillerCoda Linux Environment

The KillerCoda Linux environment uses the `enp1s0` network interface with the IPv4 address `172.30.1.2/24`. This provides network connectivity for the virtual Linux environment.

---

## 4. Operating System

### Example in the Linux Environment

The operating system is Ubuntu 24.04.4 LTS (Noble Numbat), running kernel version `6.8.0-136-generic`.

### Purpose

The operating system manages the computer's hardware and provides an environment for applications and users to run.

### Importance in Cloud Computing

An operating system is important in cloud computing because it manages the underlying compute, memory, storage, networking, and applications running on a virtual machine or server.

### Relation to the KillerCoda Linux Environment

KillerCoda provides an Ubuntu 24.04.4 LTS Linux environment. The operating system manages the available CPU, memory, storage, and networking resources and allows us to investigate the cloud server using Linux commands.
