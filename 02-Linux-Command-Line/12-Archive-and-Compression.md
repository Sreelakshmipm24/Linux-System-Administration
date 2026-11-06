# 12. Archive and Compression in Linux

## 1. Introduction

Linux provides commands to combine multiple files into one archive and reduce file sizes through compression.

These operations are useful for backups, file transfers and storage management.

## 2. Common Commands

| Command | Purpose |
|---|---|
| `tar` | Creates and extracts archives |
| `gzip` | Compresses files |
| `gunzip` | Decompresses `.gz` files |
| `zip` | Creates ZIP archives |
| `unzip` | Extracts ZIP archives |

## 3. TAR Command

### Create an archive

```bash
tar -cvf backup.tar /home
```

### List archive contents

```bash
tar -tvf backup.tar
```

### Extract an archive

```bash
tar -xvf backup.tar
```

## 4. TAR with GZIP Compression

### Create a compressed archive

```bash
tar -czvf backup.tar.gz /home
```

### Extract a compressed archive

```bash
tar -xzvf backup.tar.gz
```

### List compressed archive contents

```bash
tar -tzvf backup.tar.gz
```

## 5. GZIP Command

### Compress a file

```bash
gzip file.txt
```

Creates `file.txt.gz` and normally removes the original file.

### Decompress a file

```bash
gunzip file.txt.gz
```

## 6. ZIP and UNZIP Commands

### Create a ZIP archive

```bash
zip backup.zip file1.txt file2.txt
```

### Extract a ZIP archive

```bash
unzip backup.zip
```

### List ZIP contents

```bash
unzip -l backup.zip
```

## 7. TAR Options

| Option | Meaning |
|---|---|
| `-c` | Create archive |
| `-x` | Extract archive |
| `-v` | Display operation details |
| `-f` | Specify archive filename |
| `-t` | List archive contents |
| `-z` | Use gzip compression |

## 8. TAR vs ZIP

| TAR | ZIP |
|---|---|
| Mainly combines files into an archive | Combines and compresses files |
| Compression requires an additional option or tool | Compression is built into the format |
| Common in Linux administration | Common across Windows and Linux |

## 9. Practical Example: Backup a Directory

Create a compressed backup:

```bash
tar -czvf website-backup.tar.gz /var/www/html
```

Verify its contents:

```bash
tar -tzvf website-backup.tar.gz
```

Extract it:

```bash
tar -xzvf website-backup.tar.gz
```

## 10. Interview Questions

**Q1. What is archiving?**

Combining multiple files into a single archive.

**Q2. What is compression?**

Reducing the size of files to save storage space.

**Q3. What is the difference between `.tar` and `.tar.gz`?**

`.tar` is an archive without compression. `.tar.gz` is an archive compressed using gzip.

**Q4. How do you create a compressed backup?**

```bash
tar -czvf backup.tar.gz /home
```

**Q5. How do you extract a `.tar.gz` file?**

```bash
tar -xzvf backup.tar.gz
```

**Q6. Which command extracts ZIP files?**

```bash
unzip backup.zip
```

**Status:** Documentation completed.
