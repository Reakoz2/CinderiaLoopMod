CinderiaLoopMod — Loop Mode
============================

Version: 1.0.0
Author: [Reakoz]
Game: Cinderia (Early Access)
Requires: BepInEx 5.4.x


WHAT DOES THIS MOD DO?
----------------------

This mod adds a Loop Mode to Cinderia. When you cross the portal after the boss of chapter 4
instead of being forced to fight the final the boss, you are presented with a choice:

  - Face the Final Boss   : continue the run normally
  - Loop Back (Keep Build): restart from Chapter 1 while keeping all your
                            spells, gear, and passive abilities

Each loop makes enemies progressively harder, with scaling you can adjust
yourself directly in the UI before choosing to loop.


FEATURES
--------

  - Custom loop choice UI appears before the final boss portal
  - Full build preservation on loop (skills, gear, relics, passives)
  - Adjustable enemy scaling sliders in the UI:
      * Enemy HP per loop (default +25%)
      * Enemy Attack per loop (default +15%)
      * Enemy Speed per loop (default +10%)
  - Scaling values are saved between sessions in the config file
  - Loop counter displayed in the UI so you always know which loop you're on


INSTALLATION
------------

Step 1 - Install BepInEx
  1. Download BepInEx 5.4.x (win_x64) from:
     https://github.com/BepInEx/BepInEx/releases
  2. Extract the contents into your Cinderia root folder:
     Steam\steamapps\common\Cinderia\
  3. Launch Cinderia once and close it - BepInEx will initialize itself
  4. Confirm it worked by checking that BepInEx/LogOutput.log was created

Step 2 - Install the mod
  1. Copy CinderiaLoopMod.dll into:
     Steam\steamapps\common\Cinderia\BepInEx\plugins\
  2. Launch Cinderia - the mod is now active


CONFIGURATION
-------------

After your first launch a config file is created at:
  Steam\steamapps\common\Cinderia\BepInEx\config\com.yourname.cinderia.loopmod.cfg

You can edit the default scaling values there directly:

  [Scaling]
  HpMultiplierPerLoop = 0.25
  AtkMultiplierPerLoop = 0.15
  SpeedMultiplierPerLoop = 0.10

Or just use the sliders in the in-game UI - they update the config file
automatically.


HOW TO USE
----------

  1. Play through Chapters 1 to 4 as normal
  2. Defeat the Chapter 4 boss
  3. Cross the portal to Chapter 5, the Loop Mode UI will appear
  4. Adjust the scaling sliders if you want
  5. Click "Loop Back" to restart from Chapter 1 with your full build
  6. Click "Face the Final Boss" to continue normally


KNOWN ISSUES
------------

  - Since Cinderia is in Early Access, game updates may break the mod.
    Check back for updates after major patches.
  - The mod does not persist the loop count between game sessions. If you
    close and reopen the game your loop count resets to 0 (your build is
    still saved by the game normally though).
  - Enemy scaling applies to all enemies including bosses.


COMPATIBILITY
-------------

  BepInEx 5.4.23.x             OK
  Cinderia Early Access (2026)  OK
  Unity 2023.1                 OK


CREDITS
-------

  BepInEx  - https://github.com/BepInEx/BepInEx
  dnSpy    - https://github.com/dnSpy/dnSpy
