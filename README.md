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

### Step 5: Download the packagelists/flatpaks

Download the .txt files and put them onto your home folder, then input the following commmands:

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

### Step 6: Reboot and enjoy!

### Extra: Remove sudo asking for password

Add this line at the bottom:

```
sudo nano /etc/sudoers
```

```
tomeq537 ALL=(ALL) NOPASSWD:ALL
```

;)

```
sudo nano /etc/pacman.conf
```

ILoveCandy
