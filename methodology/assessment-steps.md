# Linux Privilege Escalation - Assessment Methodology

## Introduction
In this lab, I practised checking a Linux system for misconfigurations that could allow a normal user to get higher privileges.

I used Kali Linux as my testing machine and Ubuntu Server as the target machine. I connected to the target using SSH.

## Steps I Followed

### 1. Connect to the target
I connected to the Ubuntu machine through SSH using a normal user account.

### 2. Check user permissions
I used commands such as `whoami`, `id`, and `sudo -l` to understand the current user's identity, group memberships, and allowed sudo commands.

### 3. Enumerate the system
I checked system information, SUID files, scheduled tasks, and file permissions to look for possible security issues.

### 4. Review the findings
I investigated suspicious configurations and checked whether they could actually lead to higher privileges.

### 5. Remediation
I reviewed how unnecessary permissions could be removed and why users should only receive the permissions they need.

### 6. Verification
After applying a fix, I checked the permissions again to confirm that the configuration had changed as expected.

## What I Learned
This practical helped me understand Linux permissions, sudo configuration, system enumeration, and the importance of documenting security findings properly.

## Lab Scope
All testing was intended for an isolated lab environment that I owned or was authorized to assess.
