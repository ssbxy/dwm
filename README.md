```
 ____ ____  ______  ____   __  ______        ____  __ 
/ ___/ ___|| __ ) \/ /\ \ / / |  _ \ \      / /  \/  |
\___ \___ \|  _ \\  /  \ V /  | | | \ \ /\ / /| |\/| |
 ___) |__) | |_) /  \   | |   | |_| |\ V  V / | |  | |
|____/____/|____/_/\_\  |_|   |____/  \_/\_/  |_|  |_|
```

# ssbxy DWM Fork
Personal fork of DWM                   

## Patches
* [attachbelow](https://dwm.suckless.org/patches/attachbelow/)
* [alwayscenter](https://dwm.suckless.org/patches/alwayscenter/)
* [fullgaps-toggle](https://dwm.suckless.org/patches/fullgaps/)
* [warp](https://dwm.suckless.org/patches/warp/)
* [pertag](https://dwm.suckless.org/patches/pertag/)
* [hide vacant tags](https://dwm.suckless.org/patches/hide_vacant_tags/)
* [splitstatus](https://dwm.suckless.org/patches/splitstatus/)

## Dependencies
### Pacman
```bash
sudo pacman -S base-devel git libx11 libxft xorg-server xorg-xinit
```
## Recommended Tools
* [slstatus](https://github.com/ssbxy/slstatus)
* [dmenu](https://tools.suckless.org/dmenu/)
* [slock](https://tools.suckless.org/slock/)

## .xinitrc
### Example
```bash
#!/bin/sh
#
# ~/.xinitrc
#
# Executed by startx (run your window manager from here)

## DWM
feh --bg-fill ~/Pictures/wallpaper.png
xrdb ~/.Xresources
picom &
slstatus &
exec dwm
```

## Build
```bash
git clone https://github.com/ssbxy/dwm.git
cd dwm
sudo make clean install
```
