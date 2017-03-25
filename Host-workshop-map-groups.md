Hosting workshop map groups are just as simple as hosting a workshop map. You need the API authorization key as described in [Host workshop maps](https://github.com/lenosisnickerboa/csgosl/wiki/Host-workshop-maps). 

Then go to [CSGO workshop map groups](https://steamcommunity.com/workshop/browse/?section=collections&appid=730) (they are also called collections).

Select a map group, e.g. [Best DM collection](http://steamcommunity.com/sharedfiles/filedetails/?id=538085065)

Please note the number next to the "id=..." part in the browser address field. Copy and paste this number (538085065 in this example) into the **mapgroup** setting on the Run tab and start the server. That's it! The server will download the maps from the workshop and your connecting friends will automatically download the maps from the workshop when they connect to your server.

The maps will from now on show up under the Maps tab and they will also be selectable when you create your own map groups. Also note, once the server has downloaded the maps you don't need to host them using the collection id number any more, your friends will still be automatically download the maps from the workshop.

**You currently need to restart csgosl to see the map in the maps list. This will be fixed.**