# dotfiles

These dotfiles contain all of the necessary packages, plugins and config I need to be a productive (Python/Javascript) developer. They mostly concern [Kitty](https://sw.kovidgoyal.net/kitty), zsh, tmux and vim.

![my setup](./screenshot.png)

I've tested these dotfiles on both ubuntu and OS X.

**NOTE - you will need vim version 8.0 or higher.**

## Contents

- custom config for vim/nvim, ack-grep, zsh, eslint, tmux and kitty
- [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
- vim plugins:
  - [ale](https://github.com/w0rp/ale)
  - [ctrlp.vim](https://github.com/kien/ctrlp.vim)
  - [nerdtree](https://github.com/scrooloose/nerdtree)
  - [vim-nerdtree-tabs](https://github.com/jistr/vim-nerdtree-tabs)
  - [vim-gitgutter](https://github.com/airblade/vim-gitgutter)
  - [vim-airline](https://github.com/bling/vim-airline)
  - [tagbar](https://github.com/majutsushi/tagbar)
  - [vim-easytags](https://github.com/xolox/vim-easytags)
  - [vim-javascript](https://github.com/pangloss/vim-javascript)
  - [vim-jsx](https://github.com/mxw/vim-jsx)
  - [typescript-vim](https://github.com/leafgarland/typescript-vim)
- vim colorschemes:
  - [termschool-vim-theme](https://github.com/marcopaganini/termschool-vim-theme)
- TMUX plugins
  - [tpm](https://github.com/tmux-plugins/tpm)
  - [tmux-resurrect](https://github.com/tmux-plugins/tmux-resurrect)
  - [tmux-yank](https://github.com/tmux-plugins/tmux-yank)

## Requirements

- These dotfiles are designed to work best with the Kitty terminal emulator. Download and install the latest binaries here - https://sw.kovidgoyal.net/kitty/binary.html

- Ensure you have zsh installed
```
linux:
sudo apt-get install zsh

mac:
brew install zsh
```
- Ensure zsh is set as your default shell:
```
chsh -s $(which zsh)
```
Note: you will need to logout and log back in for this to take effect

- Ensure you have flake8 installed (for ale python linting)
```
sudo pip install flake8
```
- Ensure you have exuberant-ctags installed (for vim tags and tagbar)
```
linux:
sudo apt-get install exuberant-ctags

mac:
brew install ctags
```
- Ensure you have eslint requirements installed (for ale js linting)
```
sudo npm install -g eslint eslint-config-tomjwatson
```
- Set your terminal background to `#3a3a3a` for best integration with tmux config

## Installation

- Clone the repository and install the configs
```
git clone https://github.com/tom-james-watson/dotfiles

cd dotfiles

./install.sh
```

- To install the tmux plugins, start tmux and run `prefix` + <kbd>I</kbd>.

- To install the vim plugins, open vim and run
```
:PlugInstall
```

## Updating

```
./update.sh
```
