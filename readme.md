+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
										
										Napf bank markers for Zupa's gold coin script
										
										Credit to Zupa for the originl map marks file
												
												http://devzupa.be/#/dayz/sc999
												
												Credit to Nexus for the banks
										
										http://opendayz.net/members/pwn3d-nexus.18419/

+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++


														INSTALLATION 

														Server.PBO

Step one: Put the "napfbanks" folder in the your server.pbo root 

Step two: In your server_functions.sqf, add 

// Nexus's Npaf Banks
execVM "\z\addons\dayz_server\napfbanks\napfbanks.sqf";

Directly under 

server_maintainArea = 			compile preprocessFileLineNumbers "\z\addons\dayz_server\compile\server_maintainArea.sqf";



														Mission.PBO

Step one: If you don't already have acustom variables.sqf the get it from @Dayz_Epoch\addons\dayz_code\init\variables.sqf

Step two: Make a folder called "compiles" in your mission root.

Step three: Put your Variables.sqf in that folder. 

Step four: In your init.sqf Add 

call compile preprocessFileLineNumbers "Compiles\variables.sqf";				//Initilize the Variables (IMPORTANT: Must happen very early)

in place of 

call compile preprocessFileLineNumbers "\z\addons\dayz_code\init\variables.sqf";				//Initilize the Variables (IMPORTANT: Must happen very early)

Now you have a custom variables.sqf. 

Step five: Open your variables.sqf and add 

DZE_ATM = ["Laptop_EP1","MAP_Table"]; // objects where u can bank, add them here if u want extra's.

below 

disableSerialization;

Step six: At the bottom of your init.sqf add 

execVM "napfbankmarkers\addbankmarkers.sqf";

Step seven: Put the "napfbankmarkers" folder in the root of your mission file. 

That's it, repack your .pbo's and you should be all good. 


+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

										Credit to Zupa for the originl map marks file
												
												http://devzupa.be/#/dayz/sc999
												
												Credit to Nexus for the banks
										
										http://opendayz.net/members/pwn3d-nexus.18419/

+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++