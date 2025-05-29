# 🐗 Linux Fundamentals

## 🐧 Linux Operating System Overview
- History and evolution of Linux
- Linux kernel vs distributions
- Open-source philosophy and licensing (GPL)
- Use cases: servers, desktops, embedded, IoT

## 🏗️ Linux Filesystem Structure
- Hierarchical directory structure (/ root)
- Essential directories:
  - /etc – system config
  - /home – user directories
  - /var – variable files/logs
  - /usr – user binaries, libraries
  - /bin, /sbin, /lib, /lib64
  - /dev, /proc, /sys, /run
- Filesystem types: ext4, XFS, Btrfs
- Mounting and unmounting
- Fstab and persistent mounts

## 🔄 Boot Process & Runlevels
- BIOS/UEFI to GRUB to kernel
- Init systems: SysVinit vs systemd
- Kernel loading and initrd
- Targets (runlevels) in systemd
- systemctl, journalctl, dmesg

## 🧑‍💻 Users, Groups & Permissions
- /etc/passwd, /etc/shadow, /etc/group
- File permissions (rwx), chmod, chown, umask
- SUID, SGID, Sticky Bit
- adduser, useradd, usermod, groupadd
- User context switching: su, sudo, /etc/sudoers

## 🗂️ Package Management
- Debian-based (apt, dpkg)
- Red Hat-based (yum, dnf, rpm)
- Arch-based (pacman)
- Building from source: `./configure && make && make install`
- Snap, Flatpak, AppImage

## 🔎 Process Management
- Foreground vs background processes
- ps, top, htop, kill, nice, renice
- systemctl for managing daemons
- Jobs: jobs, fg, bg, disown
- Signals and signal handling

## 🧰 Command Line Proficiency (Bash)
- Navigation: cd, ls, pwd
- File operations: touch, cp, mv, rm
- Viewing: cat, less, more, tail, head
- Text manipulation: grep, cut, awk, sed, tr
- Redirection: `>`, `>>`, `<`, `|`, `tee`
- Variables and quoting
- Command substitution: `$(...)`, backticks
- Globbing and wildcards: `*`, `?`, `[]`
- Loops and conditionals in bash

## 📜 Shell Scripting
- Creating scripts (`#!/bin/bash`)
- Arguments: `$1`, `$2`, `$@`, `$#`
- Control flow: `if`, `case`, `while`, `for`, `until`
- Functions and return values
- Exit codes and error handling
- Logging and debug (`set -x`, `trap`)

## 🌐 Networking in Linux
- `ip`, `ifconfig`, `ip a`, `ip route`
- Hostname and DNS: `/etc/hosts`, `/etc/resolv.conf`
- Network services: sshd, nginx, netcat
- `ping`, `netstat`, `ss`, `tcpdump`, `traceroute`, `curl`
- Opening ports and firewalls: `ufw`, `iptables`
- SSH key management: `ssh-keygen`, `ssh-copy-id`, `authorized_keys`

## 🧩 System Monitoring & Logs
- System logs in `/var/log`
- `journalctl` for systemd logs
- `uptime`, `free`, `vmstat`, `iostat`
- `top`, `htop`, `iotop`, `dstat`
- Custom log management with `logrotate`

## 🛡️ Linux Security Fundamentals
- Understanding root and least privilege
- `sudo`, `visudo`, `/etc/sudoers.d`
- AppArmor and SELinux basics
- `chmod`, `chown`, `setfacl`
- Secure shell (SSH) practices
- Disabling unused services
