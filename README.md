# ArchBackup
Stuff that needs to be transferred over to the new PC in the files.

Made by @TomeQ_537

### Step 1: Install Arch Linux

https://github.com/TomeQ537/How-to-install-arch-linux/tree/main

### Step 2: Download the ML4W dotfiles:

https://github.com/mylinuxforwork/dotfiles

### Step 3: Replace the .mydotfiles folder with the new one

### Step 4: Download the packagelists/flatpaks

Download the 2 .txt files with the flatpak list and put them onto your home folder, then input the following commmands:

```
sudo pacman -S --needed - < ~/pacman_list.txt
```

```
yay -S --needed - < ~/yay_list.txt
```
For flatpak:

Ensure flathub is setup:

```
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
```

Install the stuff:

```
xargs -a ~/flatpak_list.txt flatpak install -y flathub
```

### Step 5: Reboot and enjoy!

