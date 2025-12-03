
# 🐧 **The Ultimate Linux Command Cheat Sheet**

A clean, structured, and developer-friendly cheat sheet of essential Linux commands.
Perfect for beginners, sysadmins, and power users who want a fast & reliable reference.

---

## 🛡️ Badges

<p align="left">
  <img src="https://img.shields.io/badge/Stars-Welcome-yellow?style=flat" />
  <img src="https://img.shields.io/badge/PRs-Accepted-brightgreen?style=flat" />
  <img src="https://img.shields.io/badge/Contributions-Open-blue?style=flat" />
  <img src="https://img.shields.io/badge/Code%20Quality-Excellent-success?style=flat" />
  <img src="https://img.shields.io/badge/License-MIT-purple?style=flat" />
</p>

---

# 📑 **Table of Contents**

* [📂 File & Directory Commands](#-file--directory-commands)
* [🧰 System Information](#-system-information)
* [⚙️ Package Management](#️-package-management)
* [🔐 Permissions & Ownership](#-permissions--ownership)
* [🌐 Networking](#-networking)
* [📝 File Viewing & Editing](#-file-viewing--editing)
* [🔍 Process Management](#-process-management)
* [💬 Contribution](#-contribution)

---

# 📂 File & Directory Commands

<details>
<summary><strong>Click to Expand</strong></summary>

| Command                    | Description                     | Example                    | Use Case                             |
| -------------------------- | ------------------------------- | -------------------------- | ------------------------------------ |
| `ls`                       | Lists files & directories       | `ls -la`                   | View all files including hidden ones |
| `cd <path>`                | Change directory                | `cd /var/www`              | Navigate into directories            |
| `pwd`                      | Print current working directory | `pwd`                      | Know where you are in the system     |
| `mkdir <name>`             | Create a directory              | `mkdir backups`            | Create folders                       |
| `rm <file>`                | Remove a file                   | `rm old.txt`               | Delete unnecessary files             |
| `rm -r <dir>`              | Remove directory recursively    | `rm -r logs/`              | Delete folders with content          |
| `cp <src> <dest>`          | Copy files or directories       | `cp file.txt /backup/`     | Backing up files                     |
| `mv <src> <dest>`          | Move or rename                  | `mv app.log logs/`         | Renaming or relocating files         |
| `touch <file>`             | Create empty file               | `touch notes.txt`          | Quickly create a new file            |
| `find <dir> -name pattern` | Search for files                | `find /etc -name "*.conf"` | Locate configuration files           |

</details>

---

# 🧰 System Information

<details>
<summary><strong>Click to Expand</strong></summary>

| Command       | Description                 | Example       | Use Case                     |
| ------------- | --------------------------- | ------------- | ---------------------------- |
| `uname -a`    | Displays system info        | `uname -a`    | Check OS & kernel details    |
| `df -h`       | Disk usage (human readable) | `df -h`       | Monitor storage space        |
| `free -m`     | Memory usage                | `free -m`     | RAM monitoring               |
| `top`         | Interactive system monitor  | `top`         | See live processes & CPU use |
| `htop`        | Better system monitor       | `htop`        | Easier system monitoring     |
| `uptime`      | Shows uptime & load         | `uptime`      | Check system stability       |
| `hostnamectl` | System hostname details     | `hostnamectl` | Identify server              |

</details>

---

# ⚙️ Package Management

<details>
<summary><strong>Click to Expand</strong></summary>

### **APT (Debian/Ubuntu)**

| Command             | Description                | Example                  | Use Case                   |
| ------------------- | -------------------------- | ------------------------ | -------------------------- |
| `apt update`        | Refresh package lists      | `sudo apt update`        | Before installing packages |
| `apt upgrade`       | Upgrade installed packages | `sudo apt upgrade`       | Keep system updated        |
| `apt install <pkg>` | Install a package          | `sudo apt install nginx` | Install software           |
| `apt remove <pkg>`  | Remove a package           | `sudo apt remove nginx`  | Uninstall software         |

### **YUM/DNF (CentOS/Fedora)**

| Command             | Description    | Example                  | Use Case         |
| ------------------- | -------------- | ------------------------ | ---------------- |
| `dnf install <pkg>` | Install apps   | `sudo dnf install httpd` | Install packages |
| `dnf remove <pkg>`  | Remove package | `sudo dnf remove httpd`  | Cleanup          |
| `dnf update`        | System updates | `sudo dnf update`        | Patch system     |

</details>

---

# 🔐 Permissions & Ownership

<details>
<summary><strong>Click to Expand</strong></summary>

| Command                   | Description             | Example                      | Use Case                   |
| ------------------------- | ----------------------- | ---------------------------- | -------------------------- |
| `chmod 755 <file>`        | Change file permissions | `chmod 644 index.html`       | Set read/write rules       |
| `chown user:group <file>` | Change file owner       | `chown root:root /etc/hosts` | Correct ownership          |
| `umask`                   | Default permission mask | `umask 022`                  | Control default file perms |

</details>

---

# 🌐 Networking

<details>
<summary><strong>Click to Expand</strong></summary>

| Command         | Description        | Example                 | Use Case                       |
| --------------- | ------------------ | ----------------------- | ------------------------------ |
| `ip a`          | Shows IP addresses | `ip a`                  | Network troubleshooting        |
| `ping <host>`   | Check connectivity | `ping google.com`       | Verify internet                |
| `curl <url>`    | Make HTTP requests | `curl https://api.com`  | API testing                    |
| `wget <url>`    | Download files     | `wget file.com/app.deb` | Download packages              |
| `ss -tulpn`     | Show open ports    | `ss -tulpn`             | Check which service is running |
| `ssh user@host` | Remote login       | `ssh admin@server`      | Access servers                 |

</details>

---

# 📝 File Viewing & Editing

<details>
<summary><strong>Click to Expand</strong></summary>

| Command          | Description          | Example              | Use Case             |
| ---------------- | -------------------- | -------------------- | -------------------- |
| `cat <file>`     | Show file content    | `cat notes.txt`      | View text quickly    |
| `less <file>`    | Page viewer          | `less logfile.log`   | Read large files     |
| `head <file>`    | First 10 lines       | `head -n 20 app.log` | Preview file         |
| `tail <file>`    | Last 10 lines        | `tail app.log`       | Watch logs           |
| `tail -f <file>` | Real-time log watch  | `tail -f system.log` | Monitor live updates |
| `nano <file>`    | Simple text editor   | `nano config.json`   | Quick edits          |
| `vim <file>`     | Advanced text editor | `vim index.html`     | Power editing        |

</details>

---

# 🔍 Process Management

<details>
<summary><strong>Click to Expand</strong></summary>

| Command                      | Description            | Example                 | Use Case                     |                          |
| ---------------------------- | ---------------------- | ----------------------- | ---------------------------- | ------------------------ |
| `ps aux`                     | List running processes | `ps aux                 | grep nginx`                  | Inspect running services |
| `kill <pid>`                 | Kill a process         | `kill 2013`             | Stop frozen apps             |                          |
| `kill -9 <pid>`              | Force kill             | `kill -9 2013`          | Terminate stubborn processes |                          |
| `systemctl start <service>`  | Start service          | `systemctl start sshd`  | Manage services              |                          |
| `systemctl stop <service>`   | Stop service           | `systemctl stop sshd`   | Shutdown services            |                          |
| `systemctl status <service>` | Service status         | `systemctl status sshd` | Debug service issues         |                          |

</details>

---

# 💬 **Contribution**

Contributions are **welcome & appreciated**!
You can help by:

* Adding more Linux commands
* Improving descriptions
* Adding examples for real-world use
* Reporting issues
* Making documentation even cleaner

---

# **Image :**

<img src="https://github.com/alok-kumar8765/linux_cheatsheet/blob/main/img.jpg" height="50%" width="50%">