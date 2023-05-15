# Overview

Are you looking to end the pernicious threat of artificial intelligence? Maybe play the inverse of Determined Exterminators, or the slightly friendlier cousins of Fanatic Purifiers? Look no further, this is the mod for you! Play as the Organic Zealots who seek to outlaw and curtain development of cybernetics, robotics, and artificial intelligence. Should they encounter an abominable Machine Intelligence, or should the worst come to pass and an organic empire synthetically "ascend..." - that's what the Anti-Thinking Machine Jihad is for.  _Thou shalt not make a machine in the likeness of an organic mind._

# Changes

This mod introduces a new homicidal civic, the Organic Zealots. They engage in diplomacy with organic species (including cybernetic ones, but they don't like it), and have a total war _casus belli_ against synthetic empires and machine intelligences. They are effectively the inverse of Determined Exterminators. Organic Zealots also have the option to join the defense of empires suffering a Machine Uprising - but beware - Determined Exterminators now also have the option to join the Machine Uprising in support of the new Machine Intelligence! These options are weighted so that AI empires with these civics will be interested in helping "their" side but not suicidally so.

In order to make Organic Zealots more interesting, this mod introduces a new war goal for them to "Outlaw Cybernetics, Robot Pops, and AI" against empires which allow any of those areas. Should their target lose, it will be forced to cease all cybernetic and robotic pop assembly, cease cybernetic assimilation, outlaw robot Pops, outlaw artificial intelligence, and be prevented from pursuing cybernetic or synthetic ascension for 20 years!  Status quo results in a new empire being created which outlaws the relevant policies, if there is at least one occupied colony.  Subjects of Organic Zealots are prevented from pursuing these areas indefinitely!

The war goal to "Outlaw Cybernetics, Robot Pops, and AI" uses a new _casus belli_ "Impose Policy" which is available to any empire (although only Organic Zealots currently have a corresponding war goal).  It is ripe for expansion with new ways for empires to force their ideas onto others via additional custom war goals.  What can you come up with to mod?

To offset the penalty Organic Zealots suffer by not being able to assemble robot Pops, this mod introduces a new building and job (Clone Birth-Labs employ Cloning Technicians) to create Organic Pop Assembly for them.  The building is available to any non-gestalt empire with the Cloning technology.  Organic Zealots begin the game with Cloning unlocked and Clone Birth-Labs, if there is space on their homeworld.

Organic Zealots and empires that outlaw AI can no longer research Positronic AI, but can instead now research Mentat Computation to unlock special leader traits for organic rulers, governors, and scientists.

Finally, this mod overrides many built-in events where artificial intelligence or robotics come into play in order to offer Organic Zealot-themed options, excluding First Contact events.  As a side-effect of needing to override related events anyway... the Enigmatic Cache scans planets 10x faster (1 years vs the original 10) so that it has a hope of completing its task at some point before the end of the game and getting to the event where it offers to "uplift" an empire.

## Compatibility

Due to a significant number of overrides to implement the new, homicidal Organic Zealots civic, this mod may conflict with other mods that alter core gameplay mechanics.  It is explicitly compatible with all mods authored by me, CorsairMarks.  This mod has one minor conflict with [Gigastructural Engineering](https://steamcommunity.com/sharedfiles/filedetails/?id=1121692237) regarding orbital bombardment policy.  This mod does not conflict with [Planetary Diversity](https://steamcommunity.com/sharedfiles/filedetails/?id=819148835).

What this means to you as a player is that you should carefully vet other complex mods to see whether they will work alongside this one. You may wish to use a mod conflict solver such as [Irony Mod Manager](https://bcssov.github.io/IronyModManager/) to detect and potentially resolve conflicts between this mod and others.

Built for Stellaris version 3.8 "Gemini."  Not compatible with achievements.

### When to Install

This mod should be added before starting a new game and not removed from an in-progress game.

### Not Included in "Subtle Polish"

This mod is intentionally not included in my modpack [Subtle Polish: A Collection of Fixes and Enhancements](https://steamcommunity.com/sharedfiles/filedetails/?id=2522974089) because it is a new civic.  It is otherwise fully compatible.

### Mods With Gameplay Interaction

* [Assimilate All the Pops](https://steamcommunity.com/sharedfiles/filedetails/?id=2908463208) respects restrictions that can be placed on assimilation and ascension by losing an "Outlaw Cybernetics, Robot Pops, and AI" war or having an Organic Zealot as an overlord
* [Deassimilate Machines](https://steamcommunity.com/sharedfiles/filedetails/?id=2553812372) outlaws Machine Deassimilation in the event of losing an "Outlaw Cybernetics, Robot Pops, and AI" war or having an Organic Zealot as an overlord
* [Forgotten History](https://steamcommunity.com/sharedfiles/filedetails/?id=2916982793) by [kroun](https://steamcommunity.com/id/metallichydra/myworkshopfiles/?appid=281990) allows you to begin as Origin: Banished Threat, an origin specifically for homicidal empires - start having just escaped your shielded world!

## Known Issues

### Gameplay

* Organic Zealots can never choose a "friendly" greeting when meeting other empires
    * There will never be a "green" option when making first contact, only the yellow and red options
    * Could be added but requires overwriting two significant events with compatibility concerns
* Some events and diplomacy screens may have no options for Organic Zealots
    * Please report which ones in the Steam comments, my Discord channel, or GitHub
    * This is usually because the game uses the `is_homicidal` trigger to exclude those types of empires, but only offers options for the built-in homicidal civics rather than a catch-all choice - I can fix it by overriding the relevant event to add an appropriate option
* Organic Zealots cannot interact with enclaves or the caravaneers - Paradox blanket-bans any homicidal empires from communicating with them, and this mod does not alter those restrictions

### Error Logs

So, so many game object overwrites will leave warnings in the error.log file.  These overwrites are to enforce the homicidal nature of Organic Zealots and having other empires react accordingly.  Here is a short list of what is affected: some ascension perks, many diplomatic actions, some game rules, many policies, a few crucial built-in scripted triggers, the assimilation citizenship type, several purge types, some AI-related technologies, the traditions which enable the cybernetic and synthetic special projects, and most built-in events dealing with AI or robots/machines.

## Changelog

* 1.0.0 Initial version
* 1.1.0 Add support for Origin: Banished Threat from [Forgotten History](https://steamcommunity.com/sharedfiles/filedetails/?id=2916982793)
* 1.2.0 New anti-cybernetics features for Civic: Organic Zealots
    * Cannot research Integrated Cybernetics (and by extension, also Quantum Neuro-Links)
    * Can deassimilate cybernetic species to remove their cybernetic implants, attempting to convert them to the relevant biological traits in the process (with the technologies Gene Tailoring and Gene Banks)
    * Improve compatibility with Forgotten History
    * Fix broken edits for the Helpful Drones event chain
    * Properly allow _all_ other empire types to declare an End Threat (Containment) total war against Organic Zealots - was incorrectly limited to robotic empires only
* 1.3.0 Update Mentat traits for governors and rulers - governors now reduce pop upkeep by 5% and have decreased other bonuses, rulers have a lower unity bonus
* 1.3.1 Fix bug introduced in 1.2.0 that disallowed Civic: Organic Zealots from proposing Secret Fealty, courtesy of reporting by [MrFunEGUY](https://steamcommunity.com/profiles/76561198025143641/myworkshopfiles/?appid=281990)
* 1.3.2 Event bugfixes ([MrFunEGUY](https://steamcommunity.com/profiles/76561198025143641/myworkshopfiles/?appid=281990) strikes again)
    * Fix the Galactic Community invitation event `galcom.16` so it can be rejected by empires with Civic: Organic Zealots
    * Ensure that the Marauder rejection event `marauder.19` for homicidal empires can handle Civic: Organic Zealots (unused by this mod, but just in case)
    * Add a fallback homicidal option for both the above events
    * [Machine Deassimilation](https://steamcommunity.com/sharedfiles/filedetails/?id=2553812372) was not allowed after an empire gained access different form of assimilation - thanks [wagnerleung0079](https://steamcommunity.com/profiles/76561198261183621)
* 1.3.3 Ensure that Organic Zealots have can declare Total War on normal End Threat targets (Awakened Empires, other homicidal empires)
* 2.0.0 Update for Stellaris version 3.7 "Canis Minor"
    * Integrate underlying game changes
    * Allow homicidal empires to assimilate their main species (Organic Zealots can gene-deassimilate or psionic assimilate any qualifying species)
    * Civic: Organic Zealots is now more rare
* 2.1.0 Code refactoring for better reuse - no functionality changes
* 2.2.0 Code refactoring
    * Remove overridden origins from Forgotten History in favor of a script_value compatibility file
    * Rename and add more validation triggers (similar to additions in 2.1.0)
* 2.2.1 Performance improvements for assimilation - only process species which have at least one Pop
* 3.0.0 Update for Stellaris version 3.8 "Gemini"
    * Integrate underlying game changes
    * Mentat leader trait now has a variation for every leader class

## Source Code

Hosted on [GitHub](https://github.com/corsairmarks/organic_zealots)

### Development Notes

It is best to clone this repository into `<Stellaris User's Directory>/Paradox Interactive/Stellaris/mod`, and then make a connection to the `mod` folder via a `*.mod` file's `path` property.  That will ensure the game can see the files, and also that CWTools will parse them.  Also note that the README.md file exists in the `mod` directory but is symbolically linked in the root directory.