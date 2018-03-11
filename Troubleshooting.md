1. If you have problems starting your server make sure you don't have spaces in the folder name where you installed csgosl. csgosl doesn't properly handle spaces.
1. Linux only: If your server crashes on startup with the following message on the console:<br>
`Failed to open dedicated.so (libstdc++.so.6: cannot open shared object file: No such file or directory)`
`Add "-debug" to the server/srcds_run command line to generate a debug.log to help with solving this problem`<br>
Simply issue this command:<br>
`sudo apt-get install lib32stdc++6`