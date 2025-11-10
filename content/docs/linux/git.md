---
title: "git"
draft: false
---

# git

## git config

### List git global configuration

```bash
git config --global --list
```

### List git configuration

```bash
git config --list
```

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

## git switch

Switch to an existing branch

```bash
git switch <existing branch>
```

Create a new branch

```bash
git switch -c <fix|feature/branch name>
```


## git checkout

Obtaining a specific Version of a file using a hash or a branch:

```bash
git checkout <branch name | commit hash> -- <file path>
```
