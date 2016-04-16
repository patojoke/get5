Development is performed on linux. I currently run Ubuntu 14.04 but you should be alright with most mainstream distros. 

First clone the repo:

`git clone https://github.com/lenosisnickerboa/csgosl.git`

Then build everything (see below for building for separate platforms):

`cd csgosl`
`make install`
`make`

This will download all required components, build windows and linux archives in out/windows/csgosl.zip and out/linux/csgosl.zip.

When the above steps have been performed you can buidl the different targets separately, e.g. `make windows` or `make linux`.

