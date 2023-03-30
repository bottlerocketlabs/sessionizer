# sessionizer

## Use sessionizer with zellij

start sessionizer as shell command

```yaml
# alacritty.yml
shell:
  program: /usr/local/bin/zsh
  args:
    - -c
    - /Users/you/.local/bin/sessionizer
```

detach from current session to select another

## Use sessionizer with tmux

run sessionizer within tmux session

```conf
# tmux.conf
bind-key p run-shell "tmux neww ~/.local/bin/sessionizer"
bind-key F1 run-shell "tmux neww ~/.local/bin/sessionizer somegitreponame"
```

## credit

* [https://github.com/ThePrimeagen/.dotfiles/blob/master/bin/.local/scripts/tmux-sessionizer]
* [https://github.com/zellij-org/zellij/issues/884#issuecomment-1250483279]
