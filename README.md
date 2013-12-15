RPG1
====

A compilation of code that can be used to make RPGs in javascript.

====

Player object:

The player object has health, an inventory, effects, and armor/weapon slots.

The player can equip items with the .equip(i) function.

The player can cast spells that will be created outside of the player variable

====

Item object:

Items can be equipped by the player and the items that were equipped before will be placed in the inventory.

Items have effects that give values to the player and are sent via address using Object["address"].

Items have an onUse function, so that you can have the item do things when you use it.

Items have an onEquip function, so that it will do something when it's equipped.

Items have two values, can be used for the high and low damage of a weapon, but generally, value1 is used for the main value, such as armor.

Objective items are items related to an objective, will be given when objective begins, and will be removed when it is cancelled or returned.

====

Spell object:

When cast, a spell will execute a customizable function that will do anything you want it to do, using one variable. The variable used is the player, so that you can use the player's target and deal damage to it or what ever you want.

====

Effect object:

Effect objects have two parts: address and value. Effects belong to a player or entity, so the effects will affect only its owner.

