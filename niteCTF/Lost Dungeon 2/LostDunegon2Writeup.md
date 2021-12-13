# Lost Dungeon - 2

Welcome Adventurer! There is a portal that teleports you to other levels but unfortunately only wizards can use it. Can you figure out how to make the portal work and get to the hidden level "level0"? 



## Getting started

A unity game is provided to us. We can use **dnSpy** to decompile and modify the code for this challenge. On opening the game, we see that there is a portal and a wizard npc next to it who says the portal can be used only by wizards.
## Getting the portal to work

Let us open **Assembly-CSharp.dll** using **dnSpy** from the folder Game_data>Managed. On going through the scripts we find the script **Portal**.  Here lets change the if statement to allow **Player** instead of wizard. 
![Speed Modify](https://dl.dropboxusercontent.com/s/50rldo88giapwu5/Screenshot%202021-10-20%20183858.png?dl=0)
Now we can get to two random levels but those are not the ones we are looking for. From the description of the challenge we know we need to get to level0. So lets change the code to send us to level0.
![Dungeon](https://dl.dropboxusercontent.com/s/3cti2otmqbjq246/1.png?dl=0)
Now we have reached the hidden level and see a bunch of npcs. On talking to them they ask us to respawn somehow.
![Dungeon](https://dl.dropboxusercontent.com/s/4war1gcl3gsdndx/3.png?dl=0)
Hence we understand we have to do something to be able to respawn in this map.

## Respawning
Let us go through the code and try to find something related to respawning. On the GameManager Script we see a function to respawn. Hence we have to call this function when we spawn on that map.
![fix](https://dl.dropboxusercontent.com/s/qt001t3t4yr36xo/4.png?dl=0)

On analysing the code we find that **n()** is the load state function and it takes you to the spawn point once the scene is loaded. So we have to add a if function there and call the respawn function here. We know that the scene name is level0 from the description. 

![Flag](https://dl.dropboxusercontent.com/s/q4jw2s0drp0v2b9/6.png?dl=0)

Now we have reached the location with the flag and on moving to the right we find the flag.

![Flag](https://dl.dropboxusercontent.com/s/bvzknjh0wxami8r/flag.png?dl=0)
***Flag: nite{L3veL_100_Maf1a_b055}***