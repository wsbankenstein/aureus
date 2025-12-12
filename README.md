# aureus
a minimal AUR helper written in bash

## Installation
```
git clone https://aur.archlinux.org/aureus.git
cd aureus
makepkg -si
```

(this is how you install AUR packages without an AUR helper. it's also what aureus does!)

## Installing packages
`aureus -S` (for **S**ync, like in pacman) gives you a lovely searchable package list. find the one you want and press Enter to install it!

or, if you already know the name of the packages you want to install, `aureus -S pkg1 pkg2 pkg3...` just installs them.

## Updating packages
`aureus -U` (for **U**pgrade) updates all AUR packages that have newer versions available on the AUR.

`aureus -P` (for **P**acman) is an alias to `sudo pacman -Syu`.

`aureus` (no args) is an alias to `aureus -UP`.

## Removing packages
`aureus -R` (for **R**emove, like in pacman) gives you a list of all your installed packages (including non-AUR ones), and pressing Enter yeets the package and all packages that depend on it (`sudo pacman -Rsnc $package`).

or, if you already know the name of the packages you want to remove, `aureus -R pkg1 pkg2 pkg3...` just removes them.

(yes, the default remove operation is -Rsnc. i should probably change that)

## Information about installed packages
`aureus -Q` (for **Q**uery, like in pacman) gives you a list of all your installed packages (including non-AUR ones), and pressing Enter shows the corresponding package info + file list (`pacman -Qil $package | less`).

or, if you already know the name of the package you want info about, `aureus -Q pkgname` just gives it to you.

## Clearing the cache
`aureus -C` (for **C**lear) clears (by way of `rm -rf`) the aureus cache (usually `$HOME/.cache/aureus`).

## Multiple operations at once
You can combine operations any way you like!
- `aureus -UP` (upgrade everything)
- `aureus -SUP pkgname` (install `pkgname` and upgrade everything)
- `aureus -RC` (remove a package and clear the aureus cache)
- whatever else you can think of!

---

This project is on [GitHub](https://github.com/wsbankenstein/aureus) and [Codeberg](https://codeberg.org/bankenstein/aureus).

If you have suggestions, please use the issue trackers.

If there's something particularly urgent, please contact me at `aureus () martinbogdanov . com`.
