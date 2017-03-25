![Run](https://raw.githubusercontent.com/wiki/lenosisnickerboa/csgosl/pics/config-page-server1.jpg)

* **name** The name of your server, shown in the CSGO server browser list. 
* **password** Protect your server with a password. Must be entered to connect to your server.
* **tags** Your servers tags, enter them as a comma separated list. Can be searched for in the csgo server browser. Example: 128fps,admins
* **port** The port your server is listening to. See [Host public server](Host public server)
* **lanonly** Your server will only be reachable from your LAN (Local Area Network).
* **rcon** If enabled enables the remote server console used to control the server at run time.
* **rconpassword** Protect your rcon connection with a password. Must be entered to be able to control your server.
* **updateserveronstart** Performs a csgo server update when csgosl is started.
* **restartserveronstart** Restarts your csgo server when csgosl is started. Server is started if not running.
* **restartserverat** Restarts your csgo server at certain points in time. Enter times as a space separated list of 24h times, e.g. 05:00 11:00 17:00 23:00.
* **updateserveronrestart** Performs a csgo server update when csgosl is restarted.

![Run](https://raw.githubusercontent.com/wiki/lenosisnickerboa/csgosl/pics/config-page-server2.jpg)
* **bindip** IP address which your server should bind to.Leave blank if you don't have a problem with connecting to the server. May e.g. be used when running on a VLAN to force the server to bind to the VLAN.
* **autorestart** If enabled automatically restarts your server if it crashes.
* **tickrate** Sets the tickrate used for communication between your game client and the server. Will request all connecting game clients to use the stated tickrate.
* **netmaxfilesize** Affects how large files (maps) can be downloaded from your server. 64 (MB) is the maximum value. This is only valid for user installed non-workshop maps.
