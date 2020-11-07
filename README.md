## INTRO: ##
This script is designed to simplify the task of opening up DS4Windows, BakkesMod, and Rocket League seperately.
It will search for the location of DS4, BakkesMod, and Rocket League, and will create an icon with the Rocket League
logo (which replaces your actual Rocket League icon). This will allow all three programs to be opened up at the same
time with one shortcut.




## DISCLAIMER: ##
Be sure to save the "RL Trio Shortcut" folder in a location that will not be deleted. If you do not have DS4Windows,
BakkesMod, and Rocket League installed, do not run this script. You can download each of the additional programs 
here:

* DS4Windows: https://github.com/Jays2Kings/DS4Windows/releases
* BakkesMod: https://bakkesmod.com/download.php

As of now, there are no security precautions to check and see if all of these programs are installed on your system
before running the script.




## SETUP: ##
The follow files should be in your "RL Trio Shortcut" folder:
	- README.txt (this file)
	- RL script.ps1
	- RL.ico

1. Right-click on "RL script.ps1" and click on "Run with PowerShell" (This should take few minutes).

2. Once the script is finished, a Rocket League icon will be on your desktop. Right-click on the icon and click
   "Properties".

3. There should be a fill box labeled "Target:". Add the following to the beginning of the path:
	`powershell.exe -ExecutionPolicy Bypass -File`
   In this case, mine looks like this: 
	`powershell.exe -ExecutionPolicy Bypass -File "C:\Users\Name\Desktop\RL Trio Shortcut\RL script.ps1"`

4. Apply the new changes and you're all set. You should now be able to open up the new Rocket League shortcut and it
   will open up BakkesMod, DS4Windows, and Rocket League. Enjoy!




## NOTE: ##
* Sometimes, Bakke's Mod will need an update and will cause Rocket League to get closed. You should be able to reopen
  the Rocket League shortcut again without a problem.

* If you would like to revert any changes done by this script, you can remove the Rocket League icon. Navigate to 
  your Steam apps (will vary if you changed your install location for Rocket League):
	C:\Program Files (x86)\Steam\steamapps\common\rocketleague\Binaries
  Remove 'Paths.txt', right-click on Rocket League, and click on "Create shortcut". You can then drag this shortcut 
  to your desktop.

* If you have any errors, suggestions, improvements, or any comments, feel free to send me a message through 
  Steam: Johnobomb
  Reddit(Post): Johnobomb
