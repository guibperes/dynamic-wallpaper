# Dynamic Wallpaper
X11 Dynamic background wallpaper CLI tool, minimal written in Shell Script.
Uses [xwinwrap tool](https://github.com/ujjwal96/xwinwrap) and [mpv](https://mpv.io)

## Install
### Ubuntu
MPV
```sh
sudo apt-get install -y mpv
```

xwinwrap
```sh
sudo apt-get install xorg-dev build-essential libx11-dev x11proto-xext-dev libxrender-dev libxext-dev
git clone https://github.com/ujjwal96/xwinwrap.git
cd xwinwrap
make
sudo make install
make clean
```

dynamic-wallpaper
```sh
git clone https://github.com/guibperes/dynamic-wallpaper
cd dynamic-wallpaper
sudo cp dynamic-wallpaper /usr/local/bin
cp dynamic-wallpaper.desktop ~/.config/autostart
mkdir `xdg-user-dir VIDEOS`/wallpaper
touch `xdg-user-dir VIDEOS`/wallpaper/.wallpaper
```

### Other Linux
Follow [mpv](https://mpv.io/installation) and [xwinwrap](https://github.com/ujjwal96/xwinwrap) installations steps.

dynamic-wallpaper
```sh
git clone https://github.com/guibperes/dynamic-wallpaper
cd dynamic-wallpaper
sudo cp dynamic-wallpaper /usr/local/bin
cp dynamic-wallpaper.desktop ~/.config/autostart
mkdir `xdg-user-dir VIDEOS`/wallpaper
touch `xdg-user-dir VIDEOS`/wallpaper/.wallpaper
```

## Usage
Change wallpaper video file
```sh
dynamic-wallpaper -c <FILE>
```

Restart wallpaper
```sh
dynamic-wallpaper -r
```

Stop wallpaper
```sh
dynamic-wallpaper -S
```

Start wallpaper
```sh
dynamic-wallpaper -s
```
The `.wallpaper` file container the full path of video wallpaper file.
To disable autostart remove `.config/autostart/dynamic-wallpaper.desktop` file.
