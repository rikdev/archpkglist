# Arch Linux package lists

This repository contains lists of packages for Arch Linux.

## Installation

To install pacman packages run:

```sh
sudo pacman -S --needed - < pacman.txt
```

See the
[ArchWiki](https://wiki.archlinux.org/index.php/Pacman/Tips_and_tricks#Install_packages_from_a_list)
for details.

To install AUR packages run:

```sh
git submodule update --init
```

after run `makepkg --syncdeps --install --clean` for each submodule from `aur` directory:

```sh
git submodule foreach 'makepkg --syncdeps --install --clean'
```

To update AUR packages run:

```sh
git submodule update --remote --recursive
```

after rebuild and update outdated packages:

```sh
git submodule foreach 'git clean -ffdx && makepkg --syncdeps --install --needed --clean'
```
