<div align="center">

# 💌 My fork of JaKooLit's Debian/Ubuntu Hyprland Install Script 💌

</div>

### ⚠️ Pre-requisites and VERY Important! ###
- Do not run this installer as sudo or as root
- This Installer requires a user with a priviledge to install packages
- Needs a Debian 13 Testing (Trixie) Branch  as it needs a newer wayland packages! I have tried on Stable Debian 12 Bookworm in which, Hyprland wont build.
- In theory, it should also work on Debian SID (unstable) but I have not tested yet.
- edit your /etc/apt/sources.list and remove # on lines with deb-src to enable source packaging else will not install properly especially Hyprland
```bash
sudo nano /etc/apt/sources.list
```
- delete # on the lines with 'deb-src' 
- ensure to allow to install non-free drivers especially for users with NVIDIA gpus. You can also install non-free drivers if required. Edit install-scripts/nvidia.sh and change the nvidia stuff's if required
- If you have login Manager already like GDM (gnome login manager), I highly advice not to install SDDM. But if you decide to install SDDM, see here [`Issue 2 - SDDM`](https://github.com/JaKooLit/Debian-Hyprland/issues/2)



### ✨ to run
> clone this repo by using git. Change directory, make executable and run the script
```bash
git clone https://github.com/JaKooLit/Debian-Hyprland.git
cd Debian-Hyprland
chmod +x install.sh
./install.sh
```
### ✨ for ZSH and OH-MY-ZSH installation
> do this once installed and script completed; do the following to change the default shell zsh
```bash
chsh -s $(which zsh)
zsh
source ~/.zshrc
```
- reboot or logout
- by default mikeh theme is installed. You can find more themes from this [`OH-MY-ZSH-THEMES`](https://github.com/ohmyzsh/ohmyzsh/wiki/Themes)
- to change the theme, edit ~/.zshrc ZSH_THEME="desired theme"

### 👍👍👍 Thanks and Credits!
- Of course to [Hyprland](https://hyprland.org/) and @vaxerski for this awesome Dynamic Tiling Manager.   [JaKooLit](https://github.com/JaKooLit) for his scripts and dotfiles.
- shout out to CooSee from Gentoo forums for the nice rainbow borders
  
