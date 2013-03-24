MC-mining-turtle
================

MC-mining-turtle can automate mining with your favorite turtle.

1. Global fonctionnement

[TODO]

2. Perquisit

Theses scripts works with the following version of minecraft and mods :
* Minecraft
* Computer Craft XXX

3. Setup

What you need is :
- 1 wirless mining turtle
- 2 chests
- Some torchs
- Some lava cells
- 1 bloc of each : cobblestone, gravel, sand, dirt
- Optional : 1 extra computer with 1 modem attached on the side

Setup Plan


     ^							- Place an empty chest in A.
     | Direction of mining		- Place a chest in B. Put some lava cells in it.
     |							- Place the wireless turtle in T.
+-+ +-+							- Check turtle orientation. It need to face the good
|A| |T|							  direction as shown in the image.
+-+ +-+							- Open turtle inventory. Place some lava cells
    +-+							  in slot 1 & 2. Leave it empty if you dont have
    |B|							  enough of it.
    +-+							- Place some torch in slot 3
								- Place one bloc of cobblestone in slot 4, one 
sand in bloc 5, on gravel un bloc 6 and one dirt in bloc 7.
- Connect to the turtle and type "dig".	

4. Rednet usage

A diging turtle broadcast lots of messages on Rednet. You can listen it with
ananother computeur. Simply place your computer not too far from the working
turtle (remember, rednet has a 64 bloks reach). 

Run the "search" program, it will list all turtle broadcasting near you. It will
also show the turtle ID. You will need it to listen all messages from a turtle.

Now run the "listen" program, it will ask for a turtle ID. Type the ID en hit 
return, all message will now prompt on your computer screen.

If your turtle goes to far from your computer ( 64 bloks again !), you will stop 
receiving messages. Theses messages are lost but don't worry the connection is 
not completely lost, you will again messages if the turtle return near your 
computer.

For disabling the broadcast, edit the "dig" program. Set the local variable "broadcast" 
to false : 
> local broadcast = false

5. Debug mod

For enabling debug message, edit the "dig" program. Set the local variable "debug"
 to "true" : 
> local debug = true

6. Other stuff

All files contained in this archive are licensed as stated in the LICENSE file.

If you find any bugs please feel free and send an e-mail to sebastien.braun@troll-idees.com

Future versions of this code can be downloaded from: 
https://github.com/sbraun/mc-mining-turtle

Thanks for taking the time to download this code. If you have any questions
please feel free to contact me.


- Sebastien Braun <sebastien.braun@troll-idees.com> 2013
