RealGamer's RealBot Readme
--------------------------
"won the contest "Best Bot of the Year 2000" of CSBots@PHL"

	RealBot is written by Stefan Hendriks.

Realbot at    : http://bot.counter-strike.net/realbot
RB Fanzone    : http://bot.counter-strike.net/realbot/fanzone
Counter-Strike: http://www.counter-strike.net
		
Nuclearbox    : http://www.nuclearbox.com
RealGamer     : http://www.realgamer.nl

CSBots@PHL    : http://www.planethalflife.com/csbots

RealBot Info-Points: (At the Fanzone!)
http://bot.counter-strike.net/realbot/fanzone/infopoints.html


RealBot Readme File.
--------------------

New in Beta 2 are the sub-folders. Allowing you to update that what you need
only.

Folder			Content
DLL			RealBot Brain
LANGUAGE		Different language RB_INSULT files.
RBL			The RBL files (learned information)
RealGamer		Information about RealGamer
TXT			The TXT files

The 'main' folder contains:

BOT.CFG			Settings of RealBot, auto excecuted
RB_INSULT.TXT		RealBot Insults file
RB_NAMES.TXT		RealBot Names
README.TXT		This file
REALBOT_HELP.CHM	Windows Help file about RealBot. Dubbelclick on it.

--------------
RealBot Beta 2
--------------
Note: This version is not completely what i personally wanted to be included. However, since everybody
is screaming for a new version. I release it earlier. The following features where planned but not built
in. (so you can expect these features in future releases!).

- Drop weapons for better ones
- Personalities (change almost every aspect of a bot)
- Create own fighting styles

The following is changed/fixed/new compared to Beta 1.0:

NOTE: Some changes/new are compared to a previous internal release. I've typed them so you know how bots
      will react on several situations.

Fixes:
- Bots will not stick at each other anymore
- Bots dont switch weapons fast anymore
- Bots shoot now through breakable objects like glass.
- Bots should strafe different directions know.
- Bots now have colored chat. 
- Bots cant be added using the ADDBOT command by clients.
- Bots will less fall of heights.
- Bots defuse now properly
- Bots will now not jump when trying to defuse or planting a bomb
- Server keeps control over RB's when changing map.
- Less 'lag on new round'
- CPU Usage lowered.

Changes:
- Bots buy more flashbangs than smoke grens now
- Bots don't chat that often in dead chat.
- Bots will not pick immidiatly a gren/flash/smoke gren when
  encountering an enemy. 
- Bots strafing improved
- Bots aiming altered.
- Bots reaction times tweaked/new code.
- New navigation theory mixed with original one.
- Max info-points is now 40
- Move-info point now more affective
- Bots will never strafe/run/rush when holding sniper gun.
- Recoded bomb planting
- Recoded bomb defusing
- Chatrate depended on maxplayers in server

New:
- New fightingstyle: Duck and shoot (more stable, head is target)
- New fightingstyle: Moveback and shoot (retreat fire)
- New Strafing styles:
  + STRAFE-RUSH
  + STRAFE-RETREAT
  + STRAFE-JUMP
- Bots try to change from time to time their fighting style.
- Sometimes a bot will choose knife when it has no enemy so it can move faster. 
- Better unstucking and preventing using strafe.
- Bots use ladders a lot better now.
- Bots will shoot through rotating doors when enemy is
  spotted and behind a rotating door.
- Bots help each other out. Bots who see friendly bots shoot enemies
  will help them if they dont have an enemy yet. 
- Bots are affected by level type. Its more like "rushing team vs
  camping/defending team".. 
