# Linux Capabilities Misconfiguration

## Overview
In this part of my Linux privilege escalation project, I studied Linux capabilities and how incorrect configurations can create security risks.

## What are Linux capabilities?
Linux capabilities divide the privileges traditionally associated with root into smaller groups. This allows certain programs to perform specific privileged operations without necessarily having full root access.

## What I checked
I learned how to list the capabilities assigned to programs and investigate whether any of them provide more privileges than the program actually needs.

I used these commands to inspect capabilities:

```bash
getcap -r / 2>/dev/null
```

To check the capabilities of a specific process, I can also inspect its status:

```bash
grep Cap /proc/self/status
```

## Why this matters
Some capabilities can allow powerful actions. If a program receives unnecessary capabilities, a user may be able to misuse them to access resources or perform operations beyond their intended permissions.

However, finding a capability does not automatically mean that a vulnerability exists. The program, its configuration, and the user's access must also be considered.

## How to reduce the risk
- Remove unnecessary capabilities from programs.
- Give programs only the privileges they require.
- Review file capabilities regularly.
- Keep software updated.
- Investigate unusual capability assignments.

## What I learned
This topic helped me understand that Linux privileges are not limited to normal user permissions and sudo rules. Capabilities are another important area to review during a Linux security assessment.

## Assessment status
These are my learning notes. Any confirmed vulnerability should be documented with evidence from my own authorized lab.
