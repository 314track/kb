---
title: "rsync"
draft: false
---

# rsync

## Synchronize local directories

```bash
rsync -vaxSHAX --delete <source directory> <target directory>
```

## Synchronize local directory with SSH target directory

```bash
rsync -vaxSHAX --delete /<source directory>/ root@server.example.com:/<target directory>/
```
