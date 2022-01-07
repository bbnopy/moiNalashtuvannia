# Vstanovlennia XORG

```zsh
$ sudo pacman -S xorg xorg-server
```

# Openbox

osnovni pakunky
```zsh
$ sudo pacman -S lightmd lightdm-gtk-greeter openbox obconf pcmanfm
```

dodatkovi pakunky
```zsh
$ sudo pacman -S tint2 xterm alacritty nitrogen geany unzip xarchiver gnome-background manumaker
```

## Aktyvuiemo LIGHTDM

```zsh
$ sudo systemctl enable lightdm
$ sudo reboot now
```

Robymo **reboot**, pislia choho mozhna vykorystovuvaty desktop

## Menu v OPENBOX

rekonfihuratsiia meniu

```zsh
$ mmaker openbox -f -t terminal
```

# YAY Package manager

vstanovlennia

```zsh
$ pacman -S --needed git base-devel
$ git clone https://aur.archlinux.org/yay.git
$ cd yay
$ makepkg si
```

# PAMAC

```zsh
$ sudo pacman -S --needed base-devel git wget yajil
$ cd /tmp
$ git clone https;//aut.archlinux.org/package-query.git
$cd package-query/
$ makepkg -si
$ yay -S pamac-aur
```