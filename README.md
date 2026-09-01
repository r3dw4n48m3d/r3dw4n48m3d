<div align="center">

# CVE-2021-3493-Exploit

**A proof-of-concept local privilege escalation exploit for CVE-2021-3493, written in C.**

</div>


<div align="center">
  <img align="right" width="200" src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExOHp1eXR6bW5oNjB4eG9oZzR5eGZ6eGZ6eGZ6eGZ6eGZ6eGZ6JmVwPXYxX2ludGVybmFsX2dpZl9ieV9pZCZjdD1n/YQitE4YNQNahy/giphy.gif">
</div>

## 📌 Description
This repository contains a C implementation of the exploit for **CVE-2021-3493**. 

This is a **Local Privilege Escalation (LPE)** vulnerability in the `OverlayFS` implementation in the Linux kernel. It allows a local user to gain root access due to incorrect validation of extended attributes (xattrs) when files are set in an overlay mount.


### 🎯 Affected Versions
- Ubuntu 20.10
- Ubuntu 20.04 LTS
- Ubuntu 18.04 LTS
- Ubuntu 16.04 LTS
- Ubuntu 14.04 ESM
- (Kernel versions prior to 5.11)

---

## ⚠️ Disclaimer
> [!WARNING]
> This tool is for **educational purposes only** and for use in authorized security testing. The author, **Redwan Ahmed**, is not responsible for any misuse or damage caused by this program. **Don't be a script kiddie; understand the code before you run it!** 👽

---

## 🚀 Usage

### 1. Prerequisites
Ensure you have `gcc` installed on the target machine.

### 2. Compilation
```bash
gcc exploit.c -o exploit
