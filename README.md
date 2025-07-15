# 🐧 Linux Commands Practice

This repository documents my hands-on practice with essential Linux commands. It includes file creation, content manipulation, metadata inspection, and terminal editors. Screenshots of each session are attached for visual reference.


## 📂 Topics Covered

| #  | Topic                     | Description |
|----|---------------------------|-------------|
| 1  | File Creation             | `cat`, `touch` |
| 2  | File Viewing              | `cat`, `tac` |
| 3  | Content Redirection       | `>`, `>>` |
| 4  | File Merging              | `cat file1 file2 > file3` |
| 5  | Metadata Viewing          | `stat` |
| 6  | Editing with vi           | `vi file` |
| 7  | File Permissions & Info   | `ls -l` |

---

## 🧪 Commands and Explanations

### 🔐 Switching to Superuser
```bash
sudo su
```
Switches to the root user, giving elevated privileges.

---

### 📄 Creating and Writing to Files
```bash
cat > file1
```
Creates `file1` and allows writing interactively.

```bash
cat > file2
```
Same for `file2`.

---

### 📤 Viewing File Content
```bash
cat file1
cat file2
```

---

### 🔁 Redirecting and Appending Content
```bash
cat file1 > file2   # Overwrites file2 with content from file1
cat >> file1        # Appends new input to file1
```

---

### 🔗 Merging Files
```bash
cat file1 file2 > All
cat All
```
Combines contents of file1 and file2 into `All`.

---

### 🔁 Reversing File Output
```bash
tac file1
```
Displays file1 with lines in reverse order.

---

### 📁 Creating Multiple Files
```bash
touch file3 file4 file5
```
Creates multiple empty files.

---

### 🔍 Checking File Metadata
```bash
stat file1
```
Shows detailed file info:
- Size
- Access, Modify, Change times
- Owner and permissions

---

### 📝 Editing Files
```bash
vi file3
```
Opens `file3` in the `vi` editor. You can edit the file using `i` for insert mode and `:wq` to save and exit.

---

### 📋 Viewing All Files with Metadata
```bash
ls -l
```

Sample output:
```
-rw-r--r-- 1 root root  37 Jul 15 07:23 All
-rw-r--r-- 1 root root  57 Jul 15 07:31 file1
-rw-r--r-- 1 root root  26 Jul 15 07:26 file2
-rw-r--r-- 1 root root  49 Jul 15 07:30 file3
-rw-r--r-- 1 root root   0 Jul 15 07:30 file4
-rw-r--r-- 1 root root   0 Jul 15 07:30 file5
```

---

## 🎯 Purpose

This documentation and practice help reinforce foundational Linux skills which are essential for:
- System administration
- DevOps roles
- Shell scripting
- Working with servers

---

## 📌 Note

Screenshots are taken from an AWS EC2 Ubuntu instance with root privileges.

---

## 📜 License

MIT License – free to use and modify.
