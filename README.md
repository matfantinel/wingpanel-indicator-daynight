<h1 align="center">wingpanel-indicator-daynight</h1>

<p align="center">A wingpanel indicator to toggle 'prefer dark variant' option in elementary OS.</p>

<p align="center"><img src="https://raw.githubusercontent.com/maze-n/wingpanel-indicator-daynight/master/screenshots/screenshot-1.png" width="350">
</p>

## Build & Run

```bash
# install elementary-sdk, meson and libwingpanel
sudo apt install elementary-sdk meson libwingpanel-2.0-dev
#install dependencies
sudo apt install libglib2.0-dev libgranite-dev libxml2-dev
# clone repository
git clone https://github.com/matfantinel/wingpanel-indicator-daynight.git wingpanel-indicator-daynight
# cd to dir
cd wingpanel-indicator-daynight
# run meson
meson build --prefix=/usr
# cd to build, build and test
cd build
sudo ninja install
# restart switchboard to load your indicator
pkill wingpanel -9
```

## Uninstall

```bash
cd build
sudo ninja uninstall
```
