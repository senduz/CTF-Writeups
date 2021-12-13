# Lost Dungeon

Welcome Adventurer! Legend has it that there lies a dungeon filled with powerful beasts which can be tamed to reveal a secret message. The path to the dungeon is long and arduous. No one who has found the dungeon has returned back as once the beasts get to you they never leave. Can you reach the dungeon and tame the beasts?



## Getting started

A unity game is provided to us. We can use **dnSpy** to decompile and modify the code for this challenge. On opening the game, we see that we are in a room and see a path leading out. There are two NPCs in the room so let us talk to them.

![NPC1](https://dl.dropboxusercontent.com/s/1ek41reuon76bz1/Screenshot%202021-10-01%20181752.png?dl=0)

![NPC2](https://dl.dropboxusercontent.com/s/o49nw8zll6ozojk/oldman.png?dl=0)

Next, on trying to leave the room through the path we see that the path is too long.
## Changing the speed to get there faster

Let us open **Assembly-CSharp.dll** using **dnSpy** from the folder Game_data>Managed. On going through the scripts we find the script **Mover** which is used to move the player. Here we can see that **bn** and **bo** are the speed multipliers, hence we are going to modify it and give it a high value.
![Speed Modify](https://dl.dropboxusercontent.com/s/p4h42vxs7vum8bl/Screenshot%202021-10-02%20002328.png?dl=0)

Now we can travel superfast and reach the dungeon very fast.
However on reaching the dungeon, we see that we are surrounded by mobs.
![Dungeon](https://dl.dropboxusercontent.com/s/r1el3smguerq6ku/dungeon.png?dl=0)
## Stoping the mobs from moving
From talking to the oldman NPC, we can understand that the mobs are arranged as the flag and we have to stop them from moving and surrounding you. 
Let us now check the **Enemy** script. We see a FixedUpdate function that makes the mobs chase you. So lets modify the script and remove the contents of the function.
![fix](https://dl.dropboxusercontent.com/s/iwqzc4sh5gcmgxm/fix.png?dl=0)

On doing this, we can see that the mobs are arranged as the flag.

![Flag](https://dl.dropboxusercontent.com/s/oy8cimrv3w3v0ep/flag0.png?dl=0)

***Flag: nite{Eb1c_9aM3R}***
