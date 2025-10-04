---
title: "systemd"
draft: false
---

# systemd

## Clear DNS cache

```bash
systemd-resolve --flush-caches
```

## Bindmount with systemd

Example for GitLab logs

```bash
cat << EOF > /etc/systemd/system/var-opt-gitlab.mount
[Unit]
Description=Bind mount from /var/opt/gitlab to /data/var/opt/gitlab
 
[Mount]
What=/data/var/opt/gitlab
Where=/var/opt/gitlab
Type=none
Options=bind
 
[Install]
WantedBy=local-fs.target
EOF
```
