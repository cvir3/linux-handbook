# 🧾 WSL

### 🔹 What is WSL?
WSL (Windows Subsystem for Linux) lets you run a real Linux environment directly on Windows, without installing a virtual machine or dual-booting.

In simple terms:
- You are on Windows
- You open a terminal
- You run Linux commands like ls, grep, ssh, apt, docker, etc.
- It feels like Linux, but it runs inside Windows

With WSL, Windows and Linux work side by side.

### 🔹 Why use WSL?

**Main reasons people use WSL**
1. Run Linux tools on Windows

Many dev and DevOps tools are built for Linux:

- Docker

- Kubernetes (kubectl, helm)

- Terraform

- Ansible

- Bash scripts

- SSH, rsync, curl, grep, awk

- WSL lets you use all of these natively.

2. No virtual machine headache

Traditional VM problems:

- Heavy memory usage

- Slow startup

- Networking issues

**WSL:**

- Starts in seconds

- Uses fewer resources

- Shares files easily with Windows

3. Perfect for DevOps and Cloud work

Most cloud servers run Linux.
**Using WSL means:**

- Your local setup matches production

- Fewer “works on my machine” issues

4. Best of both worlds

You get:

- Windows apps (VS Code, browsers, Office)

- Linux shell and tooling

No switching systems.

### 🔹How WSL works (simple view)
- Windows hosts the system

- WSL runs a lightweight Linux kernel

- Linux runs in its own filesystem

- Windows and Linux can access each other’s files

Example:

- Windows path: **C:\Users\folder**

- Linux path: **/mnt/c/Users/folder**
---
### 🔹 Install WSL

    wsl --install
Restart the system after installation.

### 🔹 Install WSL Without Default Linux Distro
    wsl --install --no-distribution

### 🔹 Install Ubuntu on WSL
    wsl --list --online

### 🔹 Install a specific version:
    wsl --install -d Ubuntu-22.04

### 🔹 Launch Ubuntu
    wsl
### 🔹 Check WSL Status & Information
    wsl --list
### 🔹 Detailed view:
    wsl --list --verbose
### 🔹 Check WSL Version
    wsl --version
### 🔹 Check WSL Status
    wsl --status
### 🔹 Shutdown & Stop WSL
    wsl --shutdown
### 🔹 Stop a Specific Linux Distribution
    wsl --terminate Ubuntu
### 🔹 Restart WSL
    wsl --shutdown
    wsl
### 🔹 Uninstall Ubuntu (Linux Distribution)
    wsl --unregister Ubuntu

