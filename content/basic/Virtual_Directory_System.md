---
title: "Virtual Directory System"
created: 2025-07-26
tags: [linux]
---


[[Basic - Command Line Interface]]
## 📁 Linux Filesystem Hierarchy Standard (FHS)

|Directory|Purpose|
|---|---|
|`/`|**Root** directory – the top of the filesystem|
|`/bin`|Essential **user binaries** (e.g. `ls`, `cp`, `rm`)|
|`/boot`|Boot loader files (e.g. GRUB, kernel images)|
|`/dev`|Device files (e.g. `/dev/sda`, `/dev/tty`)|
|`/etc`|System-wide **configuration files**|
|`/home`|User home directories (e.g. `/home/user`)|
|`/lib`, `/lib64`|Essential shared libraries for binaries in `/bin` and `/sbin`|
|`/media`|Mount point for **removable media** (e.g. USB drives, CDs)|
|`/mnt`|Temporary mount point for filesystems|
|`/opt`|Optional or third-party software|
|`/proc`|Virtual filesystem for **process and system info**|
|`/root`|Home directory for the **root user**|
|`/run`|Runtime data for processes started since boot|
|`/sbin`|Essential **system binaries** (e.g. `fsck`, `reboot`)|
|`/srv`|Data for **services** (e.g. FTP, HTTP)|
|`/sys`|Virtual filesystem for **kernel and device info**|
|`/tmp`|Temporary files (cleared on reboot)|
|`/usr`|User programs, libraries, and documentation|
|`/var`|Variable data (e.g. logs, mail, spool files)|

---

### 🔧 Key Notes:

- **`/usr/bin`**: Non-essential user applications (e.g. `nano`, `python`).
    
- **`/usr/local/`**: Locally compiled software (kept separate from OS-managed).
    
- **`/var/log/`**: System logs.
    
- **`/etc/`**: Configuration (e.g. `fstab`, `hosts`, `passwd`).
    

---

### 🔍 Visual Overview (Simplified)

```
/
├── bin/
├── boot/
├── dev/
├── etc/
├── home/
│   └── username/
├── lib/
├── media/
├── mnt/
├── opt/
├── proc/
├── root/
├── run/
├── sbin/
├── srv/
├── sys/
├── tmp/
├── usr/
│   ├── bin/
│   └── local/
└── var/
```

---

