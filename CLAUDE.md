# Dotfiles

Personal shell configuration and dotfiles.

## Shell Aliases (sh/aliases.sh)

| Alias | Command | Description |
|-------|---------|-------------|
| `ls` | `ls -p -G` | List with trailing slashes and colors |
| `ll` | `ls -l -h --color` | Long listing with human-readable sizes |
| `editlocal` | `vim $HOME/dotfiles/sh/local.sh; source ...` | Edit and reload local shell config |
| `dotfiles` | `vim $HOME/dotfiles` | Open dotfiles in vim |
| `t250` | `tail -n250` | Tail last 250 lines |
| `vi` | `vim --noplugin` | Vim without plugins |
| `hosts` | `sudo vim /etc/hosts` | Edit hosts file |
| `tmuxw` | `tmux new -s w` | New tmux session named 'w' |
| `ed` | `emacs --daemon` | Start emacs daemon |
| `e` | `emacsclient -nw` | Connect to emacs in terminal |
| `d` | `docker` | Docker shorthand |
| `a` | `atom` | Atom editor |
| `fd <pattern>` | `find . -name "*$1*"` | Find files matching pattern |
| `... \| gp <text>` | `xargs grep -l "$1"` | Grep piped files for text |

Example: `fd yaml_gen | gp DocProc` - Find files with "yaml_gen" in name that contain "DocProc"
