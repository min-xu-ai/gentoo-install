sudo apt install rhash dialog libncurses-dev ntp && sudo systemctl stop ntp

git clone https://github.com/oddlama/gentoo-install

add new packages:

networkmanager iwd nm-applet xorg-server icewm firefox-bin font-misc-misc alacritty vim sudo zsh x11-misc/slim

setup:
  * sync and update everything
  * .xinitrc: icewm-session -> config in .icewm
  * .icewm/startup or .config/icewm/startup: nm-applet &
  * add a regular user with right groups and zsh
  * .xsession: icewm-session; config slim to autologin; config in .config/icewm
  * install rofi: set "Super+Space" and "Super+Shift+Space" keys in .config/icewm/keys to call it up with rofi -show drun and rofi -show run
  * install apcilight: use xbacklight in keys config for keyboard control of monitor brightness
  * python venv: glances, rickslab-gpu-utils (need to comment out some code to run gpu-mon in text mode)
