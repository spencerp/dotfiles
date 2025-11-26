In `~/.bashrc`:
```
DOTFILES=~/spencerp/dotfiles/sh/bashrc

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
DOTFILES=~/spencerp/dotfiles/sh/zshrc

# Reference custom dotfiles
if [ -f $DOTFILES ]; then
        . $DOTFILES
fi
```

## Git Configuration

To apply the gitconfig globally:
```bash
git config --global include.path ~/spencerp/dotfiles/git/gitconfig
```

This will include the custom git configuration (aliases, push settings, LFS filters) in your global git config.
