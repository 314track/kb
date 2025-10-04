---
title: "ghorg"
draft: false
---

# ghorg

Quickly clone an entire org/users repositories into one directory - Supports GitHub, GitLab, Bitbucket, and more

`https://github.com/gabrie30/ghorg`

Place GitLab PAT in the file `~/.gitlab-pat`. The PAT must have at least read_api permissions.
Copy ghorg to `~/bin`.

```bash
ghorg clone <gitlab group> --scm=gitlab --protocol=ssh --base-url=<Webendpunkt> --output-dir=<gitlab instance> --preserve-dir --token=$(cat ~/.gitlab-pat)
```
