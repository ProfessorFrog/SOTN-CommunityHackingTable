# SOTN-CommunityHackingTable
This is a list of SymphonyOfTheNight ISO addresses that can be edited for game modding purposes, and then written to the ISO.
It uses Cheat Engine (cheat engine can apparently write to ISOs), because that makes it easier to share between hackers and build a nice list over time to make the game better.
SOTN modding is slow, and we should work together to make things happen. Contact me on discord if you want to communicate: Frog#9003



==USAGE INSTRUCTIONS==


 IMPORTANT DISCLAIMER;                                                                              
 In this process we use cheat engine in 2 different ways, and most likely you're gonna want to do   
 this in 2 different cheat engine windows.                                                          
                                                                                                   
                                                                                                   
 [A: Find memory values while a game is running]                                                    
 Use cheat engine like you would with any other game to find addresses.                             
 Open cheat engine, click magnifying glass icon (open process), and select your ps1 debug emulator. 
                                                                                                   
                                                                                                   
 [B: Look for your found addresses in the rom/iso file]                                             
 Open Cheat engine, click: "file" -> "open file". Then load up your iso/rom's main file.            
 In the case of .cue+.bin games, you'd load the .bin file.                                          




0) [Make a backup of your game's rom/iso because we're going to be editing the existing one. This process does NOT save a new rom/iso.]



1) [While the game is running, Find the address so we can change a value to edit]
There are various ways to do this:

[a: 	] Use a debugger emulator, like no$psx, Debugger emulators have RAM organized in a way that doesn't randomize. So we can find and 
        calculate addresses consistently.
        These also show the hex memory data while the game is running.
        Use cheat engine's "open process" on the window that the game
        runs in(some emus have 2 windows) and find memory addresses 
        through cheat engine.

[b: 	] Look for gameshark cheats online and convert them to run-time addresses. (UNFINISHED INSTRUCTIONS)

[c: 	] Get addresses from other hackers and add them to the cheat engine list.



2) [Try to edit the value at an address to see what it does.]
If it does something you think might also exist inside the rom/iso , you'll need to find it in the rom/iso. (Some in-memory stuff that exists while the game is running doesn't always exist in the rom/iso)



3) [Finding the address in the rom/iso]
There are various ways to do this;

[A: 	] Find the unique combination of values we found while the game is running in the rom/iso
		     Copy the value you found while running the game, along with the following 10 values.
		     Go into cheat engine, go to "file" and click "open file"; select your game's rom/iso.
		     Set value type to "array of bytes"
		     click "first scan"
		     You should be able to find the values in one scan, if not, try copying more than 10 values, say 14 or whatever. and trying again. If you don't find 
		     anything, try copying less values.
		     Drag the found entry to the bottom section of cheat engine. Once it's there, Set it's "type" by double clicking, and setting it to "byte".
		     You can change the description of the address by double clicking, this is very important to organize your work. I also suggest you put notes about what the 
		     values do in the cheat table. This way we'll have all our information in one place.
                     Save the cheat file by going to "file", and clicking "save as".
		     Careful; if you click "save file" you'll overwrite the rom/iso.


[B: 	] Calculate it using a bunch of information. (UNFINISHED INSTRUCTIONS)
		     You need to calculate the location in the rom/iso using the while running memory address you found. 
		     This is fairly complicated because we need to know the type of address you have at runtime, and what address we need in the iso/rom. (I believe ps1 games 
		     start at 8000 0000, but this is not the case for other systems)




4) [Editing the rom/iso using our address list] 
With the found rom/iso addresses in our cheat engine list, we can now edit some of those values. Double click on 
Go to file, and Click "save file" you'll save the iso.




5) [Playtest]
Open the game in your emulator of choice and see if the changes have worked. If it has. Good on you, romhacker.





6) [Creating a patch.]
Using a program called PPF studio. You can create a patch easily. You load in the original game, load in your hacked game, and it will create a patch from the differences between the 2 game versions.
Now you can "legally" distribute your hack over the internet.





7) [TROUBLESHOOTING]

MY SAVE IS GONE AFTER I GO TO TEST MY HACKED GAME IN MY EMULATOR
In most emulators the name of the savefile for a game should be the same as the name of the game iso/rom. So if you renamed your hacked iso, there's your problem.


HOW DO I KNOW IF AN ADDRESS I FOUND WHILE THE GAME IS RUNNING IS GOING TO BE IN THE ROM/ISO?
uuuh......





8) [GOOD SOTN HACKS]
https://sotn.io/   <- randomizer with a bunch of features. Default settings are good. Output it as a .ppf file and you can patch it over hacked versions of the game.
https://github.com/Lakifume/SotnKindAndFair/releases/tag/1.3.4 <- an all-in-one difficulty hack. Click the "ABOUT" button for instructions. patch it with your sotn.io .ppf file for the best sotn experience you can get right now.
