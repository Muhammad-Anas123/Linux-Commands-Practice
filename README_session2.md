# 🐧 Linux File & Directory Management Practice

This session documents practical hands-on Linux command usage involving file and directory operations including hidden files, nested directories, navigation, copying, moving, and deletion. The commands were executed on an Ubuntu server instance.

---

## 📂 Topics Covered

| #  | Topic                     | Description |
|----|---------------------------|-------------|
| 1  | Directory Creation        | `mkdir`, `mkdir -p` |
| 2  | Hidden Files & Dirs       | `.file`, `.dir` |
| 3  | Navigation                | `cd`, `pwd`, `ls -a`, `ls -l` |
| 4  | Copying and Moving Files  | `cp`, `mv` |
| 5  | File Editing              | `vi`, `cat` |
| 6  | Deleting Files/Dirs       | `rm -rf` |
| 7  | Traversing Root           | `cd /`, `ls -al /` |

---

## 🧪 Commands and Explanations

### 📁 Create Directories
```bash
mkdir test1
mkdir -p dirC/dirD/dirE  # creates nested directories
```

---

### 📄 Create Hidden Files and Directories
```bash
touch .file4
mkdir .dirA
```

Hidden files and directories start with a dot (`.`) and are shown using `ls -a`.

---

### 📂 List Files (All and Detailed)
```bash
ls        # list visible files
ls -a     # list all files including hidden
ls -al    # long listing with permissions, ownership, and size
```

---

### 🔍 Navigate Directory Structure
```bash
cd dirC/dirD/dirE   # navigate deep into nested folders
cd ../..            # move up two directories
cd /                # go to root
cd ~ or cd /home/ubuntu  # go to user home
```

---

### 📄 File Content and Editing
```bash
cat file1
vi file1            # open file1 in terminal editor
```

---

### 📝 Copy and Move Files
```bash
cp file1 file2      # copy file1 to file2
cp file2 dir1       # copy to directory
mv file2 dir1       # move file2 into dir1
```

---

### 🗑️ Delete Files or Directories
```bash
rm -rf dir1         # remove directory and contents
```

---

### 🧠 History
```bash
history
```
Displays previously executed commands for reference.

---

## 🎯 Purpose

This session enhances understanding of:
- Navigating and manipulating the Linux file system
- Creating hidden files/directories
- Using recursive flags
- Editing with `vi` and checking content with `cat`

---

## 📜 License

MIT License – free to use and modify.
