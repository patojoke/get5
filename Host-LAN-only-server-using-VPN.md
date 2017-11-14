*** UNDER CONSTRUCTION - NOT FULLY WORKING AND UNRELIABLE ***

Update: The below never worked reliably for me. I ended up just setting up a VPN using my ASUS router. I selected an IP range in the LAN IP range and invited external players to connect to my VPN. Worked like a charm. Keeping the below text for potential future updates.

This description will show you how to setup a LAN only server over VPN allowing friends to connect to your server across the Internet. I will be using Hamachi for setting up the VPN.

A VPN (Virtual Private Network) is just a way to setup an private network across the Internet. This way you and you friends can connect in the same way you would if you were all connected to the same physical network (in the same building).

The advantage with running a LAN only server is that you are allowed to run more sourcemod plugins which would get you banned if run on a public server.

Please note at this point this description is not fully tested. I have only set it up on my LAN using a csgosl operated server running windows. I will test this further and update this page accordingly. At this point my theory is it should work the same way across the Internet. Please report if this works or not for you.

First you need to download and install the Hamachi software on the machine where you want to run the server. Hamachi is free and can be downloaded from [here](http://vpn.net/). 

Start Hamachi, register an account and select to create a "New client owned network". Select a descriptive "Network ID:" (e.g. NisseNet) and a password. If the network is not started automatically right-click it and select "Go online". You should now see the connected network with its IP address (something like 12.34.56.78 / 1234:12::4321:1234).

Now start csgosl (on the same machine), head over to the Server config page and enable **lanonly** and enter the IP address from above in the **bindip** field. Now start your server and it should be up and running on your newly created VLAN.

I did notice repeated error messages in the server console window:

`CreateBoundSocket: ::bind returned error [no name available](10049)`

I ignored them, it seems to work anyhow.

Now install Hamachi on the machine(s) you want to connect from, your friends will of course have to do the same. They will also need to register new accounts if not already registered.

Now select "Join an existing network" and select the name of the network you created above (NisseNet). 

Start CSGO, select "Browse Community Servers". Select the LAN tab and your server should be present. Connect and you're done!

To verify that you really are connecting using the VPN open the console window in CSGO (key ~ by default) and type `status` and hit ENTER. You should now see (a couple of lines down) a line starting with "udp/ip:" and the IP adress of your server (the one you entered in the **bindip** field in csgosl, 12.34.56.78 in the example).

