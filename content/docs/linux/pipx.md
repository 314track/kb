---
title: "pipx"
draft: false
---

# pipx

Install and Run Python Applications in Isolated Environments

## Installation 

https://github.com/pypa/pipx

```bash
sudo apt update
sudo apt install pipx
pipx ensurepath
sudo pipx ensurepath --global # optional to allow pipx actions with --global argument
```

## Install a package

```bash
pipx install <package>
```

## Inject a module into an installed package

For example, if molecule-plugins is installed and the Python module docker is required.

```bash
pipx inject molecule-plugins docker
```

## Upgrade all packages

```bash
pipx upgrade-all
```

