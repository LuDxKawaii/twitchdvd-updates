========================================================================
                              TwitchDVD
                          Made By LuDxKawaii
                          Build Version: 1.2
========================================================================

------------------------------------------------------------------------
UPDATE 1.2 CHANGELOG
------------------------------------------------------------------------
* Connectivity, UI & System
  - Added an automated in-game update system to download 
    and install new versions directly from the menu.
  - Better connection integration to Twitch for more reliable gameplay.
  - Improved color rendering to provide better visibility for dark colors.

* New Game Mode: DVDClash
  - Added DVD Clash, a brand new team-based battle game.
  - See Section 5 below for full rules, commands, and powerups!

------------------------------------------------------------------------
UPDATE 1.1 CHANGELOG
------------------------------------------------------------------------
* UI & Menu Enhancements
  - Added a quick last connect button in the main menu.
  - Game settings and the last connected channel are now automatically 
    saved and remember between stream sessions.
  - Added 1600x900 resolution.
  - Added a Reconnect Button inside the main game.
  - Added a physical Exit/End Button for the main game.

* Gameplay & Mechanics
  - Changed speed settings to modular numbers from x0.5 to x2.
  - Added an option to change speed during the game.
  - Added powerups features: size up, speed, double points, magnet.
  - Added a Powerup Toggle (enable/disable) in the options menu.

* Chat & Viewer Integration
  - Implemented the viewer command as !mydvd so users can track down their logos.

* Graphics & Visual Effects
  - Changed and updated some fonts.
------------------------------------------------------------------------
------------------------------------------------------------------------

Welcome to TwitchDVD! This is an interactive stream overlay game 
where the chat becomes the game. 
Viewers spawn in as their own bouncing DVD logos, battling it out to 
see who can rack up the most points and claim the crown.

------------------------------------------------------------------------
1. HOW THE GAME & POINTS WORK
------------------------------------------------------------------------

* THE WALL BOUNCE (1 Point): 
  Every time a player's logo hits any of the four walls, they earn 
  1 point. 

* THE PERFECT CORNER (15 Points): 
  If a player is lucky enough to hit exactly in the corner of the 
  screen, they trigger a perfect corner bounce and are rewarded with 
  15 points.

* THE CROWN:
  The player currently in 1st place will automatically wear the golden 
  crown. If there is a tie, all tied leaders share the crown.

------------------------------------------------------------------------
2. POWERUPS & GAMEPLAY MODIFIERS (CLASSIC MODE)
------------------------------------------------------------------------
Powerups can randomly spawn in the arena. You can toggle them on or 
off in the options menu. 
- Powerup can be collected 5 seconds after spawned.
- Player will be in a 2 minutes cooldown before can collect another
  powerup.

* SIZE UP: 
  Makes the player's logo significantly larger for 15 seconds.

* SPEED: 
  Greatly increases the logo's movement speed for 15 seconds.

* DOUBLE POINTS: 
  Gives the logo a glowing aura and doubles all points earned 
  for 30 seconds.

* MAGNET: 
  Creates a swirling silver vortex that sucks nearby players toward 
  the logo for 15 seconds.

------------------------------------------------------------------------
3. VIEWER CHAT COMMANDS
------------------------------------------------------------------------
Viewers use the following commands in Twitch chat to play. 

!dvd
- Spawns the viewer into the game. Their logo will automatically grab 
  their Twitch username and their chosen chat color.

!mydvd
- Spawns a bouncing arrow directly above the viewer's logo for 5 
  seconds so they can easily find themselves in the crowd.

!shake
- Gives the viewer's logo a quick jiggle on the screen. Great 
  for try to change directions or just causing visual chaos.

!target @username
- Activates homing mode. The viewer's logo will change route and 
  aggressively hunt down the target player's logo. 
  (Example: !target @ludxkawaii)

!end
- STREAMER ONLY. This command ends the game and brings up the final Top 10 Leaderboard. 

------------------------------------------------------------------------
4. STREAMER DEBUG MODE
------------------------------------------------------------------------
Debug Mode is a special testing environment accessed via the Options 
Menu. 

WARNING: Do not leave Debug Mode active while live streaming! It allows 
viewers to bypass name restrictions and can clutter your screen.

While Debug Mode is ON, the following tools are unlocked:

* !dvdc <Any Name>
  - (Chat Command) Allows you to spawn a logo with any custom text you 
    type after the command. This is used to test how long names, weird 
    characters, and capital letters affect the physics and the UI.
    (Example: !dvdc SuperLongTestName)

* Spacebar
  - (Keyboard) Instantly spawns a generic test logo (DVD1, DVD2, etc.) 
    so you can test collisions and crowd density without needing to type 
    in the Twitch chat.

* Esc (Escape)
  - (Keyboard) Instantly forces the Leaderboard to appear without needing 
    to type the !end command.

------------------------------------------------------------------------
5. DVDCLASH MODE (TEAM BATTLE)
------------------------------------------------------------------------
DVD Clash is a team-based battle game. Players are split into two teams. 
It emphasizes high-speed bouncing and collision-based team gameplay.

* HOW TO PLAY & REWARDS
  - The mode is started via the streamer only command !dvdclash. 
  - Teams compete to capture corners and accumulate points.
  - Capturing a corner rewards the team with +50 points every 10 seconds.

* LOBBY COMMANDS
  - !red : Join the Red Team.
  - !blue : Join the Blue Team.

* COMBAT & DEBUFFS
  - Players can use powerups to hit opponents, trigger debuffs, or leech points.
  - Being hit can result in debuffs (such as being floored, bitten, or infected).
  - These debuffs temporarily restrict player actions and prevent them from capturing flags.
  - Battle-specific powerups introduce chaotic team combat and display specific 
    debuff icons to indicate a player's status.

* BATTLE POWERUPS
  - The game includes unique powerups:

  - Wrecking Ball: Smash enemies into the floor!
  - Vampire: Drain points from bitten targets!
  - Virus: Severely slow down your enemies!
  - Vortex: Trap enemies in a spinning tornado!
  ========================================================================