- Dedicated server support (read below)
- New command : 		rb_removebot <amount> <team>
- New command :			rb_maychat <value>
- End-round command is now also added as console command; rb_endround
- When bots camp, some bots will randomly leave if to much bots are camping
- Radio Command: Go Go Go -> Bots stop camping
- rb_insult.txt translated in the following languages:
	Bulgarian
	Danish
	Dutch
	English
	Finnish
	French
	German
	Greek
	Italian
	Indonesian
	Norwegian
	Portuguese
	Spanish
	Swedish
	Tagalog
	>>>>>>>> Read the realbot_chat.txt file which is located in the LANGUAGE folder!
	
Removed:
- command RB_EXTRASKILL has been removed.


Info-Points:
- Maps are remapped, thanks to MikeJ for his great job!
- LADDER info-point. If you want to force bots using ladders.
- Tweaked "refine/filter" code.
- "refine/filter" code only called via menu. No more when saving RBL or
  after each round.

Misc:
- Just lots of tweaks you wouldnt notice that much and not worth to mention.
- More insults
- More names
- New directory structure!
- Translations of the bot chat insult sentences. So far only the insult file.
  The dead chat is only in english..

DEDICATED SERVERS:
The syntax is:

BOT <COMMAND>

NOTE: In a dedicated server you cannot pass arguments, this bug is known and
      being worked on.

The commands:

ADDRB <team> <model> <name> <skill>	- Adds bot (!!!)
FILLSERVER 				- Fills server with bots 
REMOVEBOT <amount> <team>		- Removes <amount> bots.  (!!!)
MIN_BOTS <min>				- Min bots that should be in game (!!!)
MAX_BOTS <max>				- Max bots that may be in a game (!!!)
RBHELP					- Small help
FORCESKILL <skill>			- Force bots to be skill <skill> (!!!)

!!!-> The arguments will not work!!! Dont fill them in. MIN_BOTS and MAX_BOTS will
       only work if they are in the bot.cfg!


------------------------------------------------------------------------------
			Previous RealBot Versions
------------------------------------------------------------------------------
Beta 1.0 - Finally:
===================
List compared to FTR 2.1

Fixes:
- More fixes for changing angle.
- MAC10 is now no longer used as sniper gun.
- Fix in Menu, accidently switched SNIPE and CAMP info-point, thats
  why the CAMP info-point didnt work properly
- Fix in time for blinded bots. (Thanks [DUSK]PacMan!)
- Bots aim better.
- Bots buy Armor more often.
- Only Servers can perform realbot specific commands, also only servers 
  can use MENU and add bots. Clients will get a 'unknown command' error
  when they try to add bots or do any other RealBot specific command.
- Bots use FN Five Seven Handgun now properly.
- Again a distance check fix in Defuse Code
- info_bomb_target is now also chased by Terror bots to plant bomb.
- All Counter Bots will have the C4 as goal when planted now.

Changes:
- Better info-point refine code
- Bots get less confused now by more MOVE info-points.
- Bots buy less grenades and flashbangs.
- Bots chase you better
- Bots speed up faster.
- rb_extraskill console command more effective. Bots only aim for the head
  and the aiming is more refined, STILL based uppon skill though!
- When enemy far away, it will aim for body, not head (also not when extra
  skill is enabled).
- Botmenu is now bound with key "h".

Info-Points:
- CAMP info-point works now basicly. 
  Bots report 'in position' most of the time (depends on skill).


New:
- Bots learn jumping and ducking again!
- rb_forceskill <skill>  command,
  will force realbots be <skill>.
- When a bot is hit by a bullet but he can't see where the enemy
  is, then (depended on skill) the bot will not know immidiatly where that
  shot came from.
- Bot Personalities:
	
	COWARD		-> Calls more for backup and is more afraid
	
  More personalities will be implemented in further versions. 
  (this code is in early stages)

- New Navigation Thinking! Instead of 2 seperate Navigations, the bots use the
  2 navigation types combined! Still, maps WITHOUT ANY MOVE info-points will use
  the FTR 1 navigation. (*new navigation type, read further for rb_navigationtype*)
