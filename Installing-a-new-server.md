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

## To install on Linux (Ubuntu, Minth, Manjaro):

You may watch the clip above showing the Windows installation. The Linux installation does the same thing using the command line.

The following packages are required on Ubuntu/Minth, install them like this:<br>
`sudo apt install tcl libtk-img lib32gcc1 lib32stdc++6 net-tools`<br>
(See [Steamcmd information](https://developer.valvesoftware.com/wiki/SteamCMD#Downloading_SteamCMD) for information about lib32gcc1)
Note: net-tools needed for ifconfig which is used by Steam.


The following packages are required on Manjaro, install them like this:<br>
`sudo pacman -Syu pamac`<br>
`sudo pamac install tcl`<br>
`sudo pamac build tkimg net-tools-debian-ifconfig`<br>
Note: Lazy use of pamac, could of course be done using pacman only but pamac takes care of the tkimg building stuff which I don't want to bother with.
Note: net-tools-debian-ifconfig needed for ifconfig which is used by Steam.

`cd <install-location>`<br>
`wget https://github.com/lenosisnickerboa/csgosl/releases/download/v2.7.1/csgosl-linux.zip -O csgosl-linux.zip`<br>
`unzip -o csgosl-linux.zip`<br>
`cd csgosl`<br>
`./csgosl.sh`<br>

Click "I understand" button to acknowledge the message dialog about no server being installed.<br>
Click "Install Server" button.<br>

All required files will now be downloaded and installed. You can follow the progress in the terminal window from which you started csgosl. Once ready restart the application and click "Start Server" and your up and running!

## Install using an existing csgo server installation:
If the existing installation is a csgosl installation you can simply copy the entire folder to have a new installation.

If the existing installation is a non csgosl installation, i.e. a standard csgo server installation, use the procedure below.

This procedure can be used when you already have an up-to-date server installation and want to avoid having to download the csgo server files again. Please be aware that you will loose some of the settings which are controlled by csgosl since csgosl will use its own internal configuration files.

The same procedure is valid for both windows and linux. Just follow the above instructions for your operating system but **BEFORE ** you start csgosl for the first time do this:

1. In the folder where you extracted csgosl-xxx.zip (the one containing the executable csgosl.vbs or csgosl.sh file and a bin and mods directory) create two more directories named "server" and "steamcmd" (without the quotes, see pic below).
1. Copy all files from your existing steamcmd folder into the steamcmd folder you just created.
1. Copy all files from your existing server folder into the "server" folder you just created.
1. Start csgosl (as described above). You will not see the dialog box about no server being installed. 
1. Click "Update Server" button to allow csgosl setup everything. If your original server was up-to-date no files will be downloaded, else a normal update will be performed.
1. Done!

![Install-from-existing](https://raw.githubusercontent.com/wiki/lenosisnickerboa/csgosl/pics/installing-a-new-server-from-existing-server.jpg)

The initial CSGO installation requires ~15GB so make sure you select a location with enough free storage. 

The installation folder may be copied or moved (renamed), the root folder name is not relevant. This can be used to create new installations, solve out-of-space issues, ...