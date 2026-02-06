# Linux Server Setup

## Server Environment
- OS: Ubuntu 22.04.5 LTS
- Kernel: GNU/Linux 6.6.87.2-microsoft-standard-WSL2 x86_64
- Username: nana
- Hostname: Nana
- IPv4 Address: 172.20.87.236
- Disk Usage: 0.1% of 1006.85GB
- Memory Usage: 5%
- Swap Usage: 0%
- Number of processes running: 66

## Steps Taken
1. Installed WSL2 on Windows.
2. Installed Ubuntu 22.04 LTS via Microsoft Store.
3. Logged in as user `nana`.
4. Verified the environment using the following commands:
   - `uname -a` → kernel information
   - `lsb_release -a` → OS version
   - `hostname` → machine hostname
   - `df -h` → disk usage
   - `free -m` → memory usage
