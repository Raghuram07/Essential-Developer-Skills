# 🚀 Important Linux Commands

## 📂 1. Listing Files and Directories

### `ls` - List directory contents
The `ls` command is used to list files and directories in the current location.

#### Common options:
- **`ls -a`** → 📌 Displays **all** files, including hidden ones (files starting with `.`).
- **`ls -l`** → 📋 Shows a detailed list, including permissions, owner, group, file size, and modification date.
- **`ls -la`** → 🔍 Combines both `-l` and `-a`, showing detailed information for **all** files (including hidden files).

**Example:**
```sh
ls -la
```
_Output:_
```
drwxr-xr-x  5 user  staff    160 Feb  5 10:35 Documents
-rw-r--r--  1 user  staff   1024 Feb  5 10:30 file.txt
```

---

## 📁 2. Working with Directories

### `mkdir` - Create a new directory
```sh
mkdir directory_name
```
Creates a new directory with the given name.

### `rmdir` - Remove an empty directory
```sh
rmdir directory_name
```
Removes an **empty** directory.

For non-empty directories, use:
```sh
rm -r directory_name
```

---

## 📄 3. Working with Files

### `touch` - Create an empty file or update timestamp
```sh
touch filename.txt
```
Creates a new, empty file or updates the timestamp of an existing file.

### `echo` - Display a message or write to a file
```sh
echo "Hello, World!"
```
📢 Prints text to the terminal.
```sh
echo "Hello, World!" > file.txt
```
✍️ Writes the text into `file.txt` (overwriting existing content).

### `cat` - View or concatenate file contents
```sh
cat file.txt
```
📜 Displays the contents of `file.txt`.
```sh
cat file1.txt file2.txt > merged.txt
```
🔗 Merges `file1.txt` and `file2.txt` into `merged.txt`.

---

## 🔎 4. Searching in Files

### `grep` - Search for patterns in files

#### Basic usage:
```sh
grep "error" logfile.txt
```
Finds all lines containing "error" in `logfile.txt`.

#### Case-insensitive search (`-i`)
```sh
grep -i "error" logfile.txt
```
🔤 Finds "error", "Error", "ERROR", etc.

#### Recursive search in all files (`-r`)
```sh
grep -r "error" /var/logs
```
🔍 Searches for "error" in **all** files inside `/var/logs`.

#### Show line numbers (`-n`)
```sh
grep -n "error" logfile.txt
```
📌 Displays matching lines **with line numbers**.

#### Exclude lines (`-v`)
```sh
grep -v "error" logfile.txt
```
🚫 Shows lines **not containing** "error".

---

## 🔐 5. File and Directory Permissions

### `chmod` - Change file permissions
```sh
chmod 755 script.sh
```
Gives the owner full permissions and others read/execute permissions.

### `chown` - Change file owner
```sh
chown user:group filename
```
👤 Changes the owner and group of `filename`.

---

## ⚙️ 6. Process Management

### `ps` - View active processes
```sh
ps aux
```
Shows all running processes.

### `kill` - Terminate a process
```sh
kill PID
```
❌ Kills a process with the given **PID**.

### `htop` - Interactive process viewer
```sh
htop
```
📊 Displays an interactive view of system processes.

---

## 🌐 7. Networking

### `ping` - Check network connectivity
```sh
ping google.com
```
📡 Sends ICMP packets to test if a server is reachable.

### `curl` - Fetch data from a URL
```sh
curl https://example.com
```
📥 Fetches the contents of the URL.

### `wget` - Download a file
```sh
wget https://example.com/file.zip
```
⬇️ Downloads a file from a given URL.

---

## 💾 8. Disk Usage and Management

### `df` - Show disk usage
```sh
df -h
```
📊 Displays available and used disk space in a human-readable format.

### `du` - Show directory size
```sh
du -sh foldername
```
📦 Shows the size of a folder.

---

## 📦 9. Archiving and Compression

### `tar` - Archive files
```sh
tar -cvf archive.tar directory/
```
📂 Creates an archive of `directory/`.

### `tar` - Extract files
```sh
tar -xvf archive.tar
```
📜 Extracts files from `archive.tar`.

### `gzip` - Compress a file
```sh
gzip file.txt
```
🗜️ Compresses `file.txt` to `file.txt.gz`.

### `gunzip` - Decompress a file
```sh
gunzip file.txt.gz
```
📂 Decompresses `file.txt.gz` back to `file.txt`.

---

## 🛠️ 10. Git Version Control

### `git clone` - Clone a repository
```sh
git clone https://github.com/user/repo.git
```
📥 Clones a remote repository.

### `git status` - Check repository status
```sh
git status
```
🔍 Shows the status of the working directory.

### `git commit` - Commit changes
```sh
git commit -m "Commit message"
```
💾 Commits staged changes with a message.

### `git push` - Push changes to remote
```sh
git push origin main
```
🚀 Pushes committed changes to the remote repository.

---

This document provides a structured and easy-to-follow guide on essential Linux commands for developers. Let me know if you need additional sections! 😊

