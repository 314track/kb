---
title: "bash"
draft: false
---

# bash

Some stuff about bash

## Arguments

### Use of !$ (last argument of the previous command)

```bash
ls -l -a
ls !$
```

Leads to `ls -a`

### Use of !^ (first argument of the previous command)

```bash
ls -l -a
ls !$
```

Leads to `ls -l`

### Repeat the entire last command

```bash
ls -ltrha

sudo !!
```

Leads to `sudo ls -ltrha`

## Output information about installed NVMe SSD

```bash
for disk in /dev/nvme?n1; do echo $disk; smartctl -A $disk | grep -E 'Power On Hours|Data Units'; done
```
