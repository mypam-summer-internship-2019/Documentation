INTEGRATING THE UDP_HANDLER.

Download the latest "Game Dev Package".
Unzip into an appropriate folder outside of your game's main folder.
Copy the 'JSonDotNet' folder into the assets folder of the project - this can go into sub folders such as an "Imports" folder for any imported packages.
Copy the 'UDP_Handler.cs' file into the assets folder of your game.
Create an empty object into the very first scene to be loaded and attach the UDP_Handler script to it.

This gameobject can be copied into every scene, but it will work fine so long as it is in the very first scene that loads when the game is run.
Adding it to every scene allows it to work if you are testing scenes without loading the first scene.

Unless making a fundamental change, do not edit the 'UDP_Handler' script. Create new scripts and access variables 
e.g. set a variable to the value of X2pos by using 'double xInput = UDP_Handler.X2pos'

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

BUILDING THE GAME

Ensure networking settings are set to 'Net.4.x' in the Unity Editor.
This setting is found under File > Build Settings > Player Settings > Settings for PC... > Other Settings > Configuration > Api Compatibility Level > Select .NET 4.x

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

RUNNING THE BUILD

Ensure Unity Editor is closed when trying to run a build.
Ensure the latest version of 'UDP_Handler' and 'Virtual Controller' is in use.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

MONKEY BRIDGE

Ensure the 'Local Files' folder is copied into the "GameData" folder after building.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
