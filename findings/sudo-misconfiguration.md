# Linux Privilege Escalation - Sudo Misconfiguration

## What I did
In this project, I worked on a Linux privilege escalation lab using Kali Linux and Ubuntu Server. My goal was to understand how a normal user can get more privileges if the system is not configured properly.

## What I found
While checking the sudo permissions, I found a misconfigured rule that allowed the `student` user to run the `find` command as root without entering a password.

## How I tested it
I checked the user's permissions using `sudo -l` and then tested the allowed command in my lab environment. This helped me understand how a small mistake in sudo configuration can create a serious security risk.

## Why this is a problem
If a normal user can run certain programs with root privileges, they might be able to execute other commands with higher permissions and gain control over the system.

## How to fix it
- Remove unnecessary permissions from the sudoers file.
- Give users only the permissions they actually need.
- Check sudo permissions regularly.
- Test the configuration again after making changes.

## What I learned
From this practical, I learned how to check sudo permissions, understand a privilege escalation risk, and why proper Linux permission management is important.

## Status
This document describes my lab finding. I will add my screenshots and final verification results as I organize the project.
