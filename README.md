# Forge Lag Fixer
This is intended as a Server Only mod.  It does not need to, and should not, be installed on client side.

Forge Lag Fixer is a lag reduction utility.  It will automatically scan for entities and dropped items at configurable intervals, and remove them from the world, unless they're blacklisted.  Additionally, Forge Lag Fixer can unload chunks when TPS drops below a configurable level. (Although you cannot set it higher than 15 TPS).  Forge Lag Fixer is also capable of preventing overbreeding. Players can work around the protection, of course, but it will still help.
 
## Configuration
All configuration can be handled in game through the /bgon command, and it's sub commands.  /bgon is only available to ops.  

## Commands:

* /bgon toggleitem - Places the item you have selected on your hotbar into the item Blacklist, preventing it from being removed during Clears.
* /bgon toggleentity <name> - Places the named entity into the Entity blacklist, preventing it from being removed during Clears.  This would be the displayed name of the entity, so "Skeleton" would cover skeletons, but not "Wither Skeleton".  Use the names displayed by /bgon scanentities for best results.
* /bgon clear - Manually runs a Clear, removing items and entities from the world.
* /bgon interval <time> - Sets the time between automatic Clears.  The interval is actually 1 minute longer, as it includes a 1 minute warning.
* /bgon toggleauto - Turns automatic clearing on and off.
* /bgon listitems - Lists the contents of the item blacklist.
* /bgon listentities - Lists the contents of the entity blacklist
* /bgon settps <tps> - Sets the TPS below which chunks will be unloaded automatically.  Cannot be set higher than 15 in game.  If you're insane enough to want it higher, you can do so in the config by hand.
* /bgon unload - Manually unloads unused chunks.
* /bgon scanentities - this will give you the name of all nearby entities (10x10x10 cube), exactly as it should be entered into the blacklist, to prevent /bgon clear removing them.

## Breeding Related Commands:

* /bgon togglepolice - Turns automatic policing of breeding on.
* /bgon setbreedlimit - Sets the maximum allowed mobs of type EntityAgeable in a 10x10x10 chunk, before more breeding is prevented automatically.

# Modpacks
No need to ask. Just use it. A link back to this page or the curse project would be helpful but is not required.

# License
MIT

# Authors
* Original: ZenDarva
* Current: Kreezxil

# Permission to Continue
![Continuance](https://media-elerium.cursecdn.com/attachments/218/987/lag-b-gone-private-messages-minecraft-curseforge.png)
