# 01 — Introduction to Linux

## 1. What is Linux?

Linux is an open-source, Unix-like operating system kernel.

The Linux kernel manages communication between computer hardware
and software.

A complete Linux operating system combines the Linux kernel
with system utilities, libraries, and applications.

Examples:
- Red Hat Enterprise Linux (RHEL)
- Ubuntu
- Debian
- Fedora
- Rocky Linux
- AlmaLinux

## 2. What is an Operating System?

An operating system (OS) is system software that manages
hardware resources and provides services to applications.

### Main Functions

- Process management
- Memory management
- File management
- Device management
- Security
- Networking

## 3. Why is Linux Important?

Linux is widely used in:

- Web servers
- Cloud computing
- DevOps environments
- Supercomputers
- Embedded systems
- Networking infrastructure
- Container platforms

### Advantages of Linux

1. Open-source
2. Highly customizable
3. Stable and reliable
4. Secure when properly configured
5. Suitable for automation
6. Strong command-line tools

## 4. Linux vs Windows

| Feature | Linux | Windows |
|---|---|---|
| Kernel | Linux kernel | Windows NT kernel |
| Source code | Open-source kernel | Proprietary |
| Common interface | CLI and GUI | GUI and CLI |
| Package management | DNF, APT, RPM | Winget, MSI, MSIX |
| Common server uses | Web, cloud, databases | Active Directory, enterprise applications |
| Customization | Extensive | Varies by edition |

Both operating systems are used in enterprise IT environments.

## 5. Linux Distributions

A Linux distribution is a complete operating system
built around the Linux kernel.

### Popular Distributions

**RHEL**
- Enterprise Linux distribution
- Commercial support
- Common in enterprise environments

**Ubuntu**
- Debian-based distribution
- Popular for desktops, servers, and cloud environments

**Rocky Linux**
- Enterprise Linux distribution
- Designed for compatibility with RHEL

**AlmaLinux**
- Community-driven enterprise Linux distribution

**Fedora**
- Community Linux distribution
- Often introduces newer technologies

## 6. Basic Linux Commands

### Display Kernel Information

```bash
uname -r
```

### Display System Information

```bash
uname -a
```

### Check Operating System Version

```bash
cat /etc/os-release
```

### Display Hostname

```bash
hostname
```

### Check Current User

```bash
whoami
```

### Display Current Date

```bash
date
```

### Check System Uptime

```bash
uptime
```

## 7. Hands-on Practice

### Lab 01: Identify Linux System Information

**Objective:**

Identify the Linux distribution, kernel version,
hostname, and current user.

**Environment:**

- Operating System: RHEL / Rocky Linux / AlmaLinux
- Platform: VMware Workstation

**Steps:**

1. Open the Linux terminal.
2. Execute `cat /etc/os-release`.
3. Execute `uname -r`.
4. Execute `hostname`.
5. Execute `whoami`.
6. Record the output.

**Expected Result:**

The terminal displays the operating system details,
kernel version, hostname, and current username.

**Verification:**

Compare the command outputs with the configured
system information.

## 8. Interview Questions

**Q1. What is Linux?**

Linux is an open-source, Unix-like operating system kernel.

**Q2. What is a Linux distribution?**

A complete operating system built around the Linux kernel.

**Q3. What is the difference between Linux and Windows?**

Linux distributions commonly use an open-source kernel,
while Windows uses Microsoft's proprietary NT kernel.
Both support command-line and graphical administration.

**Q4. How do you check the Linux kernel version?**

```bash
uname -r
```

**Q5. How do you identify the Linux distribution?**

```bash
cat /etc/os-release
```

## 9. References

- Red Hat Enterprise Linux Documentation
- Linux Kernel Documentation
- Linux Manual Pages

## 10. Learning Outcome

After completing this topic, learners should understand:

- What Linux is
- What an operating system does
- Why Linux is used
- Common Linux distributions
- Basic Linux system information commands

---

**Status:** Theory documented; practical verification pending.
