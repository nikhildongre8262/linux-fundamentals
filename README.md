# Linux Fundamentals 🐧

My Linux learning notes covering essential commands, terminal usage, and practical examples as part of my cybersecurity journey.

## 📚 Topics

- Linux Navigation
- File & Directory Management
- Basic Networking
- Users & Permissions
- Process Management
- Package Management
- System Information
- Linux for Cybersecurity

## 1. Navigation

| Command | Description |
|---|---|
| `pwd` | Show current directory |
| `ls` | List files and directories |
| `ls -la` | Show hidden files and details |
| `cd folder` | Enter a directory |
| `cd ..` | Move to parent directory |
| `cd ~` | Go to home directory |
| `clear` | Clear terminal |

## 2. File & Directory Management

| Command | Description |
|---|---|
| `mkdir test` | Create a directory |
| `rmdir test` | Remove an empty directory |
| `touch file.txt` | Create an empty file |
| `cat file.txt` | Read file contents |
| `nano file.txt` | Edit a file |
| `cp file.txt backup.txt` | Copy a file |
| `mv file.txt new.txt` | Rename or move a file |
| `rm file.txt` | Delete a file |
| `rm -r folder` | Delete a directory and its contents |

## 3. Reading & Searching

| Command | Description |
|---|---|
| `head file.txt` | Show first 10 lines |
| `tail file.txt` | Show last 10 lines |
| `grep "word" file.txt` | Search for a word |
| `find . -name "*.txt"` | Find text files |
| `history` | Show command history |
| `man ls` | Open command manual |

## 4. User & System Information

| Command | Description |
|---|---|
| `whoami` | Show current username |
| `id` | Show user and group IDs |
| `hostname` | Show system hostname |
| `uname -a` | Show kernel information |
| `date` | Display date and time |

## 5. Networking

| Command | Description |
|---|---|
| `ip addr` | Show IP addresses |
| `ip route` | Show routing information |
| `ping -c 4 google.com` | Test connectivity |
| `ss -tuln` | Show listening ports |
| `curl ifconfig.me` | Check public IP |

## 6. Package Management

| Command | Description |
|---|---|
| `sudo apt update` | Refresh package information |
| `sudo apt upgrade` | Upgrade installed packages |
| `sudo apt install nmap` | Install Nmap |
| `sudo apt remove nmap` | Remove Nmap |

## 7. Process Management

| Command | Description |
|---|---|
| `ps aux` | List running processes |
| `top` | Monitor processes |
| `pgrep bash` | Find a process |
| `kill PID` | Terminate a process |
| `kill -9 PID` | Forcefully terminate a process |

## 8. Permissions & Storage

| Command | Description |
|---|---|
| `ls -l` | Show file permissions |
| `chmod 755 file.txt` | Change file permissions |
| `chmod +x script.sh` | Make a script executable |
| `chown user:user file.txt` | Change file ownership |
| `df -h` | Show disk usage |
| `du -sh folder` | Show folder size |
| `free -h` | Show memory usage |

## 9. Basic Practice

```bash
mkdir linux-practice
cd linux-practice
touch notes.txt
echo "My Linux Learning" > notes.txt
cat notes.txt
cp notes.txt backup.txt
ls -la
```

## 10. Learning Progress

- [] Linux Basic Commands✅                
- [] File & Directory Operations✅
- [] Basic Networking Commands✅
- [] File Permissions✅
- [] Users & Groups
- [] Bash Scripting
- [] Linux Administration
- [] Linux Security & Log Analysis

## Resources

- [Kali Linux Documentation] - (https://www.kali.org/docs/)
- [Ubuntu Documentation] - (https://help.ubuntu.com/)
- [Linux Command Library] - (https://linuxcommandlibrary.com/)

---------------------------------------------------------------------

Learning Linux | Building Cybersecurity Fundamentals

Learn • Practice • Document • Improve
