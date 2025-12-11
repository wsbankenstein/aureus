# aureus
a minimal AUR helper written in bash

## Installation
```
git clone https://aur.archlinux.org/aureus.git
cd aureus
makepkg -si
```

(this is how you install AUR packages without an AUR helper. it's also what aureus does!)

## Installing AUR packages
`aureus -S` (no args) gives you a lovely searchable package list. find the one you want and press Enter to install it!

## Updating AUR packages
`aureus` updates all AUR packages that have newer versions available on the AUR.

(this is actually an alias to `aureus -U` which does the same thing.)

## Removing packages
`aureus -R` gives you a list of all your installed packages (including non-AUR ones), and pressing Enter yeets the package and all packages that depend on it (`sudo pacman -Rsnc $package`).

(yes, the default remove operation is -Rsnc. i should probably change that)

## Information about installed packages
`aureus -Q` gives you a list of all your installed packages (including non-AUR ones), and pressing Enter shows the corresponding package info + file list (`pacman -Qil $package | less`).

---

This project is on [GitHub](https://github.com/wsbankenstein/aureus) and [Codeberg](https://codeberg.org/bankenstein/aureus).

If you have suggestions, please use the issue trackers or contact me at `aureus () martinbogdanov . com`.
