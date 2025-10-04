---
title: "ssh-agent"
draft: false
---

# ssh-agent

## Start ssh-agent

```bash
eval $(ssh-agent)
``` 

In Windows, the service must first be started.
The space between start and auto must be retained.

```powershell
sc config ssh-agent start= auto
```
