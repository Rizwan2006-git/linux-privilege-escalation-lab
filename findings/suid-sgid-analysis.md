# SUID and SGID Analysis

## What I learned

During my Linux privilege escalation practice, I learned about SUID and SGID permissions and why they are important in Linux security.

SUID allows a program to run with the file owner's effective user ID. SGID can allow a program to run with the file group's effective group ID.

## What I checked

I learned how to search for files with special permission bits using Linux commands and how to review their ownership and permissions.

```bash
find / -type f -perm -4000 2>/dev/null
find / -type f -perm -2000 2>/dev/null
```

## Why it matters

Some programs need these permissions to work correctly, so finding an SUID or SGID file does not automatically mean it is vulnerable.

The important part is checking whether the permissions, ownership, or program behavior create a security risk.

## Security recommendations

- Review special-permission files regularly.
- Remove unnecessary SUID or SGID permissions.
- Check file ownership and write permissions.
- Keep the operating system and installed software updated.

## What I learned

This helped me understand how special Linux permissions work and how to investigate them during a security assessment.

## Evidence

I will add the results from my own lab after reviewing the files and their permissions.
