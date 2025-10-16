# Zsh Configuration Setup

This repository contains my personal Zsh configuration using **Oh My Zsh** and useful plugins.

## Installation

```bash
sudo apt install zsh
```
```bash
# oh my zsh
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```
```bash
# zsh-syntax-highlighting
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git \
  ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting

# zsh-autosuggestions
git clone https://github.com/zsh-users/zsh-autosuggestions \
  ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

# clone config
mv ~/.zshrc ~/.zshrc.backup
git clone https://github.com/that-fela/zsh-config.git ~/.temp && mv ~/.temp/.zshrc . && rm -rf ~/.temp

# apply config
source ~/.zshrc
```
