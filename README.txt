KINFRAL SMP - POWERS (Fabric 1.21.11, single player)

15 powers, 3 stages each, PvE only (powers can only ever hit hostile mobs, never players).
Each stage is bought at an altar by giving up valuables from your inventory:
  Stage 1: 2 Blocks of Gold
  Stage 2: 3 Blocks of Diamond
  Stage 3: 1 Block of Netherite
(edit the costs in Stages.java)

COMMANDS (work even with cheats off)
  /altar                  Summon an altar where you are looking.
  /powers                 List powers + stages.
  /powers wand            Get the Power Wand (a glowing Blaze Rod).
  /powers select <name>   Pick which power the wand uses / the altar upgrades.

HOW TO PLAY
  1. /altar, then right-click the enchanting table (it sits on crying obsidian).
  2. Right-click = buy the next stage of the selected power. Sneak + right-click = switch power.
  3. /powers wand. Right-click with it = use the selected active power.
     Sneak + right-click with it = switch power.
  4. Passive powers are always on once unlocked.
  5. Sneak while mining to break blocks normally (skips Vein Miner / Tree Feller).

ACTIVE (wand):  Shadow Step, Lightning Strike, Grapple Hook, Phase Dash, Earth Bender,
                Ice Nova, Gravity Slam, Mob Freeze, Beast Summon
PASSIVE:        Soul Harvest, Blood Rage, Vein Miner, Tree Feller, Flame Aura, Soul Shield

BUILD (IntelliJ IDEA + Java 21)
  1. File > Open > pick this folder. IntelliJ downloads Gradle 9.2 by itself
     (gradle/wrapper/gradle-wrapper.properties) and syncs. Wait for it to finish.
  2. Open the Gradle panel (elephant icon, right side) > Tasks > build > double-click "build".
  3. The jar is in build/libs/kinfral-smp-2.0.0.jar (not the -sources one).
  4. Put it + Fabric API for 1.21.11 in .minecraft/mods, launch the Fabric 1.21.11 profile.
  - Versions used: Loom 1.14-SNAPSHOT, Yarn 1.21.11+build.4, Fabric API 0.141.1+1.21.11.

NOT COMPILED: this source was written without being able to compile it. If the build
shows errors, send them over and they get fixed. Version-sensitive spots are in the
"Version-sensitive helpers" block at the top of Abilities.java.
