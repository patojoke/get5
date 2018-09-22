To host a workshop map you need an **API autorization key** which is issued by Valve on Steam. Just head over to the [Steam Registration page](http://steamcommunity.com/dev/apikey) and generate a key. Copy and paste this key into the **apiauthkey** setting on the Steam tab. 

NOTE: If you don't have a domain name it seems it's ok to enter e.g. your servers IP address or your PCs hostname. See e.g. [here](http://steamcommunity.com/app/4000/discussions/1/558752450986071551/) or [here](https://github.com/Jessecar96/SteamBot/issues/158).

Now you're ready to host your own maps (and map groups).

To select a new workshop map go here: [CSGO workshop maps](http://steamcommunity.com/workshop/browse?appid=730)

Select a map, e.g. [Tides - Wingman](https://steamcommunity.com/sharedfiles/filedetails/?id=1508934767&searchtext=)

Please note the number next to the "id=..." part in the browser address field. Copy and paste this number (1508934767 in this example) into the **startmap** setting on the Run tab and start the server. That's it! The server will download the map from the workshop and your connecting friends will automatically download the map from the workshop when they later connect to your server. 

The map will from now on show up under the Maps tab and it will also be selectable when you create your own map groups. Also note, once the server has downloaded the map you don't need to host it using the id number any more, your friends will still be automatically download the map from the workshop.

If you host a buggy workshop map which causes the server or connecting clients to crash remove the map folder from /server/csgo/maps/workshop/ and restart csgosl.

 **You currently need to restart csgosl to see the map in the maps list. This will be fixed.**
