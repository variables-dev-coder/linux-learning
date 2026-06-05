# Linux Day 6 - File Management

## Commands Covered

* touch
* cp
* mv
* rm

---

# touch

Creates empty files.

## Syntax

```bash
touch filename
```

## Example

```bash
touch file1.txt
```

Create multiple files:

```bash
touch a.txt b.txt c.txt
```

---

# cp

Copies files and directories.

## Syntax

```bash
cp source destination
```

## Examples

Copy file:

```bash
cp file1.txt backup.txt
```

Copy file into folder:

```bash
cp file1.txt company/
```

Copy folder:

```bash
cp -r company company_backup
```

---

# mv

Moves or renames files and folders.

## Syntax

```bash
mv source destination
```

## Examples

Move file:

```bash
mv file1.txt company/
```

Rename file:

```bash
mv file1.txt employee.txt
```

Rename folder:

```bash
mv company organization
```

---

# rm

Deletes files and directories.

## Examples

Delete file:

```bash
rm file1.txt
```

Delete multiple files:

```bash
rm a.txt b.txt c.txt
```

Delete directory:

```bash
rm -r company
```

Force delete:

```bash
rm -rf company
```

---

# Important Notes

* touch → Create files
* cp → Copy files/folders
* mv → Move or rename
* rm → Delete files/folders

⚠️ Be careful with:

```bash
rm -rf
```

Deleted data usually cannot be recovered.
