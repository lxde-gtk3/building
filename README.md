# required packages
apt install `devscripts build-essential git`

# build dependencies
apt install `gtk-doc-tools intltool libdbus-glib-1-dev libglib2.0-dev libgtk2.0-dev libexif-dev libmenu-cache-dev  pkg-config valac libglib2.0-doc libgtk-3-doc libgtk-3-dev libasound2-dev libiw-dev libwnck-dev  libcurl4-openssl-dev libxml2-dev libkeybinder-dev libwnck-3-dev libkeybinder-3.0-dev libpolkit-agent-1-dev libvte-2.91-dev openbox-dev`

# getting sources
```shell
mkdir -p /var/build/lxde
cd /var/build/lxde
git clone https://github.com/lxde-gtk3/libfm
git clone https://github.com/lxde-gtk3/pcmanfm
git clone https://github.com/lxde-gtk3/lxpanel
git clone https://github.com/lxde-gtk3/lxsession
git clone https://github.com/lxde-gtk3/lxde-common
git clone https://github.com/lxde-gtk3/lxappearance
git clone https://github.com/lxde-gtk3/lxappearance-obconf
git clone https://github.com/lxde-gtk3/lxlauncher
git clone https://github.com/lxde-gtk3/lxrandr
git clone https://github.com/lxde-gtk3/lxtask
git clone https://github.com/lxde-gtk3/lxterminal
```

# compiling
`debuild -us -uc -b`
