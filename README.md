# 🐧 Linux Basics to Advanced Command Guide

A comprehensive guide to Linux, starting from the basics, suitable for developers, support engineers, DevOps professionals, and system admins.

---

## 🧠 What is Linux?

**Linux** is an open-source, Unix-like operating system that powers everything from:
- Cloud servers (AWS, GCP, Azure)
- Android phones
- IoT devices
- Developer systems

It is known for:
- 🔐 Security
- 💻 Performance
- ⚙️ Flexibility
- 📜 Scripting and automation support

macOS is Unix-based, so most Linux commands also work in the macOS terminal.

---

## 📁 Linux File System Hierarchy (Common Folders)

| Folder         | Description                              |
|----------------|------------------------------------------|
| `/`            | Root directory                           |
| `/home`        | User home directories                    |
| `/etc`         | System configuration files               |
| `/var/log`     | Log files                                |
| `/usr/bin`     | Executable binaries                      |
| `/dev`         | Device files                             |
| `/tmp`         | Temporary files                          |
| `/proc`        | System process info                      |

---

## ✅ Stage 1: Basic Navigation Commands

| Command             | Description                                  |
|---------------------|----------------------------------------------|
| `pwd`               | Print working directory                      |
| `ls`                | List files in current directory              |
| `ls -l`             | Long listing with file size and permissions  |
| `ls -a`             | Show hidden files                            |
| `cd folder/`        | Change to a directory                        |
| `cd ..`             | Go back one level                            |
| `cd ~`              | Go to home directory                         |
| `clear`             | Clear the terminal                           |

---

## 📂 Stage 2: File and Directory Management

| Command                     | Description                        |
|-----------------------------|------------------------------------|
| `touch file.txt`            | Create an empty file               |
| `mkdir folder`              | Create a new folder                |
| `rm file.txt`               | Delete a file                      |
| `rm -r folder/`             | Delete folder recursively          |
| `cp file1.txt file2.txt`    | Copy file                          |
| `mv old.txt new.txt`        | Move or rename file                |
| `cat file.txt`              | Show content of file               |
| `nano file.txt`             | Open file in nano editor           |

---

## 🔍 Stage 3: System Info & Monitoring

| Command            | Description                                |
|--------------------|--------------------------------------------|
| `uname -a`         | Show kernel and OS info                    |
| `top`              | Show running processes                     |
| `free -h`          | Show memory usage                          |
| `df -h`            | Show disk space                            |
| `du -sh folder/`   | Show folder size                           |
| `uptime`           | Show system uptime                         |
| `whoami`           | Display current user                       |

---

## 🔒 Stage 4: User & Permission Management

| Command                                | Description                       |
|----------------------------------------|-----------------------------------|
| `adduser username`                     | Create a new user                 |
| `passwd username`                      | Set user password                 |
| `su - username`                        | Switch user                       |
| `chmod 755 script.sh`                  | Change file permissions           |
| `chown user:group file.txt`            | Change file ownership             |
| `id`                                   | Show user ID and groups           |
| `groups`                               | Show groups user belongs to       |

> **Permission Reference**:
> - `r` = read, `w` = write, `x` = execute  
> - `chmod 755` = rwxr-xr-x

---

## 🌐 Stage 5: Networking Commands

| Command                      | Description                           |
|------------------------------|---------------------------------------|
| `ping google.com`            | Test network connectivity             |
| `ip a` or `ifconfig`         | Show IP address                       |
| `netstat -tuln`              | Show listening ports                  |
| `curl ifconfig.me`           | Show public IP                        |
| `wget https://url`           | Download a file                       |
| `scp file user@ip:/path`     | Secure copy over SSH                  |

---

## ⚙️ Stage 6: Process & Service Management

| Command                         | Description                         |
|----------------------------------|-------------------------------------|
| `ps aux`                         | Show all running processes          |
| `kill <PID>`                     | Kill process by ID                  |
| `killall processname`           | Kill process by name                |
| `systemctl status nginx`         | Show service status (systemd)       |
| `systemctl restart apache2`      | Restart a service                   |
| `journalctl -xe`                 | Show recent system logs             |

---

## 📦 Stage 7: Package Management (Ubuntu/Debian)

| Command                    | Description                       |
|----------------------------|-----------------------------------|
| `sudo apt update`         | Update package index              |
| `sudo apt upgrade`        | Upgrade installed packages        |
| `sudo apt install htop`   | Install a package                 |
| `sudo apt remove nginx`   | Remove a package                  |
| `dpkg -l`                 | List all installed packages       |

---

## 🛠️ Stage 8: Logs & Troubleshooting

| Command                        | Description                       |
|--------------------------------|-----------------------------------|
| `cd /var/log`                  | Go to log directory               |
| `ls`                           | List log files                    |
| `tail -f syslog`               | Monitor logs live                 |
| `tail -n 100 app.log`          | Last 100 lines of log file        |
| `grep "ERROR" app.log`         | Search for "ERROR" in log         |

---

## 🚀 Stage 9: Advanced Linux Commands

| Command                                     | Description                           |
|---------------------------------------------|---------------------------------------|
| `find / -name "file.txt"`                   | Find a file in entire system          |
| `grep "text" file.txt`                      | Search for text in file               |
| `tar -czvf archive.tar.gz folder/`          | Compress a folder                     |
| `tar -xzvf archive.tar.gz`                  | Extract archive                       |
| `crontab -e`                                 | Edit scheduled cron jobs              |
| `ssh user@remote-ip`                         | SSH into remote server                |
| `rsync -avz source/ dest/`                   | Sync files and folders                |

---

## 🧪 Try This Sample Exercise

```bash
cd ~
mkdir linux-practice
cd linux-practice
touch hello.txt
echo "Welcome Deepak!" > hello.txt
cat hello.txt
chmod 755 hello.txt


> **Author:** Deepak Dadi  
> **Updated:** August 2025  
> **Usage:** Free for personal and educational use

