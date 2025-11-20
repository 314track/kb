---
title: "ansible-playbook"
draft: false
---

# ansible-playbook

Set limit for all groups, without a specific host

```bash
all:!<without host>
```

Set limit for a union set of group_a and group_b

```bash
group_a:&group_b
```

