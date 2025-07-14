# wps2019linuxbont



sudo apt-get update
sudo apt-get install build-essential meson ninja-build wget
wget https://sourceforge.net/projects/freetype/files/freetype2/2.13.0/freetype-2.13.0.tar.xz
tar xvf freetype-2.13.0.tar.xz
meson setup freetype-2.13.0 build
meson compile -C build
sudo cp -a build/libfreetype.so* /opt/kingsoft/wps-office/office6/
(确认wps路径ls /opt/kingsoft/)
