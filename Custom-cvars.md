First make sure you understand [Advanced mode](Advanced mode). Cvars are added on the advanced tabs and works like other advanced options, i.e. cvars added to the All_modes tab are set in all game modes and cvars added on game mode specific tabs are only set for those modes.

csgosl has support for adding custom cvars to the Advanced tabs. Custom cvars are added using the "New cvar..." button at the top of the tab. Enter the cvar name, the default value and an optional help text which will be displayed as a tooltip.

It is important to set the correct default value, since the cvar will only be added to the configuration file if its value differs from the default value. So if a cvar is by default disabled use default value 0. When you change the value to 1 it will differ from its default and be added to the proper configuration file.

Cvars may be deleted using the delete button right of the cvar.

Often the easiest way to work with custom cvars is to just add them to the All_modes tab and control them from that tab only. 

Note that custom cvar support is pretty basic at the moment. You need to restart csgosl to see the effects of adding or removing cvars. You can add or remove several cvars before you restart csgosl.