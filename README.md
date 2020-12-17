# [ Boss: Runeword Master ] 

---------------------------------------
### Contents
1. [Introduction](#introduction)
2. [Runeword Master?](#runeword-master)
    - [Concept](#concept)
    - [But Why Runeword Master?](#but-why-runeword-master)
    - [Technical Side](#technical-side)
    - [Installation](#installation)
    - [Other Info](#other-info)

---------------------------------------
## Introduction
Are you waiting for Diablo II Remastered? I don't, thanks for asking. BUT, Diablo II is one of my favorite games of all time, and so I decided to make something Diablo II related in WoW universe.

---------------------------------------
## Runeword Master?
Never farmed tower? No worries, now you'll know what it is, in a bad way, too.

### Concept
The whole idea is built around runes and runewords.  
In addition to normal abilities and mechanics, every so often boss will make players draw a rune, and will receive an effect based on result.

### But Why Runeword Master?
Because not only boss will benefit and players will suffer from rune effect(s), but also if you are very unlucky, rolled runes will make a runeword, and that **may** be a big problem for you.

### Technical Side
- A dungeon boss  
- RNG heavy  
- All runes and runewords are taken straight from Diablo II  
- Effects are converted from Diablo II where possible including numerous new mechanics such as Crushing Blow and others  
- Over 100 new spells total  
- Using entries **500000+** in **Spell.dbc**, **SpellIcon.dbc**, `creature_template`, `creature_equip_template`, `creature_text`  
- Expected client locale: **enGB**

### Installation
- [Download](Releases): within Runeworder.7z you find `server` and `client` folders  
- For client: move `patch-enGB-4.MPQ` into `/Data/enGB` folder  
- For script: move `boss_runeworder.cpp` file into `/src/server/scripts/Custom` folder and use diff to update script loader  
- For DB: apply `runeworder_world_20xx.sql` to your `world` DB  
- For dbc: move provided `.dbc` files to your `/dbc` folder or apply provided patch (created using **MyDbc Editor ver. 1.2.2**)

### Other Info
Included boss entity: 'Duchess' <Mistress of Runes> is a upgraded version of Countess, which only dies miserably and drop runes.  
Used model is one of Sylvanas early test elf models.  
All of the above are just suggstions, you may want to use someting else. The only things that may break the script are creature_template fields: `mechanic_immune_mask`, `unit_class`, `type_flags` and `entry` and `ScriptName` of course.  