- Bot dont shoot team mates , lower skilled bots do shoot teammates.
- Bots now understand the new sniper gun of CS 1.0
- rb_freeze command, for those who think moving targets are hard to hit... :)
- Bots can camp now, even low skilled bots might just have a habit of camping
- rb_init console command (same as realbot_init)
- New fighting style : Strafe
- Bots do a little chat when they are dead, sentences are hard-coded and
  picked randomly. Some sentences are 'global', meaning they can be a reaction
  or just a comment on how they died. There is no logical order in picking the
  sentences, but there can be some funny dialogs by these Global sentences.
- rb_navigationtype ## command, choose what type of navigation:
  0 (default) = Optimized and merged FTR 1 + FTR 2.1 Navigation (less CPU usage)
  1 = New Ai Think order usage of FTR 1 and FTR 2.1 Navigation (more CPU usage, smoother nav)
- Basic Hostage Rescue Code implemented. (mail me if you notice a bot rescue a hostage! thx!)
- Primitive Smoke Grenade Support. Higher skilled bots dont lose enemy fast, 
  while lower skilled bots do. Some bots 'wait' and some bots rush through smoke.
- Bots buy and use smoke grenades. 

Misc:
- Nice windows-help file. Realbot_help.chm. Dubbelclick on it to see it.
  Created by Sadbloke, thanks!
	
Summary of new Commands:
- rb_init (same as realbot_init)
- rb_forceskill
- rb_freeze
- rb_navigationtype

Feature Test Release 2.1 , for the public:
==========================================
Fixes:
- Upgraded little bit navigation
- Bots don't want to follow you anymore in a new round (when round ended with following 
  bots).
- Aim Bug fixed. (bots should be a lot harder to kill now again.) 
- CPU Usage lowered, same navigation results (even improved here and there)

New:
- All weapons supported (can be bought and used by bots).
- Some better burst fire, bots burst when you are pretty far away. 
- Caution code! Bots can get cautious, or want to rush. When low on health
  it can get afraid, and is more cautious too!
- Removed 'learn jumping and ducking' code! This code will be re-implemented
  for the next release. The current code is not efficient enough. (so, place
  them by yourself!)

Optimized maps:
AS_FOREST
CS_BACKALLEY -> Attemption, don't count on a big battle.
CS_ITALY

Added Optimized RBL files from MikeJ's MapOpPack:
AS_TUNDRA
AS_HIGHRISE
CS_747
CS_ARABSTREETS
CS_ESTATE
CS_OFFICE
DE_AZTEC
DE_CBBLE
DE_PRODIGY
DE_VEGAS

(in total 20 optimized maps!)

Changes:
- changed bot_beta7 command into a multiple version console command:  
  New Command Name: rb_playingcs <value>

  Value		Means
  0		Playing CS 1.0			<DEFAULT>
  1		Playing CS Beta 7.1/7.0
  2		Playing CS Beta 6.6/6.5

- mp_autoteambalance 0 is now set at the bot.cfg so the teams will not
  be balanced when using ME VS ALL BOTS mode.

- More Optimized maps! (Some By MikeJ)

- Adjusted GRENADE and FLASH code, i hope it makes them a little bit better with their usage.
- Changed command rb_addwaypoint into rb_addinfopoint

