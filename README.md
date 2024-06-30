# Dotfiles

Welcome to my dotfiles repo. This is where I store some of my config settings.
This repo lives in the `$HOME` directory and is symlinked using [`stow`](https://www.gnu.org/software/stow/).

The inspiration for this comes from [Youtube | Stow has forever changed the way I manage my dotfiles](https://www.youtube.com/watch?v=y6XCebnB9gs).

## Setting up

If you're setting these dotfiles up on a new device, you might have some trouble configuring everything in the beginning as my config depends upon countless dependencies.

Of course, you'll first need a package manager. I use [`brew`](https://brew.sh/).

Some notable dependencies are:

- `stow`
- `tmux`
- `neovim`

### Installation

With a package manager and the necessary dependencies installed,
you're ready to symlink these dotfiles from this directory to the `$HOME` directory:

```bash
# from $HOME
git clone git@github.com:kristoferfannar/dotfiles.git
cd dotfiles

stow .
```

You might have conflicts as you're creating symlinks for files that already exist in `$HOME`.
Just rename those or delete them.
