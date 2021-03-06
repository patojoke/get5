![Advanced](https://raw.githubusercontent.com/wiki/lenosisnickerboa/csgosl/pics/config-page-advanced-mode.jpg)

See [Custom cvars](https://github.com/lenosisnickerboa/csgosl/wiki/Custom-cvars) for more help on the "New cvar..." button.

To enable the advanced pages you need to enable the **fullconfig** option in the [[Help on Application]] Application configuration page and restart csgosl. Once this is done you get a number of new configuration pages containing a lot of options controlling most aspects of your server. 

Theres one tab named "All_modes" and then a tab per game mode. The tab per game mode controls options for that particular game mode and the tab All_modes (yes, you guessed it...) controls options for all game modes, i.e. what you set here overrides that setting in all game modes. This can be convenient when you don't want game mode specific options.

Starting from csgosl version 1.2 not all cvars are displayed in the GUI, only the ones present in the gamemode specific config files provided by Valve. The reason for this is the GUI got really sluggish when all options where present and also the relevant ones disappeared among all other options. You can still add cvars Valve didn't add to their default gamemode config files by adding that option to the gamemode__server.cfg file. The option added here will be retained during csgo and csgosl updates.