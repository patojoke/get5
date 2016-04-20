![Run](https://raw.githubusercontent.com/wiki/lenosisnickerboa/csgosl/pics/config-page-run.jpg)

* **gamemodetype** Select the game mode and type
* **mapgroup** Select map group. You can either select one of the map groups you have created using the [map groups editor](Help on Map groups) or a workshop map group as described [here](Host workshop map groups).
* **startmap** Selects the first map the server will host. The map can be any of your installed maps or a workshop map as described [here](Host workshop maps).
* **players** Sets total number of players on the server, players per team will be this number divided by two.
* **fillwithbots** If enabled bots will be automatically added to ensure the number of players on the server are always **players**. When new human players connect bots will be automatically kicked. If disabled no bots are added to compensate for missing human players.
* **botskill** Bot skill level. 
* **friendlyfire** If enabled team members can hurt each other.
* **immediaterestart** No warmup time, the game starts immediately.
* **killcam** If enabled shows who killed you and that players location on the map.
* **roundtime** Maximum time to play each round. If the game has not ended after this time it is ended.
* **options** custom srcds command line options. Anything entered here is appended to the command line when the server is started. Have a look [here](https://developer.valvesoftware.com/wiki/Command_Line_Options#Source_Dedicated_Server) for available options.