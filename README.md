# tooling


## Linux setup


```
sudo -s

apt-get install git terminator git-cola dstat
```


Adding sublime
```
wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -
echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list
apt-get update
apt-get install sublime-text

```

Adding atom
```
snap install atom --classic
```

Adding vlc
```
snap install vlc
```

Setting up gnome extensions

```
apt-get install chrome-gnome-shell gnome-tweak-tool

```

```
apt-get install chrome-shell-pomodoro
```

Extensions to add

 - extensions
 - dash to dock
 - AlternateTab
 - TopIcons Plus 
 - Sound Input & Output Device Chooser
 - Clipboard Indicator
 - Applications Menu
 - Coverflow Alt-Tab
 - Disconnect Wifi 
 - Drop Down Terminal
 - Frippery Move Clock 
 - NetSpeed 
 - Refresh Wifi Connections
 - Suspend and Lock Button 
 - System Monitor (sudo apt install gir1.2-gtop-2.0 libgtop2-dev)
 - system-monitor
 - Screenshot Tool
 - Volume Mixer 
 - Status Area Horizontal Spacing 
 - User Themes (sudo apt-get install gnome-shell-extensions)

Look into
 - taskbar


Setting up docker (https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-18-04)
```
apt install -y apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"
apt update
# apt-cache policy docker-ce
apt install -y docker-ce
systemctl status docker

```

Add current user to docker group (RUN AS USER)
```
sudo usermod -aG docker ${USER}
su - ${USER}
id -nG
```

Installing docker-compose (https://www.digitalocean.com/community/tutorials/how-to-install-docker-compose-on-ubuntu-18-04)

```
curl -L https://github.com/docker/compose/releases/download/1.21.2/docker-compose-`uname -s`-`uname -m` -o /usr/local/bin/docker-compose
chmod +x /usr/local/bin/docker-compose

```


