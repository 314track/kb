---
title: "sysctl"
draft: false
---

# sysctl

## Show all configuration variables

```bash
sudo sysctl -p
```

## configure swappiness

### Show value

```bash
cat /proc/sys/vm/swappiness
```

```bash
sudo sysctl -a | grep swappiness
```

### Change value (temporary)

```bash
sysctl vm.swappiness=10
```
