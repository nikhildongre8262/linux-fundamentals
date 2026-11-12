# 🐧 Linux Filters, Tools & User Management

## 1. Linux Filters

Powerful commands to quickly search, filter, and manipulate text output in Linux.

| Command | Description | Example |
|---|---|---|
| `tee` | Displays output and saves it to a file simultaneously. | `ls -la \| tee output.txt` |
| `grep` | Searches for matching text or patterns in files or output. | `grep "error" log.txt` |
| `cut` | Extracts specific columns or fields from text. | `cut -d ":" -f 1 /etc/passwd` |
| `wc` | Counts lines, words, and characters in files. | `wc -l file.txt` |
| `sort` | Sorts lines alphabetically or numerically. | `sort names.txt` |
| `uniq` | Removes or identifies adjacent duplicate lines. | `sort names.txt \| uniq` |
| `comm` | Compares two sorted files line by line. | `comm file1.txt file2.txt` |

### Useful Examples

```bash
# Search for a word in a file
grep "root" /etc/passwd

# Count lines in a file
wc -l access.log

# Extract usernames from /etc/passwd
cut -d ":" -f 1 /etc/passwd

# Sort and remove duplicate entries
sort names.txt | uniq

# Save command output while displaying it
ls -la | tee output.txt
```

---

## 2. Basic Linux Tools

Everyday utilities that help you navigate, inspect, and work efficiently on a Linux system.

| Command | Description | Example |
|---|---|---|
| `find` | Searches for files and directories based on criteria. | `find /home -name "*.txt"` |
| `locate` | Quickly searches files using a database of file paths. | `locate passwd` |
| `date` | Displays the current system date and time. | `date` |
| `cal` | Displays a calendar in the terminal. | `cal` |
| `tar` | Creates, extracts, and manages archive files. | `tar -cvf backup.tar files/` |
| `whoami` | Displays the username of the current user. | `whoami` |
| `who` | Shows users currently logged into the system. | `who` |
| `id` | Displays user ID, group ID, and group memberships. | `id` |

### Useful Examples

```bash
# Find a file by name
find /home -name "notes.txt"

# Search for a file using locate
locate notes.txt

# Display current date and time
date

# Display the current month's calendar
cal

# Create an archive
tar -cvf backup.tar Documents/

# Extract an archive
tar -xvf backup.tar

# Check the current username
whoami

# Check logged-in users
who

# Check user and group information
id
```

**Note:** `locate` may require updating its database before newly created files appear.

---

## 3. More Commands – User Switching

Useful user and privilege-related commands for everyday tasks.

| Command | Description | Example |
|---|---|---|
| `su username` | Switches to another user account. | `su nikhil` |
| `su root` | Switches to the root account. | `su root` |
| `su - username` | Switches to another user with their login environment. | `su - nikhil` |

### Important Tip

- Use `su - username` to switch users with their full login environment.
- Use `su username` when you need to switch users without loading their full login environment.
- Use `su -` to switch to root with the root login environment.
- Use `exit` to return to the previous shell.

**Remember:** `su` normally requires the target user's password. Root account access may be restricted depending on system configuration.

---

## 4. Linux User Management

Manage user accounts and access on a Linux system.

| Command | Description | Example |
|---|---|---|
| `useradd` | Creates a new user account. | `sudo useradd -m nikhil` |
| `userdel` | Deletes a user account. | `sudo userdel nikhil` |
| `usermod` | Modifies an existing user account. | `sudo usermod -aG sudo nikhil` |
| `chsh` | Changes a user's default login shell. | `chsh -s /bin/bash nikhil` |

### Useful Examples

```bash
# Create a user with a home directory
sudo useradd -m nikhil

# Set the user's password
sudo passwd nikhil

# Add a user to the sudo group
sudo usermod -aG sudo nikhil

# Change a user's default shell
sudo chsh -s /bin/bash nikhil

# Delete a user account
sudo userdel nikhil
```

**Note:** Group names and administrative permissions may differ across Linux distributions.

### Security Tip

Know these commands when investigating accounts, access, and privilege changes.

---

## 📚 Learning Resources

- [Linux Command Library](https://linuxcommandlibrary.com/)
- [Linux Journey](https://linuxjourney.com/)
- [GNU Coreutils Manual](https://www.gnu.org/software/coreutils/manual/)
- [The Linux Documentation Project](https://tldp.org/)

---

**Learning Linux one command at a time. 🐧**
