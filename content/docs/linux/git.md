---
title: "git"
draft: false
---

# git

## git config

List git global configuration

```bash
git config --global --list
```

List git configuration

```bash
git config --list
```

Configure user name

```bash
git config user.name 314track
```

Configure users email address

```bash
git config user.email 235858822+314track@users.noreply.github.com
```

Configure global default init branch

```bash
git config --global init.defaultBranch main
```

## git tag

Create a tag

```bash
git tag -a v1.4 -m 'version 1.4'
```

List all local tags

```bash
git tag
```

List local tags with annotation message

```bash
git tag -n
```

List local tags matching a pattern

```bash
git tag -l "<pattern>"
```

List all remote tags

```bash
git ls-remote --tags <remote-name>
```

Fetch tags from remote and list locally

```bash
git fetch --tags
```

```bash
git tag -l
```

Delete an existing tag

```bash
git tag -d v1.4
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

Obtain a specific version of a file using a hash or a branch:

```bash
git checkout <branch name | commit hash> -- <file path>
```

# git workflows

## Squash commits

```bash
git reset --soft $(git merge-base main HEAD)
```
