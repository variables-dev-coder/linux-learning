# Linux Learning Journey 🚀

## Phase 0 - Linux Mindset

### Day 1 - Linux Basics & Linux Mindset

---

# What is Linux?

Many beginners think Linux is an Operating System.

Technically:

**Linux = Kernel**

The Linux kernel is the core component that manages communication between hardware and software.

### Architecture

```text
Applications
     ↑
Linux Kernel
     ↑
Hardware
```

Example:

```text
Java Application
      ↓
Linux Kernel
      ↓
CPU / RAM / Disk
```

Applications never directly communicate with hardware.

The Linux kernel handles all communication.

---

# Responsibilities of the Linux Kernel

## 1. Process Management

The kernel controls running programs.

Examples:

* Java
* MySQL
* Docker
* Chrome

The kernel decides:

* Which process runs
* How much CPU it receives
* When it should stop

---

## 2. Memory Management

The kernel manages RAM allocation.

Example:

```text
Java      → 2GB
MySQL     → 1GB
Docker    → 1GB
```

The kernel prevents programs from interfering with each other.

---

## 3. File System Management

The kernel manages:

* Files
* Directories
* Storage
* Permissions

Example:

```bash
/home/munna/file.txt
```

---

## 4. Device Management

The kernel controls hardware devices:

* Keyboard
* Mouse
* USB Devices
* SSD/HDD
* Network Card

Using device drivers.

---

## 5. Security

The kernel enforces:

* User access
* Permissions
* Authentication
* Authorization

Examples:

```bash
chmod
chown
sudo
```

---

# Kernel vs Operating System

## Kernel

The core engine.

Responsible for:

* CPU
* RAM
* Storage
* Hardware Communication

Example:

```text
Linux Kernel
```

---

## Operating System

An Operating System includes:

```text
Linux Kernel
+
Shell
+
GNU Utilities
+
Package Manager
+
System Tools
```

Example:

* Ubuntu
* Debian
* Fedora
* RHEL

---

# Linux Distributions

A Linux Distribution (Distro) is a complete operating system built around the Linux kernel.

Formula:

```text
Linux Kernel
+
Software Packages
+
Package Manager
+
System Utilities
=
Linux Distribution
```

---

## Popular Linux Distributions

### Ubuntu

Best for beginners.

Used for:

* Learning
* Development
* Cloud Servers

---

### Debian

Known for:

* Stability
* Reliability

---

### Red Hat Enterprise Linux (RHEL)

Used by:

* Enterprises
* Banks
* Government Organizations

---

### Fedora

Provides latest Linux technologies.

---

### Arch Linux

Advanced and highly customizable.

---

# Why Companies Use Linux

## 1. Open Source

No expensive licensing fees.

---

## 2. Stability

Servers can run for months without rebooting.

---

## 3. Security

Strong:

* User Management
* File Permissions
* Firewall Support

---

## 4. Performance

Consumes fewer resources.

Suitable for:

* Servers
* Cloud Infrastructure
* Containers

---

## 5. Automation

Supports:

* Bash Scripts
* Python Automation
* DevOps Tools

---

## 6. Cloud Dominance

Most cloud infrastructure runs Linux.

Examples:

* AWS
* Azure
* Google Cloud

---

# Day 1 Commands

## System Information

```bash
uname -a
```

Displays:

* Kernel Name
* Kernel Version
* Architecture

---

## Current User

```bash
whoami
```

Displays logged-in user.

---

## Hostname

```bash
hostname
```

Displays system name.

---

## Date & Time

```bash
date
```

Displays current date and time.

---

## Calendar

```bash
cal
```

Displays calendar.

Note:

Some Linux distributions require:

```bash
sudo apt install ncal
```

---

# Practice Tasks

## Task 1

Run:

```bash
uname -a
```

Identify:

* Kernel Version
* Architecture

---

## Task 2

Run:

```bash
whoami
hostname
```

Identify:

* Current User
* Hostname

---

## Task 3

Run:

```bash
date
```

Identify:

* Date
* Time
* Timezone

---

## Task 4

Run:

```bash
cal
```

Observe current month calendar.

---

# Interview Questions

### What is Linux?

Linux is a kernel that manages communication between hardware and software.

---

### What is a Kernel?

A kernel is the core component of an operating system responsible for process, memory, device, and file management.

---

### Difference Between Kernel and Operating System?

Kernel is the core engine.

Operating System = Kernel + Tools + Utilities + Software.

---

### What is a Linux Distribution?

A complete operating system built around the Linux kernel.

Examples:

* Ubuntu
* Debian
* Fedora
* RHEL

---

### Why Do Companies Use Linux?

* Open Source
* Stable
* Secure
* High Performance
* Automation Friendly
* Cloud Dominance

---

# Day 1 Summary

✅ What Linux is

✅ What a Kernel is

✅ Kernel vs Operating System

✅ Linux Distributions

✅ Why Companies Use Linux

✅ Basic Linux Information Commands

---




**Next Topic:** Day 2 - Linux File System, Absolute Path, Relative Path, Root Directory
