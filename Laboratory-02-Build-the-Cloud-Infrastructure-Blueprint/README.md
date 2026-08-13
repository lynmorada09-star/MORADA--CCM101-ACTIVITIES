# Laboratory 02 – Build the Cloud Infrastructure Blueprint

Mission Overview

This laboratory investigates the major components of cloud infrastructure and documents how compute, storage, networking, and operating system resources work together in a Linux environment.

## Objectives

- Investigate hardware and software resources in a Linux environment.
- Identify compute, storage, networking, and operating system resources.
- Understand how these infrastructure components relate to cloud computing.
- Compare equivalent infrastructure services offered by AWS, Microsoft Azure, and Google Cloud Platform.
- Design a simple cloud infrastructure blueprint.

## Cloud Infrastructure Components

### Compute Resources

The KillerCoda Linux environment uses an Intel Xeon E312xx (Sandy Bridge, IBRS update) processor with 1 CPU core and 1.9 GiB of RAM. These resources provide the processing and memory needed to run the Linux environment and execute applications and commands.

### Storage Resources

The environment provides a 20 GB virtual disk identified as `/dev/vda`. The main filesystem `/dev/vda1` has a capacity of approximately 19 GB and is mounted at `/`.

### Networking Resources

The main network interface is `enp1s0`, which uses the IPv4 address `172.30.1.2/24`. The environment also has a Docker network interface with the address `172.17.0.1/16`.

### Operating System

The operating system is Ubuntu 24.04.4 LTS (Noble Numbat), running kernel version `6.8.0-136-generic`.

## Tools Used

- KillerCoda
- Linux Terminal
- GitHub
- Markdown
- Draw.io

## Linux Commands Executed

```bash
cat /etc/os-release
uname -r
lscpu
nproc
free -h
lsblk
df -h
findmnt
hostname
hostname -I
ip addr
