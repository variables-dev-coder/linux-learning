# Linux Day 5

## Commands Learned

- cd
- mkdir
- rmdir

---

# cd (Change Directory)

Used to move between directories.

## Syntax

```bash
cd directory_name
```

## Examples

```bash
cd Documents
```

Go Home:

```bash
cd
```

or

```bash
cd ~
```

Move One Directory Up:

```bash
cd ..
```

Move Two Directories Up:

```bash
cd ../..
```

Go Root:

```bash
cd /
```

Previous Directory:

```bash
cd -
```

---

# mkdir (Make Directory)

Creates directories.

## Syntax

```bash
mkdir directory_name
```

## Examples

```bash
mkdir company
```

Create Multiple:

```bash
mkdir java linux dsa
```

Create Nested:

```bash
mkdir -p company/project/backend
```

---

# rmdir (Remove Directory)

Deletes empty directories.

## Syntax

```bash
rmdir directory_name
```

## Example

```bash
rmdir test
```

## Limitation

Works only on empty directories.

```bash
rmdir demo
```

Error:

```text
Directory not empty
```

---

# Summary

| Command | Purpose |
|----------|----------|
| cd | Change directory |
| mkdir | Create directory |
| rmdir | Remove empty directory |
| cd .. | Move up one level |
| cd / | Go to root |
| mkdir -p | Create nested directories |
