# Linux Learning Journey - Day 2

## Terminal Basics, Paths & Navigation

---

## 🎯 Objective

Learn how to navigate the Linux file system using terminal commands and understand how Linux paths work.

---

# 1. Terminal Basics

The Terminal is a command-line interface (CLI) used to communicate with Linux.

Instead of clicking folders with a mouse, we execute commands.

Example:

```bash
pwd
ls
cd
```

### Why Terminal?

* Faster than GUI
* Used on Linux servers
* Essential for DevOps, Cloud, Backend Development, and System Administration
* Supports automation through scripts

---

# 2. Root Directory (/)

Linux starts from a single top-level directory called the Root Directory.

```text
/
├── home
├── etc
├── var
├── usr
├── tmp
└── opt
```

Everything in Linux exists under `/`.

Move to Root Directory:

```bash
cd /
```

---

# 3. Present Working Directory (pwd)

Displays your current location.

```bash
pwd
```

Example:

```text
/home/munna
```

Meaning you are currently inside:

```text
/home/munna
```

---

# 4. List Files and Directories (ls)

Displays files and directories inside the current location.

```bash
ls
```

Example Output:

```text
Desktop
Documents
Downloads
Pictures
```

## Useful Options

### Long Listing

```bash
ls -l
```

Shows:

* Permissions
* Owner
* Size
* Date

### Hidden Files

```bash
ls -a
```

Shows hidden files such as:

```text
.bashrc
.profile
```

### Human Readable Sizes

```bash
ls -lh
```

---

# 5. Change Directory (cd)

Used to move between directories.

Move to Home Directory:

```bash
cd
```

or

```bash
cd ~
```

Move to Root Directory:

```bash
cd /
```

Move to Documents Directory:

```bash
cd Documents
```

Verify Location:

```bash
pwd
```

---

# 6. Absolute Path

An Absolute Path starts from the Root Directory (`/`).

Example:

```bash
cd /home/munna/Documents
```

Structure:

```text
/
└── home
    └── munna
         └── Documents
```

Absolute Path:

```text
/home/munna/Documents
```

---

# 7. Relative Path

A Relative Path starts from your current location.

Current Location:

```text
/home/munna
```

Move to Documents:

```bash
cd Documents
```

Linux automatically understands:

```text
/home/munna/Documents
```

---

# Absolute Path vs Relative Path

| Absolute Path       | Relative Path                 |
| ------------------- | ----------------------------- |
| Starts with `/`     | Starts from current directory |
| Full location       | Partial location              |
| Works from anywhere | Depends on current location   |

Examples:

```bash
cd /home/munna/Documents
```

```bash
cd Documents
```

---

# 8. Special Navigation Symbols

## Current Directory

```bash
cd .
```

No movement.

---

## Parent Directory

```bash
cd ..
```

Moves one level up.

Example:

```text
/home/munna/Documents
```

After:

```bash
cd ..
```

Result:

```text
/home/munna
```

---

## Two Levels Up

```bash
cd ../..
```

Example:

```text
/home/munna/Documents
```

Result:

```text
/home
```

---

# 9. Creating Directories

Create a directory:

```bash
mkdir company
```

Verify:

```bash
ls
```

Output:

```text
company
```

---

# Practical Commands

```bash
pwd

ls

cd /

pwd

cd ~

pwd

mkdir company

ls

cd company

pwd

cd ..

pwd
```

---

# Interview Questions

### 1. What does `pwd` stand for?

Print Working Directory.

### 2. What is the Root Directory?

The top-most directory represented by `/`.

### 3. What is the difference between Absolute and Relative Paths?

Absolute Path starts from `/`.

Relative Path starts from the current directory.

### 4. Which command lists files and directories?

```bash
ls
```

### 5. Which command changes directories?

```bash
cd
```

---

# Day 2 Summary

## Commands Learned

```bash
pwd
ls
ls -l
ls -a
ls -lh
cd
mkdir
```

## Concepts Learned

* Terminal Basics
* Root Directory
* Present Working Directory
* Absolute Path
* Relative Path
* Directory Navigation
* Creating Directories

---

