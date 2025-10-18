---
title: "csli"
draft: false
---

# Crowdsecurity CLI

## List installed configurations

```bash
sudo cscli hub list
```

## List which collections are active

```bash
sudo cscli collections list
```

## Install Collection for GitLab

```bash
sudo cscli collections install timokoessler/gitlab
```

## Display which IP was banned and why

```bash
sudo cscli decisions list --type ban
```

## Show decisions

```bash
sudo cscli decisions list
```
