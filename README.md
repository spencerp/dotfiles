In `~/.bashrc`:
```
DOTFILES=~/dotfiles/sh/bashrc

# Reference custom dotfiles
if [ -f $DOTFILES ]; then
        . $DOTFILES
fi
```

In `~/.bash_profile`:
```
# Get the aliases and functions
if [ -f ~/.bashrc ]; then
        . ~/.bashrc
fi
```

In `~/.zshrc`:
```
DOTFILES=~/dotfiles/sh/zshrc

# Reference custom dotfiles
if [ -f $DOTFILES ]; then
        . $DOTFILES
fi
```