- MOVE info-points have priority #1 when you add them. Meaning when database
  is full. Then it will try to 'overwrite' it with a lower priority info-point.
  (MOVE is #1, JUMP and DUCK #2 , etc)


Misc:
- When typing RB_MINSKILL or RB_MAXSKILL without value, you can see what the
  current settings are.

- RB_HELP Console Info Updated.


Feature Test Release 2 , for the Public:
========================================

New:
- Menu for Adding bots and other stuff
- Very primitive learning system. Currently learns Jumping and Ducking
- Global Waypoint System supported. Waypoints must be placed by Humans.
- "EndRound" command. (Thanks Ditlew!)
- "Me VS All Bots" command. (via Menu)
- rb_minskill and rb_maxskill console commands.
- rb_extraskill command to make bots even harder to kill.
- Q key is bound as Menu in BOT.CFG

Changes:
- Bots will not listen to radio when blinded.
- Buying code tweaked for dual berettas (5% change)
- FTR 1 bot.cfg settings hard coded as default
- A little change made, less chance that lower skilled bots
  will buy a new weapon, even when they have one already.

Fixes:
- Bots will not follow you anymore when blinded.
- Counter-Strike V1.0 Compatible
- Distance fix in DEFUSE BOMB code. 
- Fixed some code on BOMB PLANTING code.
- Some fix with FOLLOW ME code.. now bots move more realisticly after you!

Misc:
- Added a new manner for 1 Human VS xxx bots in the realbot_manual.txt
- Rewrote the bot.cfg, should hopefully fix the MSG_ONE error
- RealGamer Document, read here what it is...
- realbot_infopoint.txt , fully explained txt file about info-points and
  how to add them.

Maps:
- Included Optimized(*) RBL Files:
  CS_ASSAULT
  CS_SIEGE
  CS_MILITIA
 
  DE_DUST
  DE_TRAIN
  DE_NUKE
  

(*) Although RealBot auto-generates RBL files, you need to place MOVE info-points
    to optimize the maps even more. Without these info-points they are not officially
    optimized. The included RBL files have MOVE info-points to let bots move with more
    knowledge of the map layout.

NOTE: Its recommended to download the patch to upgrade HL
to version 1.1.0.4, this fixes most changelevel bugs too!

NOTE 2: There is NO Hostage Rescue code.



Feature Test Release 1:
=======================

- Totally NEW navigation code (much faster)
- Bots affected by flashbangs
- Bots throw flashbangs
- Bots reload much better
- Door usage much better
- Bots have a better sight
- Bots have a first reaction time
- Bots don't shoot at unbreakable stuff that can't be broken
- Bots listen to radio (Thanx to Ditlew!)
- Bots use more radio
- Aiming , buying, and other behaviour affected by skills
- Bots use CS 7.x weapons (and still compatible in 6.x)
- Bots almost don't fall of heights
- Less CPU usage 
- Bots buy secondary guns
- 10 extra names
- Bots use ALL CS weapons.
- Chat sentences and names are loaded from TXT files!

Read REALBOT_MANUAL.TXT to read how it works.

To UNINSTALL (deactivate), run RB_UNINST.BAT
To RE-INSTALL (activate), run RB_REINST.BAT
To TOTALLY UNINSTALL(remove), run RB_UNINST.BAT, then RB_CLEAN.BAT

RealBot Names are in: rb_names.txt
RealBot Insults in  : rb_insults.txt

-------------------------------------------------------------------------------
				REALBOT CREDITS
-------------------------------------------------------------------------------
Coding:

Botman		- HPB Bot Code, and help with problems.
Stefan		- RealBot AI , Combat, etc.

Help on Coding:
Ditlew		- exchanging code information for new features.
DaTa		- for the great conversations about AI.
Count Floyd	- For the last 2 Entity's of CS 1.0
DarkYouth	- Nice conversations about navigation/learning maps etc.

Bugs and overall Help:
GooseMan	- help on flashbang, and other questions.
Cliffe		- for his help on HTML.
Marcus Klimstra - For the menu code.
MikeJ		- Optimized RBL files!
ImpaileR & Necro- For testing previous versions of RB and being in the team.

Official Testers:
SadBloke
Leagle		
Ca$h
Neverwinter
Siro
Mike

Offical Optimizer:
MikeJ

RealBot for Dummies txt file:
ca$h
[ATC]Poison for his help.

Website(s):
CS.NET		- For hosting realbot, thanks to the CS team!
Sputsnik        - For his official fansite about RealBot!
CSBots@PHL	- For their great up-to-date news and for
                  the "Best bot of the Year 2000" contest.