---
title: "zsh"
draft: false
---

# zsh

## Installation

```bash
sudo apt install zsh zplug
```

```bash
zsh
```

```bash
chsh -s /bin/zsh
```

## Install oh-my-zsh

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## Plugins

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

```bash
git clone https://github.com/zdharma-continuum/fast-syntax-highlighting.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/fast-syntax-highlighting
```

```bash
git clone --depth 1 -- https://github.com/marlonrichert/zsh-autocomplete.git $ZSH_CUSTOM/plugins/zsh-autocomplete
```

```bash
vim ~/.zshrc
```

```bash
plugins=(git ssh-agent gpg-agent zsh-autosuggestions zsh-syntax-highlighting fast-syntax-highlighting zsh-autocomplete colorize colored-man-pages)
```
