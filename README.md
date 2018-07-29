# NetHack-Realm

NetHack-Realm is your classic fun, loving, and unforgiving, NetHack(Rouge) with a twist. We dont like to through around the term `AI` but... Do humans count as `AI`? Cause thats who your fighting. Yep its you vs XXXX other bots, *cough*, "players" :). Till there is only one of you left standing. Dont worry there will be lot scattered around randomly, so break out the old shrine to RNGsus and hope you find something good. Sounds ok right? Well there is more!!! 
A good friend once told me "Save-states, saves lives", so you know what that means? The contracts `SAVE_STATE` function allows you to do just that! For a small fee you can pay the contract to pause your game for you, cost based on amount of data being saved and length of time. End goal would be that we implement all of NetHack's classes and items. Things that need to be figured out:

* Function async request handling?

	* User would push to the chain the list of commands they are executing for a given moveSet. Can we execute that in one request to the contract? Or multiple? Move input would be network time dependent. 

* Game Limits
	
	* Amount of blocks that game will wait for your move to be input when in battle queue. 

	* After each round that you play in and live you have the option to pause for free. 

	* Each time you battle you put up a small network fee for your moves that game. 

		* Fee should be able to be calcuated based on the number of items generated and circle close time.
	
	* If you die in the storm you die in the game.

	* There is the ability to move `ITEMS` to a `BANK` aka the contract and it will allow you to interact with it and withdraw only the items you give it.

		* Might add ability for a bank heist of sorts help with garbage collection of failure accounts?
	
	* All actions in game are RNG based


* Map generation:

	* How big?

	* X:Y based? X:Y:Z based?

* Item generation:

	* How do we allow for inspecting items in area?

	* How do we generate random items?
