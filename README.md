# Arch Linux package lists
This reposutory contains lists of packages for Arch Linux.

## Installation
To install pacman packages run:
```sh
# pacman -S --needed - < pacman.txt
```
See the [ArchWiki](https://wiki.archlinux.org/index.php/Pacman/Tips_and_tricks#Install_packages_from_a_list) for details.

To install AUR packages run:
```sh
$ git submodule update --init
```
after run `makepkg --syncdeps --install --clean` for each submodule from `aur` directory.
