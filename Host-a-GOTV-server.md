This is coming in the next csgosl release, working on it...

# Background
Read about [GOTV](https://steamcommunity.com/sharedfiles/filedetails/?id=411316022).

# Configure
Setup your GOTV server in the csgosl GOTV tab. Most relevant options can be controlled from this page.

# Public servers
If your server should be possible to spectate from outside your LAN you need to forward the GOTV port (default 27020) in your router to the IP address of your csgo server. See more about port forwarding on the [[Host public server]] page. For LAN only servers you don't need port forwarding.

# Spectating the server (LAN only)
To spectate the server enter:

`connect <server-ip-address>:<gotv-port>`

Example:

`connect 192.168.1.100:27020`

If you set a password for your server use:

`connect <server-ip-address>:<gotv-port>; password <your-password>`

Example:

`connect 192.168.1.100:27020; password 123`

# Spectating the server (Public)

To allow persons to connect to your GOTV server from outside your LAN you need to give them your external IP address which you e.g. can get from [whatismyip](https://www.whatismyip.com/). Assuming you have properly forwarded the GOTV port in your router your friends should be be able to connect as described above using your external IP address.

# Record a GOTV demo

To start a recording:

`tv_record "mydemo1"`

To stop recording:

`tv_stop`

To play demo:

`playdemo mydemo1`

Demos are stored in Steam\SteamApps\common\Counter-Strike Global Offensive\csgo