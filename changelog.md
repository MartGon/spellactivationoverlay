## SpellActivationOverlay Changelog

#### v0.6.1 (2022-09-06)

Shout-out to MartGon and xHashii for their contribution to the code. Thanks!

- Buttons should glow correctly when using Bartender, ElvUI or Dominos
- New GAB: Hunter's Kill Shot button glows when the target has low HP
- New GAB: Paladin's Hammer of Wrath button glows when the target has low HP
- New GAB: Warrior's Execute button glows when the target has low HP
- New GAB: Warrior's Victory Rush button glows after killing an enemy
- Riposte should display its SAO as intended
- Reload UI should no longer cause a Lua error because of options
- Glowing Buttons checkbox should now apply the option correctly

#### v0.6.0 (2022-09-04)

- After extensive testing, SpellActivationOverlay now leaves its Beta phase!
- Options Panel, available from Interface > AddOns > SpellActivationOverlay
- Options for Spell Alerts: opacity, scale factor, offset
- Options for Glowing Buttons: on/off
- A "Toggle Test" button displays fake Spell Alerts for testing interactively

#### v0.5.0-beta (2022-08-31)

SpellActivationOverlay now has a Discord server!
Make sure to check it out at https://discord.gg/VrDkvDV4

Support for Glowing Action Buttons (GABs), making some actions glow, namely:
- Death Knight's Rune Strike button glows after parrying or dodging an attack
- Death Knight's Howling Blast button glows during Rime
- DK's Icy Touch/Frost Strike/Howling Blast buttons glow during Killing Machine
- Druid's Wrath button glows during Solar Eclipse
- Druid's Starfire button glows during Lunar Eclipse
- Hunter's Counterattack button glows after parrying an attack, unless on CD
- Hunter's Aimed/Arcane/Chimera Shot buttons glow during Improved Steady Shot
- Hunter's Arcane/Explosive Shot buttons glow during Lock and Load
- Mage's Arcane Missiles button glows during Missile Barrage
- Mage's Pyroblast button glows during Hot Streak
- Mage's Fire Blast button glows during Impact
- Mage's Fireball and Frostfire Bolt buttons glow during Brain Freeze
- Paladin's Flash of Light and Holy Light buttons glow during Infusion of Light
- Paladin's Flash of Light and Exorcism buttons glow during The Art of War
- Priest's Smite and Flash Heal buttons glow during Surge of Light
- Priest's Greater Heal and Prayer of Healing glow at 3 stacks of Serendipity
- Rogue's Riposte button glows after parrying an attack, unless on cooldown
- Warlock's Shadow Bolt button glows during Nightfall, a.k.a. Shadow Trance
- Warlock's Shadow Bolt and Incinerate buttons glow during Backlash
- Warlock's Incinerate and Soul Fire buttons glow during Molten Core
- Warrior's Overpower button glows after the enemy dodges, if in Battle Stance
- Warrior's Revenge button glows after parry/dodge/block in Defensive Stance
- Warrior's Execute button glows during Sudden Death
- Warrior's Slam button glows during Bloodsurge
- Warrior's Shield Slam button glows during Sword and Board

- New SAO: Rogue's Riposte
- SAOs should now always show up on ReloadUI

#### v0.4.2-beta (2022-08-05)

- Mage's Heating Up is no longer lost on death
- Alpha is reduced by 50% when out of combat
- SAOs are shown uplon login if player already has the corresponding buffs
- Currently, this includes all SAOs but Heating Up, which is not a buff

#### v0.4.1-beta (2022-08-05)

- New SAO: Paladin's Infusion of Light
- Textures should keep pulsing after gaining/losing stacks
- Mage's Heating Up does not pulse anymore
- Shamans's Maelstrom Weapon does not pulse at stacks 1-4

#### v0.4.0-beta (2022-07-31)

- Because all classes are supported, the addon now enters its Beta phase!
- New classes: Druid, Hunter, Rogue
- New SAO: Druid's Lunar Eclipse
- New SAO: Druid's Solar Eclipse
- New SAO: Druid's Omen of Clarity
- New SAO: Hunter's Improved Steady Shot
- New SAO: Hunter's Lock and Load
- New SAO: Mage's Impact
- New SAO: Shaman's Elemental Focus
- The Rogue class, although supported, currently doesn't have any SAO

#### v0.3.4-alpha (2022-07-31)

- New class: Warlock
- New SAO: Warlock's Backlash
- New SAO: Warlock's Empowered Imp
- New SAO: Warlock's Molten Core
- New SAO: Warlock's Nightfall, a.k.a. Shadow Trance

#### v0.3.3-alpha (2022-07-29)

- New classes: Shaman, Warrior
- New SAO: Priest's Serendipity
- New SAO: Shaman's Maelstrom Weapon
- New SAO: Warrior's Bloodsurge
- New SAO: Warrior's Sudden Death
- New SAO: Warrior's Sword and Board

#### v0.3.2-alpha (2022-07-27)

- New classes: Priest, Paladin
- New SAO: Priest's Surge of Light
- New SAO: Paladin's Art of War

#### v0.3.1-alpha (2022-07-26)

- New SAO: Mage's Missile Barrage
- New SAO: Mage's Brain Freeze

#### v0.3.0-alpha (2022-07-25)

- New SAO: Mage's Fingers of Frost
- Major changes to how stackable auras, such as Fingers of Frost, are handled
- Due to a game limitation, stackable auras rely a bit less on combat logs
- Talent checks could fail during login
- This addon no longer stores data to the game client local storage

#### v0.2.0-alpha (2022-07-24)

- Major changes to how custom code can be implemented, on a per-class basis
- Mage's Heating Up is now fully functional
- Mage's Heating Up now triggers only for mages who picked Hot Streak talent

#### v0.1.2-alpha (2022-07-24)

- New SAO: Mage's Heating Up, barely functional because Wrath has no such buff
- Factorized code in common.lua

#### v0.1.1-alpha (2022-07-24)

- New class: Mage
- New SAO: Mage's Hot Streak

#### v0.1.0-alpha (2020-07-24)

- SpellActivationOverlay is now public!
- Addon hosted on Curse https://www.curseforge.com/wow/addons/spellactivationoverlay
- Source code is available on GitHub https://github.com/ennvina/spellactivationoverlay
- This release mostly focuses on cleaning up some files before sharing them

#### v0.0.5-alpha (2022-07-24)

- Track combat event log instead of unit auras
- Support for stackable effects, although no stackable example is written yet

#### v0.0.4-alpha (2022-07-23)

- Utility functions are now centralized in common.lua
- First working Spell Activation Overlays (SAOs): DK's Rime and Killing Machine

#### v0.0.3-alpha (2022-07-23)

- Custom code for initializing new frame members
- Extra caution to ensure Blizzard original code changes as little as possible
- Utility functions to work around auras; defined in a separate source file

#### v0.0.2-alpha (2022-07-23)

- Re-use WeakAuras "Blizzard Alert" category for listing textures
- Map texture IDs to a local texture name in the addon folder

#### v0.0.1-alpha (2022-07-23)

- Re-use Blizzard code from Retail's FrameXML source code
- Re-use Rime and Killing Machine textures from Retail
- Ignore displaySpellActivationOverlays cvariable, unavailable in Classic
