# Fixing Sudo Permissions

## What was the issue?
During my Linux privilege escalation lab, I worked with a sudo rule that allowed a normal user to run the `find` command with root privileges without a password.

## How I fixed it
I opened the sudoers configuration using `visudo` and removed the unnecessary permission granted to the test user.

## How I verified the fix
After making the change, I checked the user's permissions again using `sudo -l`. I confirmed that the unwanted permission was no longer listed.

## Why this matters
Users should only have the permissions they need. Unnecessary sudo permissions can create security risks and may allow a normal user to perform administrative actions.

## What I learned
This exercise helped me understand the importance of reviewing sudo rules, applying the principle of least privilege, and verifying security fixes after making configuration changes.

## Note
These steps are documented for an isolated Linux lab environment.
