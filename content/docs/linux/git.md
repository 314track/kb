---
title: "git"
draft: false
---

# git

## git config

### Configure user name

```bash
git config user.name 314track
```

### Configure users email address

```bash
git config user.email 235858822+314track@users.noreply.github.com
```

## Configure global default init branch

```bash
git config --global init.defaultBranch main
```

## Working with tags

```bash
git tag -a v1.4 -m 'version 1.4'
```

## Squash commits

```bash
git reset --soft $(git merge-base main HEAD)
```

## git checkout

Obtaining a specific Version of a file using a hash or a branch:

```bash
git checkout <branch name | commit hash> -- <file path>
```
