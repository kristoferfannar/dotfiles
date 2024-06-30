# Dotfiles

Welcome to my dotfiles repo. This is where I store some of my config settings.
This repo lives in the `$HOME` directory and is symlinked using [`stow`](https://www.gnu.org/software/stow/).

The inspiration for this comes from [Youtube | Stow has forever changed the way I manage my dotfiles](https://www.youtube.com/watch?v=y6XCebnB9gs).

## Setting up

If you're setting these dotfiles up on a new device, you might have some trouble configuring everything in the beginning as my config depends upon countless dependencies.

Some notable are:

- tmux
- neovim

Once that's done, you're ready to symlink these dotfiles from this directory to the `$HOME` directory using:

```bash
stow .
```

You might have conflicts as you're creating symlinks for files that already exist in `$HOME`.
Just rename those or delete them.
