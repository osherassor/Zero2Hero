# 🧩 Virtualization & Containers

## 🧰 Virtualization Basics

### What is virtualization?
- Concept of abstraction
- Benefits: isolation, scalability, testing environments

### Hypervisors
- Type 1 (bare-metal) vs Type 2 (hosted)
- Examples: VMware ESXi, Microsoft Hyper-V, VirtualBox

### Guest OS vs Host OS

## 🖥️ Working with Virtual Machines

### Creating VMs
- ISO selection and installation
- Assigning virtual hardware: CPU, RAM, disk, network

### Snapshots and cloning
- Use cases for testing and recovery

### VM networking modes
- NAT
- Bridged
- Host-only

## 🧱 Containers Fundamentals

### What are containers?
- Difference from VMs
- Use of shared OS kernel

### Container engines
- Docker: image, container, volume, network
- Podman (rootless alternative)

### Dockerfile basics
- Image layering
- Build process

### Docker Compose overview

## 🕸️ Container Networking
- Bridge networks
- Host networking
- Overlay networks (for clustering)
- Port publishing and NAT

## 🔐 Security Considerations
- VM escape basics (concept only)
- Container isolation risks
- Namespaces and control groups (cgroups)
- Image scanning and hardening

## 🧪 Tools & Utilities

### Virtualization
- VirtualBox, VMware Workstation
- QEMU, KVM

### Containers
- Docker CLI
- Docker Desktop GUI
- `docker inspect`, `docker exec`, `docker logs`
