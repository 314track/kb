---
title: "apt"
draft: false
---

# apt

Find out which packages were installed via apt and when.
This can be checked in the file /var/log/apt/history.log.

## update list of available packages

```bash
apt update
```

## list installed packages

```bash
apt list --installed
```

## upgrade the system by removing/installing/upgrading packages

```bash
apt full-upgrade
```
