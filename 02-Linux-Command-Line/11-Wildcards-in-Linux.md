# 11. Wildcards in Linux

## 1. Introduction

Wildcards are special characters used to match filenames and patterns.

They help administrators work with multiple files without typing every filename.

## 2. Common Wildcards

| Wildcard | Meaning | Example |
|---|---|---|
| `*` | Matches zero or more characters | `ls *.txt` |
| `?` | Matches exactly one character | `ls file?.txt` |
| `[]` | Matches one character from a given set or range | `ls file[123].txt` |

## 3. Practical Examples

### Example 1: List all text files

```bash
ls *.txt
```

### Example 2: List files starting with `log`

```bash
ls log*
```

### Example 3: List files ending with `.conf`

```bash
ls *.conf
```

### Example 4: Match a single character

```bash
ls file?.txt
```

This can match `file1.txt` or `fileA.txt`, but not `file10.txt`.

### Example 5: Match specific characters

```bash
ls file[123].txt
```

This can match `file1.txt`, `file2.txt`, or `file3.txt`.

### Example 6: Copy all PDF files

```bash
cp *.pdf /backup/
```

## 4. Wildcards vs Regular Expressions

| Wildcards | Regular Expressions |
|---|---|
| Commonly used for filename matching | Used for searching and matching text patterns |
| Example: `ls *.txt` | Example: `grep -E '^[0-9]+' file.txt` |
| Used by the shell | Used by tools such as `grep` and `sed` |

**Important:** Shell wildcards and regular expressions are different. Their symbols may look similar, but their behaviour depends on the tool.

## 5. Interview Questions

**Q1. What are wildcards in Linux?**

Special characters used to match multiple filenames or patterns.

**Q2. What does `*` mean?**

It matches zero or more characters.

**Q3. What does `?` mean?**

It matches exactly one character.

**Q4. How do you list all `.log` files?**

```bash
ls *.log
```

**Q5. What is the difference between wildcards and regular expressions?**

Wildcards are commonly used for filename matching, while regular expressions are used for more advanced text-pattern matching.

**Status:** Documentation completed.
