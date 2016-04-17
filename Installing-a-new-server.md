The installation is very similar on Windows and Linux, you simply download a zip file for the intended platform, unzip it,  change directory into the unzipped folder and start csgosl from there. csgosl will then download and install everything needed for your CSGO server.

## To install the server on Windows:

TODO: create gif-anim 

1. Browse to download page at [github](https://github.com/lenosisnickerboa/csgosl/releases) and download the latest csgosl-windows.zip file to the location where you want to install your server.
1. Unzip the downloaded file. A directory `csgosl` is created.
1. Double-click the `csgosl` folder, then double-click `csgosl.vbs`.
1. Click "I understand" button to acknowledge the message dialog about no server being installed.
1. Click "Install Server" button.

All required files will now be downloaded and installed. You can follow the progress in the "Console" page.
Once ready restart the application and click "Start Server" and your up and running!

You may also want to create a shortcut to `csgosl.vbs` and place it on your desktop.

## To install the server on Linux (Ubuntu):

TODO: create gif-anim 

The following two packages are required on Linux, install them like this:
`sudo apt-get install libtk-img lib32gcc1`<br>
(See [Steamcmd information](https://developer.valvesoftware.com/wiki/SteamCMD#Downloading_SteamCMD) for information about lib32gcc1)

`cd <install-location>`<br>
`wget https://github.com/lenosisnickerboa/csgosl/releases/download/v1.0/csgosl-linux.zip -O csgosl.zip`<br>
`unzip -o csgosl.zip`<br>
`cd csgosl`<br>
`./csgosl.sh`<br>

Click "I understand" button to acknowledge the message dialog about no server being installed.<br>
Click "Install Server" button.<br>

All required files will now be downloaded and installed. You can follow the progress in the terminal window from which you started csgosl. Once ready restart the application and click "Start Server" and your up and running!