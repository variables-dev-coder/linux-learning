# Linux Foundation - Day 4

## Goal
Master file and directory viewing commands in Linux.

---

# Commands Covered

- `pwd`
- `ls`
- `ls -l`
- `ls -a`
- `ls -la`

---

# 1. pwd (Print Working Directory)

## What is pwd?

Displays the full path of the current directory you are working in.

## Syntax

```bash
pwd
```

## Example

```bash
$ pwd

/home/munna/company/backend/java
```

## Output Explanation

```text
/
└── home
    └── munna
         └── company
              └── backend
                   └── java
```

Current location:

```bash
/home/munna/company/backend/java
```

---

## Why Use pwd?

Before executing commands like:

```bash
rm file.txt
```

Always verify your current directory:

```bash
pwd
```

This prevents accidental file deletion in the wrong location.

---

# 2. ls (List Files)

## What is ls?

Displays all visible files and directories inside the current directory.

## Syntax

```bash
ls
```

## Example

```bash
$ ls

backend
database
devops
```

---

## Directory Structure

```text
company/
├── backend
├── database
└── devops
```

Running:

```bash
ls
```

Output:

```bash
backend database devops
```

---

## List Another Directory

```bash
ls /home
```

Example Output:

```bash
munna
oracle
test
```

---

# 3. ls -l (Long Listing Format)

## What is ls -l?

Shows detailed information about files and directories.

## Syntax

```bash
ls -l
```

## Example

```bash
$ ls -l

drwxr-xr-x 2 munna munna 4096 Jun 4 backend
drwxr-xr-x 2 munna munna 4096 Jun 4 database
drwxr-xr-x 2 munna munna 4096 Jun 4 devops
```

---

# Understanding ls -l Output

Example:

```bash
drwxr-xr-x 2 munna munna 4096 Jun 4 backend
```

| Part | Meaning |
|--------|---------|
| d | Directory |
| rwx | Owner Permissions |
| r-x | Group Permissions |
| r-x | Others Permissions |
| 2 | Number of Links |
| munna | Owner |
| munna | Group |
| 4096 | Size (Bytes) |
| Jun 4 | Modified Date |
| backend | Directory Name |

---

## File Example

```bash
-rw-r--r-- 1 munna munna 1200 Jun 4 notes.txt
```

### Meaning

| Symbol | Description |
|----------|-------------|
| - | File |
| rw- | Owner Read/Write |
| r-- | Group Read |
| r-- | Others Read |

---

# 4. ls -a (Show Hidden Files)

## What is ls -a?

Displays all files including hidden files.

## Syntax

```bash
ls -a
```

## Example

```bash
$ ls -a

.
..
.git
.bashrc
backend
database
devops
```

---

# Hidden Files

Files beginning with a dot (`.`) are hidden.

Examples:

```bash
.git
.bashrc
.profile
.vscode
```

---

## Why Hidden Files Exist?

Hidden files usually store configuration settings.

Examples:

### Git Configuration

```bash
.git
```

Stores Git repository data.

### Bash Configuration

```bash
.bashrc
```

Stores terminal settings and aliases.

---

# Understanding . and ..

## Current Directory (.)

Represents the current directory.

Example:

```bash
cd .
```

No directory change occurs.

---

## Parent Directory (..)

Represents one level above the current directory.

Example:

```bash
cd ..
```

Current:

```text
/home/munna/company/backend
```

After:

```bash
cd ..
```

New Location:

```text
/home/munna/company
```

---

# ls -la

## What is ls -la?

Combines:

```bash
ls -l
```

and

```bash
ls -a
```

Shows:

- Hidden Files
- Permissions
- Owner
- Group
- Size
- Modified Date

## Syntax

```bash
ls -la
```

## Example

```bash
drwxr-xr-x 5 munna munna 4096 Jun 4 .
drwxr-xr-x 3 munna munna 4096 Jun 4 ..
-rw-r--r-- 1 munna munna 220 Jun 4 .bash_logout
-rw-r--r-- 1 munna munna 3771 Jun 4 .bashrc
```

---

# Practical Exercise

## Step 1

Check Current Location

```bash
pwd
```

---

## Step 2

Navigate to Company Folder

```bash
cd ~/company
```

---

## Step 3

List Directory Contents

```bash
ls
```

---

## Step 4

View Detailed Information

```bash
ls -l
```

---

## Step 5

Show Hidden Files

```bash
ls -a
```

---

## Step 6

Show Detailed Hidden Files

```bash
ls -la
```

---

# Engineer Challenge

Create the following structure:

```text
linux-practice/
├── java
├── mysql
├── docker
└── kubernetes
```

## Commands

```bash
mkdir linux-practice

cd linux-practice

mkdir java mysql docker kubernetes
```

---

## Verify Structure

```bash
pwd

ls

ls -l

ls -la
```

---

# Interview Questions

## Q1. What does pwd stand for?

**Answer:**

```text
Print Working Directory
```

---

## Q2. What is the difference between ls and ls -l?

**Answer:**

```bash
ls
```

Displays file and folder names only.

```bash
ls -l
```

Displays detailed information.

---

## Q3. What does ls -a do?

**Answer:**

Displays all files including hidden files.

---

## Q4. What is a hidden file?

**Answer:**

A file beginning with:

```bash
.
```

Example:

```bash
.git
.bashrc
```

---

## Q5. What does .. represent?

**Answer:**

Parent Directory.

Example:

```bash
cd ..
```

Moves one level up.

---

# Day 4 Summary

## Commands Learned

```bash
pwd
ls
ls -l
ls -a
ls -la
```

## Concepts Learned

- Current Working Directory
- Listing Files
- Detailed File Information
- Hidden Files
- Current Directory (`.`)
- Parent Directory (`..`)
- Linux File Visibility

---

