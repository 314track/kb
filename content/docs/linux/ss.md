---
title: "ss"
draft: false
---

## ss

Socket statistics

## Check whether port 3306 (MySQL/MariaDB) is open

```bash
ss -tan | grep -i 3306
```

## Display all listening ports

```bash
ss -l
```

## Show all TCP connections with process info

```bash
ss -tup
```

## Filter by status (e.g., ESTABLISHED)

```bash
ss -ant state established
```
