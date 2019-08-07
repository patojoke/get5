Development is performed on linux. You should be all right with most mainstream distros.

Ubuntu/Minth:

First make sure some basic tools are installed:

`sudo apt install git make`

Manjaro:

`sudo pacman -Syu zip unzip`

Rest is distro independent.

Clone the repo:

`git clone https://github.com/lenosisnickerboa/csgosl.git`

Then build everything (see below for building for separate platforms):

`cd csgosl`<br>
`. env.sh`<br>
`make install`<br>
`make`<br>

This will download all required components, build windows and linux archives in out/windows/csgosl-windows.zip and out/linux/csgosl-linux.zip.

When the above steps have been performed you can build the different targets separately, e.g. `make windows` or `make linux`.


