---
title: "lsof"
draft: false
---

# lsof

List Open Files.

Is solver than ss. If only ports are of interest, ss should be used.

## Check whether a local TCP port is open

```bash
lsof -i tcp:3306
```

## Diaply open ports on a host

```bash
sudo lsof -i -P -n | grep LISTEN
```

```bash
lsof -i -P -n -sTCP:LISTEN
```
