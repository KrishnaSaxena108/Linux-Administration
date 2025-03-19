# 🧪 Experiment : 3 - 4

## 📌 Objective

Learn how to:

- **Use brace expansion** to generate discretionary strings and sequences.
- **View the gedit man page.**
- **Search for ext4 file system commands** using `man -k`.

---

## 📝 Description

In Linux administration, understanding and efficiently using system commands enhances productivity and system management.  
This experiment covers:

- How to apply **brace expansion** for generating multiple strings.
- Exploring the **manual page for gedit** editor.
- Using the `man -k` command to locate commands related to **ext4 file systems**.

---

## 🚀 Tasks

### 1️⃣ Viewing the gedit Manual Page

`gedit` is a commonly used graphical text editor in Linux.

### 🔧 Command:

```bash
# Open the Manual Page of gedit
man gedit
```

#### 🖼️ Screenshots

![Screenshot 2025-03-19 172911](https://github.com/user-attachments/assets/a923aaff-9717-4532-8fd7-3fafa55df9aa)

---

### 2️⃣ Search ext4 File System Commands

To tune or manage `ext4` file system parameters, we can search for relevant commands using:

### 🔧 Command:

```bash
# List the list of Manual Pages related to ext4 keyword
man -k ext4

# Open the Manual Page for tune ext4 file-system parameters
man tune2fs
```

#### 🖼️ Screenshots

![Screenshot 2025-03-19 174250](https://github.com/user-attachments/assets/e878e66a-590d-4204-84d7-357460d149db)

![Screenshot 2025-03-19 173456](https://github.com/user-attachments/assets/ad91c988-0e94-46fa-b483-ef7cce95296b)

---

### 🌀 Brace Expansion Overview

Brace expansion is used to `generate strings or sequences` automatically.
Braces can contain:

A  `comma-separated list of strings`
A `sequence expression` with defined start, stop, and step values

### 🔧 Syntax:

```bash
# Comma-separated list expansion
echo prefix{one,two,three}suffix

# Sequence expression
echo {start..stop..step}
```

### 📄 Example:

```bash
# Using sequence expression with step
echo {1..20..2}
```

#### 🖼️ Screenshots

![Screenshot 2025-03-19 175508](https://github.com/user-attachments/assets/bc5a75e2-0bc2-4521-8a41-fe81f9907b50)

---

## 🎯 Summary
- Viewed gedit command manual.
- Used man -k to search ext4 tuning commands.
- Learned brace expansion syntax and usage.
