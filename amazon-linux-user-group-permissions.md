# 🐧 Amazon Linux Practice - User, Group & File Permission Commands

This documentation contains command-line operations performed on an **Amazon Linux 2023 EC2 instance**, focusing on:

- User & group management
- File/directory permission settings
- Ownership management
- Basic file system operations

---

## 👤 User Management

```bash
# Add a new user
useradd anaas
```

---

## 👥 Group Management

```bash
# Add a new group
groupadd linux
```

---

## 🔐 File Ownership & Permissions

```bash
# Create a file and directory
touch file1
mkdir dir1

# Change directory permission to allow all (rwx for everyone)
chmod 777 dir1

# Set file to executable and readable (rwxr-xr-x)
chmod 755 file1

# Change owner of directory to a user
chown anaas dir1

# Change group of a file (must exist)
chgrp linux file1
```

> ⚠️ Note: If a group doesn’t exist (e.g., `linus`), `chgrp` will throw an error.

---

## 📚 Useful Commands

```bash
# List directory contents with ownership & permission details
ls -l

# Switch to root user
sudo su
```

---

## ✅ Sample Output

```bash
drwxrwxrwx. 2 anaas root   6 Jul 20 06:18 dir1
-rwxr-xr-x. 1 root  linux  0 Jul 20 06:18 file1
```

---

## 🧑‍💻 Environment

- **Instance Type:** EC2  
- **OS:** Amazon Linux 2023  
- **Shell:** bash  
- **Access:** SSH with PEM key  
