---
title: "ssh-keygen"
draft: false
---

# ssh-keygen

##  Create private/public key

```bash
ssh-keygen -t ed25519 -C "<name>@e<host>" [-f ~/.ssh/<filename>]
```

## Convert multiline private key to single-line private key

```bash
ssh-keygen -y -f multiline_private_key_file > public_key_file.pub
```
