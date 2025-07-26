---
title: "Linux Path"
created: 2025-07-26
tags: [linux, path]
---


## 📌 1. **Absolute Path**

### ✅ Definition:

An **absolute path** is the **full path** from the root directory `/` to the target file or directory.

### 🛣️ Example:

```bash
cd /home/hcoco1/Documents
```

- Starts at `/` (root).
    
- Goes through `home → hcoco1 → Documents`.
    
- No matter where you are, this path will **always** lead to the same place.
    

### 💡 Rule:

> An absolute path **always starts with `/`**.

---

## 📌 2. **Relative Path**

### ✅ Definition:

A **relative path** is defined in relation to the **current working directory** (output of `pwd`).

### 🛣️ Example:

Let’s say you are in `/home/hcoco1`:

```bash
cd Documents
```

- Goes to the `Documents` directory **within the current folder**.
    
- This path only works **from specific locations**.
    

### 💡 Rule:

> A relative path **does not start with `/`**, and is based on where you currently are.

---

## 🔍 Special Relative References

|Symbol|Meaning|Example|
|---|---|---|
|`.`|Current directory|`./script.sh`|
|`..`|Parent directory|`cd ..`|
|`../dir`|Sibling of parent directory|`cd ../Downloads`|

---

### 🎯 Example Comparison

You're in `/home/hcoco1`:

|Type|Command|Meaning|
|---|---|---|
|Absolute|`cd /var/log`|Go to system logs|
|Relative|`cd Documents`|Go to `/home/hcoco1/Documents`|
|Relative|`cd ../user2`|Go to `/home/user2`|
[[Basic - Command Line Interface]]