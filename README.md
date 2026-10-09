# Linux Privilege Escalation Lab

## About the Project

This project is based on my practical learning of Linux privilege escalation. I used Kali Linux and Ubuntu Server to understand how Linux permissions and system misconfigurations can create security risks.

My goal was to learn how to enumerate a Linux system, investigate possible privilege escalation paths, and understand how to fix insecure configurations.

## Tools and Technologies

- Kali Linux
- Ubuntu Server
- SSH
- Linux command-line tools
- LinPEAS
- GitHub

## Topics Covered

### 1. Sudo Misconfiguration
Learned how sudo permissions work and how an unsafe rule can allow a restricted user to execute commands with elevated privileges.

### 2. SUID and SGID Permissions
Studied special Linux permission bits and how incorrectly configured executables can introduce security risks.

### 3. SSH Key Security
Explored how SSH keys work, why private keys must be protected, and how file permissions help secure remote authentication.

### 4. Linux Capabilities
Learned how Linux capabilities provide specific privileges to programs and why unnecessary capabilities should be reviewed.

## Repository Structure

- `findings/` — security findings and technical notes
- `methodology/` — assessment steps and methodology
- `remediation/` — recommendations for fixing misconfigurations
- `screenshots/` — terminal screenshots and lab evidence

## Key Learning

Through this project, I improved my understanding of Linux users and permissions, sudo rules, special permission bits, SSH security, and Linux capabilities.

I also learned the importance of documenting security findings and recommending appropriate fixes.

## Disclaimer

This project is intended for educational purposes. Security testing should only be performed on systems that I own or have explicit permission to assess.
