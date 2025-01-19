# Dotfiles

These are dotfiles I use for my Linux development environment (currently debian)

## Requirements

Ensure you have the following installed:

### Git

```sh
apt-get install git
```

### Stow

```sh
apt-install stow
```

## Installation

Clone the repo in your `$HOME` directory with git

```sh
# SSH
git clone git@github.com:kashje/.dotfiles.git

# HTTPS
git clone https://github.com/kashje/.dotfiles.git
```

After that use GNU Stow to create symlinks from the `.dotfiles` directory to your `$HOME` directory

```sh
stow .
```

If you ever need to ignore files that don't have to be symlinked you can create/add to a `.stow-local-ignore` file

```sh
# Add file
touch .stow-local-ignore

# Add files/folders to the stow ignore
echo .git >> .stow-local-ignore
```
