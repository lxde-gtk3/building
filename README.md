# required packages
apt install `devscripts build-essential git`

# build dependencies
apt install `gtk-doc-tools intltool libdbus-glib-1-dev libglib2.0-dev libgtk2.0-dev libexif-dev libmenu-cache-dev  pkg-config valac libglib2.0-doc libgtk-3-doc libgtk-3-dev`

# getting sources
```shell
mkdir -p /var/build/lxde
cd /var/build/lxde
git clone https://github.com/lxde-gtk3/libfm
git clone https://github.com/lxde-gtk3/pcmanfm
```

# building order
libfm -> pcmanfm 

# compiling
`debuild -us -uc -b`
