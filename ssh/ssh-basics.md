# 🔐 SSH Basics – Week 3

## ✅ What I Learned
- SSH (Secure Shell) allows you to connect to remote servers securely from the terminal.
- There are two common authentication methods:
  - Password-based
  - Key-based (more secure)

## 🛠️ Commands I Practiced

```bash
ssh username@ip_address       # Connect to a remote server
ssh-keygen                    # Generate SSH key pair
ssh-copy-id username@ip       # Copy public key to remote server (optional)
```

## 📁 SSH Key Files

- `~/.ssh/id_rsa` → Private key (keep this safe and never share it)
- `~/.ssh/id_rsa.pub` → Public key (can be shared with servers)

## 🧠 Notes
- After generating keys, I copied my public key to the server's `~/.ssh/authorized_keys` file.
- Using `ssh-copy-id` makes this automatic and easier.
- Always check file permissions. The `.ssh` folder should have `700` permissions, and the `authorized_keys` file should be `600`.

---

## 📚 Resources Used

- AltSchool LMS (SSH Module)
- DigitalOcean: [How to Use SSH](https://www.digitalocean.com/community/tutorials/ssh-essentials-working-with-ssh-servers-clients-and-keys)
- ChatGPT walkthroughs

