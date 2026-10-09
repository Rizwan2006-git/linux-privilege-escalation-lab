# SSH Key and File Permission Risks

## Overview
In this part of my Linux security project, I looked at how SSH keys are used for authentication and why protecting private keys is important.

## What are SSH keys?
SSH keys are used to authenticate users when connecting to a remote system. They usually work as a pair: a private key and a public key.

The private key must be kept secret, while the public key can be added to the remote system for authentication.

## What security risks did I study?
I learned that if a private SSH key is exposed or has unsafe permissions, another user might be able to access it. If the key is accepted by a remote server, this could lead to unauthorized access.

I also learned that saved credentials and SSH configuration files should be checked carefully during a Linux security assessment.

## How to check permissions
I used the following commands to inspect SSH files and their permissions:

```bash
ls -la ~/.ssh
ls -l ~/.ssh/id_ed25519
ls -l ~/.ssh/id_rsa
```

Some files may not exist, depending on how SSH is configured.

## How to reduce the risk
- Keep private SSH keys confidential.
- Restrict private-key file permissions.
- Remove unused keys from authorized accounts.
- Review the `authorized_keys` file.
- Disable access methods that are not needed.

For a private key owned by the current user, a common permission setting is:

```bash
chmod 600 ~/.ssh/id_ed25519
```

## What I learned
This helped me understand why SSH key security is important and how file permissions can affect remote access.

## Assessment status
This document describes the security checks I studied. Any confirmed vulnerability should be supported by evidence from my own authorized lab.
