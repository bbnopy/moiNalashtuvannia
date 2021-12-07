# ARCHlinux

## Vstanovlennia ARCHlinux

### Zavantazhennia

Na [archlinux.org](https://archlinux.org) u rozdili **Downloads** zavantazhuiemo ISO

### Haid po vstanovlenniu

[Installation Guide](https://wiki.archlinux.org/index.php/installation_guide)

### Vstanovlennia na virtualnu mashynu

```zsh
# ping google.com
```

### Hodynnyk

```zsh
# timedatectl set ntp true
# timedatectl status
```

### Rozmitka dysku

```zsh
# cfdisk
```

| Mount Point |  Partition   | Partition type |     Size    |
|-------------+--------------+----------------+-------------|
|     SWAP    | /dev/sd*\X*1 |   Linux swap   | 1:1 abo 1:2 |
|     /mnt    | /dev/sd*\X*2 |      Linux     |     15Gb    |
|   /mnt/var  | /dev/sd*\X*3 |      Linux     |   10-30GB   |
|  /mnt/home  | /dev/sd*\X*4 |      Linux     |   zalyshok  |

dali vybyraiemo **Write** potim **Quit**

### SWAP rozdil

```zsh
# mkswap /dev/sdX1
# swapon /dev/sdX1
```

### Formatuvannia dysku

```zsh
# mkfs ext4 /dev/sdX2
# mkfs ext4 /dev/sdX3
# mkfs ext4 /dev/sdX4
```

### Montuvannia rozdilu

```zsh
# mount /dev/sdX2 /mnt
# mkdir /mnt/var
# mount /dev/sdX3 /mnt/var
# mkdir /mnt/home
# mount /dev/sdX4 /mnt/home
```

### Redahuiemo dzerkala

```zsh
# nano /etc/pacman.d/mirrorlist
```

### Vstanovlennia

bazova komanda vstanovliuie vse neobkhidne

```zsh
# pacstrap /mnt base linux linux firmware
```

vse inshe treba vstanovliuvaty samostiino

```zsh
# pacstrap /mnt base linux linux-firmware base-devil sudo man-pages inetutils netctl dhcpcd s-nail vi vim
```

### Tochka montuvannia Fastab

```zsh
# genfstab -U /mnt >> /mnt/etc/fstab
# cat /mnt/etc/fstab
```

### Perekhid na ROOT vstanovlenoi systemy

```zsh
# arch-chroot /mnt
```

### Chazova zona

```zsh
# ln -sf /usr/share/zoneinfo/Riehion/Misto /etc/localtime
# hwclock --systoch
```

### Localization

Redahuiemo */etc/local.gen*, rozkomentuiemo potribnu movu, heneruiemo *locale*

```zsh
# locale-gen
# echo 'LANG=lang_LANG.UTF-8' > /etc/locale.conf
```

### Nalashtuvannia NETWORK

Vidkryvaiemo */etc/hostname*

```nano
myhostname
```

teper */etx/hosts*

```nano
127.0.0.1   localhost
::1         localhost
127.0.1.1   myhostname.localhost myhostname
```

### ROOT parol

```zsh
# passwd
```

### Vkliuchaiemo DHCP dlia NETWORK

```zsh
# systemctl enable dhcpcd
```

### Dodaiemo korystuvacha i parol

```zsh
# useradd -m username
# passwd username
```

### Dodaiemo korystuvacha do hrup

```zsh
# usermod -aG wheel,lp,network,sys,power,audio username
# groups username
```

vidkryvaiemo *visudo* i rozkomentuiemo riadok **%wheel ALL=(ALL) ALL**

### Vstanovliuiemo GRUB

```zsh
# pacman -S grub
# grub-install /dev/sda
# grubmkconfig -a /boot/grub/grub.cfg
```

### Nalashtuvannia internetu

pry vstanovleni ne na virtualnu mashynu potribno vstanovyty i nalahtuvaty internet

**WiFi**

vstanovlennia **iwd**

```zsh
$ sudo pacman -S iwd
$ sudo systemctl enable iwd
$ sudo systemstl start iwd
```

Zapuskaiemo *iwctl shell*

```zsh
$ iwctl
[iwd]$ device list
[iwd]$ station device scan
[iwd]$ station device get-network
[iwd]$ station device connect SSID
```

**Perezavantazhuiemosia**

```zsh
# exit
# shutdown now
```

vidkliuchaiemo ISO i zapuskaiemo systemu, spochatku pereviriaiemo internet

```zsh
$ ping google.com
```

### Vstanovlennia XORG

```zsh
$ sudo pacman -S xorg xorg-server
```