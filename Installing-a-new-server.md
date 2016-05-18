You first need to download and install the csgosl application. The installation is very similar on Windows and Linux, you simply download an application zip file for the intended platform, store it where you want your server to be installed, unzip it,  change directory into the unzipped folder and start csgosl from there. csgosl will then download and install everything needed for your CSGO server into this folder.

## To install on Windows:

Watch installation [clip](https://raw.githubusercontent.com/wiki/lenosisnickerboa/csgosl/pics/install-windows.gif) showing the complete installation + first server start. 

1. Browse to download page at [github](https://github.com/lenosisnickerboa/csgosl/releases) and download the latest csgosl-windows.zip file to the location where you want to install your server.
1. Unzip the downloaded file. A directory `csgosl-windows` is created. 
1. Double-click the `csgosl-windows` folder, then double-click `csgosl.vbs`.
1. Click "I understand" button to acknowledge the message dialog about no server being installed.
1. Click "Install Server" button.

All required files will now be downloaded and installed. You can follow the progress in the "Console" page.
Once ready restart the application and click "Start Server" and your up and running!

At this point you may get a question from Windows firewall where you need to allow CSGO full network access. If you run some other firewall you will need to do the same in that firewall instead.

You may also want to create a shortcut to `csgosl.vbs` and place it on your desktop.

## To install on Linux (Ubuntu):

You may watch the clip above showing the Windows installation. The Linux installation does the same thing using the command line.

The following two packages are required on Linux, install them like this:
`sudo apt-get install libtk-img lib32gcc1`<br>
(See [Steamcmd information](https://developer.valvesoftware.com/wiki/SteamCMD#Downloading_SteamCMD) for information about lib32gcc1)

`cd <install-location>`<br>
`wget https://github.com/lenosisnickerboa/csgosl/releases/download/v1.1.1/csgosl-linux.zip -O csgosl-linux.zip`<br>
`unzip -o csgosl-linux.zip`<br>
`cd csgosl`<br>
`./csgosl.sh`<br>

Click "I understand" button to acknowledge the message dialog about no server being installed.<br>
Click "Install Server" button.<br>

All required files will now be downloaded and installed. You can follow the progress in the terminal window from which you started csgosl. Once ready restart the application and click "Start Server" and your up and running!

The initial CSGO installation requires ~15GB so make sure you select a location with enough free storage. 

The installation folder may be moved around (e.g. if you run out of storage) and may also be renamed. 