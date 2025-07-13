# 🔐 Users and Permissions – Week 2

## ✅ What I Learned
- Every file and directory on Linux has an **owner**, a **group**, and **permission settings**.
- Permissions control who can:
  - Read (r)
  - Write (w)
  - Execute (x)
- Permissions apply to:
  - **User** (file owner)
  - **Group** (users in the same group)
  - **Others** (everyone else)

---

## 🛠️ Commands I Practiced

```bash
ls -l               # Show file permissions
chmod 755 file.txt  # Set file permissions to rwxr-xr-x
chmod u+x script.sh # Give the owner execute rights
chown user:group file.txt  # Change file ownership
```

---

## 🔢 Numeric Permission Reference

| Symbolic | Numeric | Meaning     |
|----------|---------|-------------|
| rwx      | 7       | Read, Write, Execute |
| rw-      | 6       | Read, Write |
| r--      | 4       | Read only   |
| ---      | 0       | No access   |

Example:
```bash
chmod 644 file.txt  # rw-r--r--
chmod 700 secrets.txt  # Only owner can read/write/execute
```

---

## 🧠 Notes

- `chmod` = change file permissions
- `chown` = change file owner or group
- Always check file permissions with `ls -l`
- Use `sudo` when modifying system-owned files

---

## 📚 Resources Used

- AltSchool LMS: Users & Permissions
- [chmod Calculator](https://chmod-calculator.com)
- YouTube: Linux File Permissions Crash Course
