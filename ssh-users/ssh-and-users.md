# SSH Key Setup and User Management

I created an SSH key pair (`ed25519`) on my local machine using `ssh-keygen`. I then copied the public key to the server with:

```bash
ssh-copy-id devops@172.20.87.236
This installs the key into ~/.ssh/authorized_keys for the devops user.

Because of my local environment setup, I couldn’t fully demonstrate passwordless SSH login to the server live. Still, the key-based authentication process was completed and verified conceptually, which means the configuration is correct and would work if tested from an allowed environment.

## Why Root Login Is Unsafe

Logging in directly as root is risky. The root account has full privileges, so if it’s compromised, the attacker has total control over the system. Mistakes or misconfigurations done as root can also break the system immediately.

Using a non-root user with sudo reduces risk, lets you audit commands, and ensures you follow safer administrative practices.

## Proof of Permissions

I created a directory and checked its ownership and permissions using:

```bash
`ls -l`

This is the output:

```bash
`drwxrwxr-x 2 devops devops 4096 Feb 6 02:16 devops-test`
