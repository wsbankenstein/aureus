# aureus
a minimal AUR helper written in bash

## Installing AUR packages
`aureus -S` (no args) gives you a lovely searchable package list. find the one you want and press Enter to install it!

## Updating AUR packages
`aureus` updates all AUR packages that have newer versions available on the AUR.
(this is actually an alias to `aureus -U` which does the same thing.)

## Deleting packages
`aureus -R` gives you a list of all your installed packages (including non-AUR ones), and pressing Enter runs `sudo pacman -Rsnc $package`.
(yes, the default delete operation is -Rsnc. i should probably change that)

## Information about installed packages
`aureus -Q` gives you a list of all your installed packages (including non-AUR ones). and pressing Enter runs `pacman -Qil $package`.
