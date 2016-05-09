NOTE: It is **very** important that you read and understand everything on this page before running sourcemod plugins on your **public** server. When running certain plugins on your **public** server you may end up in trouble with Valve. If the plugin performs actions in violation with Valve server guide lines you may get **BANNED**, or rather your GSLT (Game Server Login Token) will be. Read more [here](https://forums.alliedmods.net/showthread.php?t=279854) and [here](http://blog.counter-strike.net/index.php/server_guidelines/)

I take **NO** responsibility for any problems you may encounter running misbehaving sourcemod plugins on your public server. Having said that, I have tried as much as possible to ensure that this will not happen and I will describe below how it works.

csgosl separates "good" plugins from "bad" as you will see below. Sourcemod implements protection for "bad" plugins. This protection is by default enabled.

So a "good" plugin is a plugin which can be used with sourcemod plugin protection enabled, i.e. it should be ok to run on a lanonly as well as a public server.
A "bad" plugin is a plugin which will only work if sourcemod plugin protection is disabled. This kind of plugin should **NEVER** be used on a public server. But "bad" plugins perform some "good" stuff :) Like weapon skins and knifes... 

By default csgosl is setup so that Sourcemod is only enabled when running a lanonly server. You can enable Sourcemod on public servers by disabling the **lanonly** option. You are still protected by Sourcemod plugin protection and only "good" plugins are allowed to run. 

The first part of the Sourcemod config page handles "good" plugins:

![Sourcemod1](https://raw.githubusercontent.com/wiki/lenosisnickerboa/csgosl/pics/config-page-sourcemod1.jpg)

* **enable** Controls if sourcemod functionality is enabled. This is the manual override switch.
* **onlylocal** If onlylocal is enabled sourcemod will only be enabled if the server is run in lanonly mode. If you start the server in public mode sourcemod will automatically be completely disabled.
* **admins** List all users (separated by space) you want to give sourcemod admin permissions on your server. Users are identified by their steam id (e.g STEAM_1:1:12345678, see [here](https://steamcommunity.com/sharedfiles/filedetails/?id=209000244) for how to obtain this id) or the users ip address (e.g. 192.168.1.123). 

Following these general sourcemod options are options per supported "good" plugin. Currently some of the plugins supplied with the sourcemod package are supported. They are:

* mapchooser
* nominations
* rockthevote
* nextmap
* randomcycle

Read more about them [here](https://wiki.alliedmods.net/Map_Management_Plugins_(SourceMod))

But it's fun to be "bad", right? ...

So here follows some more options further down on the same config page:

![Sourcemod2](https://raw.githubusercontent.com/wiki/lenosisnickerboa/csgosl/pics/config-page-sourcemod2.jpg)

Following some warning text is the option **banprotection**. This option is by default enabled and ensures that all "bad" plugins are always disabled and that Sourcemod protection is enabled.

But... to be able to use the "bad" (but fun) plugins you need to disable banprotection AND perform a "Server Update" to install the "bad" plugins (they are not installed by default to protect you from mistakenly running a public server with these plugin files in the filesystem). Once this is done you can now enable the "bad" plugins and start the server.

When you disable banprotection csgosl will hard code the following settings when starting the server:

* lanonly mode will always be set (+sv_lan 1)
* no GSLT (+sv_setsteamaccount will NOT be set)
* no API auth key (-authkey will NOT be set)

This is to ensure you don't accidentally start a public server with "bad" plugins running.

You can reenable **banprotection** but it will take some manual steps to get all "bad" plugin files off the file system. 

To reenable **banprotection** do the following:

1. Enable the **banprotection** option on the config page.
1. Manually remove the sourcemod installation folder. It is located in the server/csgosl/addons folder where you installed csgosl.
1. Click "Update server" to reinstall sourcemod (but now without the "bad" plugin files since **banprotection** is enabled)

Your're done!



(controlled by FollowCSGOServerGuidelines in core.cfg)
As long as you run your server in **lanonly** mode you should be fine. 
 
FollowCSGOServerGuidelines

Only enable sourcemod plugins on local servers (to avoid potential GSLT Valve ban, read more [here](https://forums.alliedmods.net/showthread.php?t=279854) and [here](http://blog.counter-strike.net/index.php/server_guidelines/).)



Only enable sourcemod plugins on local servers (to avoid potential GSLT Valve ban, read more [here](https://forums.alliedmods.net/showthread.php?t=279854) and [here](http://blog.counter-strike.net/index.php/server_guidelines/).)



<TODO: add supported plugins here...>


How to reenable banprotection
- simple, just tick "banprotection" and disable plugins
- thorough, remove sourcemod...
