
# Introduction to Linux for DevOps Beginners

Linux is the backbone of modern DevOps, powering everything from servers to containers. This guide introduces you to essential Linux concepts and commands to get started on your DevOps journey.

---

## 📜 What is Linux?

Linux is an open-source, Unix-like operating system kernel used in various distributions (distros) such as Ubuntu, CentOS, Fedora, and Debian. It is known for stability, security, and flexibility, making it the preferred OS for servers and cloud infrastructure.

---

## 🕰️ History of Linux

- **1991**: Linus Torvalds created Linux as a free OS kernel.
- Inspired by UNIX, Linux became a community-driven project.
- Over time, various distributions evolved, supported by corporations and communities.

---

## 💻 Familiarizing Yourself with the Linux Terminal

- The terminal is the command-line interface (CLI) for interacting with the Linux OS. Commands entered into the terminal control the system directly.

- The terminal emulator is a program that present the terminal in a graphical way.

- Shell is a program that takes commands from the keyboard and gives them to the operating system to perform

```bash
root@277****23: / #
`root` - username \ computer username
`@` - seperator 
`277****23` - hostname of server
`/` - Current directory
`#` - dierctory

Example:

```bash
ls -la
```

This lists all files (including hidden ones) with detailed information.

---

## 📂 Understanding the Directory Tree Structure

Linux has a hierarchical file structure:

```
/
├── bin/       → Essential user binaries
├── boot/      → Bootloader files
├── dev/       → Device files
├── etc/       → System configuration
├── home/      → User directories
├── lib/       → Essential libraries
├── tmp/       → Temporary files
├── usr/       → User binaries and programs
└── var/       → Variable files (e.g., logs)
```

---

## 🧾 Linux Inode

Every file in Linux is represented by an inode which stores metadata like file size, ownership, permissions, and location of data blocks. Use `ls -i` to display inode numbers.

---

## 👥 Linux Users and Groups

- Every user has a UID (User ID).
- Users belong to groups for permission management.
- Use `adduser`, `passwd`, `groups`, and `chmod` to manage them.

---

## 🧪 Practical Labs

### Lab 1: Navigating Directories

```bash
cd /
ls
cd home
mkdir devops
touch hello.txt
```

### Lab 2: Working with Permissions

```bash
chmod 755 hello.txt
ls -l hello.txt
```

---

## 🔧 Common Linux Commands

| Command       | Description                              | Example Use Case                            |
|---------------|------------------------------------------|---------------------------------------------|
| `ls`          | Lists directory contents                 | `ls -l /home`                                |
| `cd`          | Changes directory                        | `cd /var/log`                                |
| `mkdir`       | Creates a new directory                  | `mkdir projects`                             |
| `rm`          | Deletes files or directories             | `rm -rf old_files/`                          |
| `cp`          | Copies files and directories             | `cp file.txt backup/`                        |
| `mv`          | Moves or renames files/directories       | `mv oldname.txt newname.txt`                |
| `chmod`       | Changes file permissions                 | `chmod 755 script.sh`                        |
| `chown`       | Changes file ownership                   | `chown user:group file.txt`                  |
| `nano` / `vim`| Text editors in CLI                      | `nano index.html`                            |
| `echo`        | Outputs strings or variables             | `echo $PATH`                                 |
| `cat`         | Displays file contents                   | `cat /etc/passwd`                            |
| `top`         | Displays system resource usage           | `top`                                        |
| `ps`          | Shows running processes                  | `ps aux`                                     |

---

## 🌐 External Learning Resources

- [Linux Journey](https://linuxjourney.com)
- [The Linux Command Line Book (Free PDF)](https://linuxcommand.org/tlcl.php)
- [OverTheWire Linux Wargames](https://overthewire.org/wargames/)
- [DevOps with Linux - YouTube](https://www.youtube.com/results?search_query=linux+for+devops)

---

## 📘 Recommended Tutorials

- [Introduction to Linux - edX](https://www.edx.org/course/introduction-to-linux)
- [Linux Essentials for DevOps - Udemy](https://www.udemy.com/course/linux-for-devops/)
- [Linux Foundation Training](https://training.linuxfoundation.org)

---

Happy Learning! 🚀
