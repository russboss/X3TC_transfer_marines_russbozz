Basic Instructions for all who have never used a script before
transfer marines
adds the ability to transfer marines from a TP to any other ship (under Piracy Menu)


Q: how is transfer Marines useful?
A: alright for starters I'll give you a situation.
Imagine an M6 doing a boarding operation on some ship, b/c your ship is an M6 there is a limit of 5 marines at a time but you have a TP full of Marines a sector over..
use Transfer marines
The TP will fly to your approximate location and using it's required teleporter transfer the spare marines to you when you have space. When it is empty it'll follow its secondary command that you gave it when you started the command. The secondary command can be any of the following: follow the original target ship, follow another ship, dock to homebase, dock at station or fly to position.

The good thing is you can make chains of TPs in this manner transfering marines to the next in line all the way to you...

Q: what if one ship in a string is destroyed?
A: as long as only one ship is destroyed at a time the chain will fill the gap in a short time (within 5 seconds).

1---2---3 if ship 1 is the head of the line and ship 2 is destroyed 

1---3 ship 3 will start transfers to ship 1 automatically

For the programmers:
Each ship running this command has a local variable named “ship.transfer.marines” that holds the target. A local variable is accessible from other scripts anywhere in the game, providing that there is a reference to the ship that the local variable is attached.
When a target is chosen, the ship will fly within transporter range and proceed to fill the target. When the target is full the ship will wait (~5 seconds) and check to see if the ship is full. When the ship is empty it will fly to the secondary objective.

In the event of a ship lost in the chain, the script has already stored its target when the script had started. All that occurs, is the ship will notice the missing ship and then reset the value of its target, and update the local variable so other ships down the list reset as well.




INSTALL:
drop files into corresponding folders

scripts folder:

setup.russbozz.transfer.marine
plugin.russbozz.transfer.marine

t folder:

9314-L044.xml





The Dry Stuff:

As for EULA:
Ha! a What!? use et as you wish, if you can build one better off of my code or had a few tweaks for better performance go right ahead do it.  Use it in whatever you want.

Give credit where credit is due
~Yup don't care if you list my name on something or not; just don't blatantly claim it as your own.

-Russbozz
