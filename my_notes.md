sudo apt install rhash dialog libncurses-dev ntp && sudo systemctl stop ntp

git clone https://github.com/oddlama/gentoo-install

add new packages:

networkmanager iwd nm-applet xorg-server icewm firefox-bin xterm vim sudo zsh x11-misc/slim

setup:
  * sync and update everything
  * .xinitrc: icewm-session
  * .icewm/startup: nm-applet &
  * add a regular user with right groups and zsh
  * .xsession: icewm-session; config slim to autologin
