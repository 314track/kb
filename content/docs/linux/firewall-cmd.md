---
title: "firewall-cmd"
draft: false
---

# firewall-cmd

## KDE Connect with Debian firewall enabled

```bash
sudo firewall-cmd --zone=public --permanent --add-port=1714-1764/tcp
```

```bash
sudo firewall-cmd --zone=public --permanent --add-port=1714-1764/udp
```

```bash
sudo systemctl restart firewalld.service
```
