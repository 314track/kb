---
title: "find"
draft: false
---

# find

## Delete log files that have not been modified for more than 30 days

```bash
find </path/to/files/> -type f -name '*.log' -mtime +30 -exec rm {} \;
```

## Delete log files that are older than 14 days

```bash
find ./ -name '*.log' -mtime +14 -type f -delete
```

```bash
find ./ *.log -mtime +14 -type f -exec rm {} \;
```
