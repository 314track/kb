---
title: "adduser"
draft: false
---

# adduser

## add a user

```bash
adduser <username>
```

## add a user to an existing group

```bash
adduser <usernmae> <groupname>
```

## add a system user without login and no homedirectory

```bash
adduser --system --no-create-home --shell /usr/sbin/nologin --group <serviceuser>
```
