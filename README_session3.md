# 🐧 Linux Practice - User, Group, File & Archiving Commands

This documentation contains a collection of essential Linux commands practiced on an Ubuntu server, covering:

- User management  
- Group management  
- File editing and linking  
- Archiving and compression  
- Useful general-purpose commands

---

## 👤 User Management

```bash
# Add a new user (no password prompt, basic config)
useradd anas

# Add a user with interactive setup (recommended)
adduser noor

# Sample adduser interaction:
# New password:
# Retype new password:
# Full Name []: ayesha noor
# ... (other fields can be left blank)
```

---

## 👥 Group Management

```bash
# Create a new group
addgroup devopslearner

# Add a single user to a group
gpasswd -a anas devopslearner

# Add multiple users to the system
useradd ali
useradd asad

# Assign multiple users to a group (replaces existing members)
gpasswd -M ali,asad devopslearner

# View all groups
cat /etc/group
```

---

## 📝 File Editing & Linking

```bash
# Append text to a file
cat >> file1
# (Type your text, then press Ctrl+D to save)

# View file contents
cat file1

# Edit a file using vi
vi file1

# Create a symbolic (soft) link
ln -s file1 softlinkfile1

# Create a hard link
ln file2 hardlinkfile2

# List files with link info
ls -l
```

---

## 🗜️ Archiving & Compression

```bash
# Create a tar archive
tar -cvf dirx.tar dirx

# Compress the tar file
gzip dirx.tar

# Decompress a gzip file
gunzip dirx.tar.gz

# Extract contents from a tar archive
tar -xvf dirx.tar
```

---

## 📚 Useful Commands

```bash
# View all users on the system
cat /etc/passwd

# View all groups on the system
cat /etc/group

# Display current directory structure as a tree
tree

# Create multiple files
touch file1 file2 file3

# Create multiple directories
mkdir -p dir1 dir2 dir3

# Create nested directories
mkdir -p dirx/diry/dirz

# List contents with details
ls -l
```

---
