This is coming in the next csgosl release, working on it...

# Background
Read more about GOTV [GOTV](https://steamcommunity.com/sharedfiles/filedetails/?id=411316022).

# Configure
Setup your GOTV server in the csgosl GOTV tab. Most relevant options can be controlled from this page.

# Public servers
If your server should be possible to spectate from outside your LAN you need to forward the GOTV port (default 27020) in your router to the IP address of your csgo server. See more about port forwarding on the [[Host public server]] page. For LAN only servers you don't need port forwarding.

# Spectating the server
To spectate the server enter:

`connect <server-ip-address>:<gotv-port>`

Example:

`connect 192.168.1.100:27020`

If you set a password for your server use:

`connect <server-ip-address>:<gotv-port>; password <your-password>`

Example:

`connect 192.168.1.100:27020; password 123`

# Record a GOTV demo

To start a recording:

`tv_record "mydemo1"`

To stop recording:

`tv_stop`

Demos are stored in Steam\SteamApps\common\Counter-Strike Global Offensive\csgo