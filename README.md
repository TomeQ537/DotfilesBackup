# ArchBackup
Stuff that needs to be transferred over to the new PC in the files.

Made by @TomeQ_537 for @TomeQ_537

### Step 1: Install Arch Linux

https://github.com/TomeQ537/How-to-install-arch-linux/tree/main

### Step 2: Download the ML4W dotfiles:

https://github.com/mylinuxforwork/dotfiles

### Step 3: Download the default papirus icons and set them to dark (KDE)

### Step 4: Replace the .mydotfiles folder with the new one

After you clone the folder, you can just delete the old folder and move the new folder replacing the old one.

```
cd .mydotfiles
```

```
git clone https://github.com/TomeQ537/DotfilesBackup.git
```

### Step 5: Download programs

Ensure flathub is setup:

```
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```

Pacman:

```
sudo pacman -S btop cava gnome-disk-utility gnome-keyring gnome-text-editor gparted ntfs-3g openrgb samba steam taskwarrior-tui wine winetricks
```

Yay:

```
yay -S qimgv theclicker
```

Flatpak:

```
flatpak install app.zen_browser.zen com.discordapp.Discord com.protonvpn.www com.usebottles.bottles md.obsidian.Obsidian org.gnome.Calculator org.kde.kwalletmanager5 org.mozilla.Thunderbird org.prismlauncher.PrismLauncher org.videolan.VLC org.vinegarhq.Sober
```

### Step 6: Reboot and enjoy!

### Extra: 

Add this line at the bottom:

```
sudo nano /etc/sudoers
```

```
tomeq537 ALL=(ALL) NOPASSWD:ALL
```

Zen mods: 

Download BG, SuperPins

;)

```
sudo nano /etc/pacman.conf
```

ILoveCandy
