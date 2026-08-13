# Cloud Infrastructure Components

1. Compute Resources

### Example in the Linux Environment
The KillerCoda Linux environment uses an Intel Xeon E312xx (Sandy Bridge, IBRS update) processor with 1 CPU core and 1.9 GiB of RAM.

### Purpose
Compute resources provide processing power and memory needed to execute applications, services, and system tasks.

### Importance in Cloud Computing
Compute resources are important because they allow cloud users to run applications, virtual machines, and workloads on demand. Cloud providers can increase or decrease computing resources depending on user requirements.

### Relation to the KillerCoda Linux Environment
The KillerCoda environment provides virtual compute resources, including a CPU and RAM, that allow Ubuntu Linux and laboratory commands to run.

---

## 2. Storage Resources

### Example in the Linux Environment
The Linux environment contains a virtual disk (`/dev/vda`) with a capacity of 20 GB. The main filesystem (`/dev/vda1`) has a size of 19 GB.

### Purpose
Storage resources are used to save operating system files, applications, configuration files, and user data.

### Importance in Cloud Computing
Storage is important because cloud applications need reliable and scalable data storage. Cloud storage services provide persistent and accessible storage for systems and users.

### Relation to the KillerCoda Linux Environment
The Ubuntu environment stores files and system data on the `/dev/vda` virtual disk and uses mounted filesystems such as `/`, `/boot`, and `/boot/efi`.

---

## 3. Networking Resources

### Example in the Linux Environment
The primary network interface is `enp1s0` with the IP address `172.30.1.2/24`.

### Purpose
Networking resources allow communication between systems, users, applications, and cloud services.

### Importance in Cloud Computing
Networking is essential because cloud resources must communicate with each other and provide access to users over networks and the internet.

### Relation to the KillerCoda Linux Environment
The KillerCoda Linux environment uses the `enp1s0` network interface to provide network connectivity and communication.

---

## 4. Operating System

### Example in the Linux Environment
The operating system is Ubuntu 24.04.4 LTS (Noble Numbat) with kernel version `6.8.0-136-generic`.

### Purpose
The operating system manages hardware resources and provides a platform for applications and users.

### Importance in Cloud Computing
Operating systems are important because they manage compute, storage, networking, and applications running on cloud servers and virtual machines.

### Relation to the KillerCoda Linux Environment
Ubuntu Linux manages the CPU, memory, storage, and networking resources available in the KillerCoda environment.
