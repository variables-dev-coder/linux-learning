# Linux Day 3 - Everything is a File & File System Hierarchy

## Everything is a File

Linux treats almost everything as a file.

Examples:

- Files
- Directories
- Hard disks
- USB devices
- Printers
- Processes
- Network connections

Benefits:

- Same commands work everywhere.
- Easy management.
- Consistent system design.

Examples:

```bash
cat notes.txt
cat /proc/cpuinfo
cat /proc/meminfo
```

---

## Linux File System Hierarchy

```text
/
├── home
├── etc
├── var
├── usr
├── tmp
├── root
```

---

## /

Root directory.

Top-most directory.

```bash
cd /
pwd
```

---

## /home

Stores personal files of users.

Examples:

```text
/home/munna
/home/john
```

---

## /etc

System configuration files.

Examples:

```text
/etc/passwd
/etc/hostname
/etc/hosts
```

Check hostname:

```bash
cat /etc/hostname
```

---

## /var

Variable data.

Examples:

```text
Logs
Cache
Mail
Databases
```

Important:

```text
/var/log
```

---

## /usr

Installed programs and libraries.

Examples:

```text
/usr/bin
/usr/lib
/usr/share
```

Find location of command:

```bash
which ls
```

---

## /tmp

Temporary files.

Example:

```bash
touch /tmp/test.txt
```

---

## /root

Home directory of root user.

```text
/root
```

Normal user:

```text
/home/username
```

Root user:

```text
/root
```

---

## Commands Practiced

```bash
pwd
ls
cd /
cd /home
cd /etc
cd /var
cd /usr
cd /tmp
cat /etc/hostname
which ls
```
