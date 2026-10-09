---
{"dg-publish":true,"permalink":"/Create Lemonade/","dgShowToc":true,"created":"2026-08-04T07:52:07.603+09:30","updated":"2026-10-09T14:41:39.495+10:30"}
---

Welcome to my main working document! Information relevant to actually playing the pack is stored in the in-game wiki (accessible via the pause menu). This document has the full credits, my workings, a shader breakdown, and some easily-changed performance settings if you aren't getting enough FPS!
# Shaders, Performance and Other Settings

#### **Shaders**

Create: Lemonade bundles three shaders to choose from (alongside Vanilla). These have been chosen and configured for pixel shadows, block outlines, visibility in dark areas, and support for relevant visual mods. I recommend Mellow, as it greatly improves visuals for very little performance cost. If you have a stronger system, Photon looks fantastic while also keeping relatively good performance.
Complementary + Euphoria Patches and Vanilla are backup choices. They're also the only two who fully show CliffTree's custom sky colours.

Your performance will vary as your system will be different to mine, however, this hopefully gives a good idea of visuals and relative performance between the shaders.
Not to mention that this benchmark was done a while ago so the FPS should be improved a bit in the current pack.

**Vanilla**
280 FPS
![vanilla.png](/img/user/Attachments/vanilla.png)

**Mellow**
258 FPS
![mellow.png](/img/user/Attachments/mellow.png)

**Photon**
130 FPS
![photon.png|720](/img/user/Attachments/photon.png)

**Complementary + Euphoria Patches**
61 FPS
![complementary.png|720](/img/user/Attachments/complementary.png)

#### **Performance and Other Settings**

**Quick Settings**
*Glowing Ores:* Go to Resource Packs, find 'Glowix' in the activated packs, and click the settings icon to the right when you hover it.

*No Spider Mode:* Go to Resource Packs, find 'Arachnophobia Mode' on the left, and enable it.

**Performance Settings**

Here's some of the most performance-costly settings that are on by default in the pack that you might want to disable!
If you're unsure what's causing the lag, open your Task Manager (or equivalent) and see what's being used the most - your GPU or your CPU. Settings are sorted here per what they effect the most.

-- CPU --
*C2ME*: If you have a cheap or old computer, and/or a CPU with not many threads, removing this mod may improve your frame stability when generating new chunks. Make sure to remove C2ME's OpenCL Engine as well if you do this.

-- GPU --
*Rainbow's Foliage:* Disable this resource pack to improve FPS in very leafy areas.
*Interactive Foliage:* Go to 'Mod Configs' in the pause menu and turn off 'waving leaves' to improve FPS in leafy areas. Optionally disable it entirely.

# Workings

**it's rebuild time**
disabling everything and working up from scratch. will stick things with a checkmark as i go. :LiBadgeCheck:
first run (nothing at all enabled) :LiBadgeCheck:
utility stuff :LiBadgeCheck:
performance stuff gets a sweet 1200fps-ish on 10 RD :LiBadgeCheck:
bugfix stuff :LiBadgeCheck:
menus :LiBadgeCheck:
sounds :LiBadgeCheck:
general rendering setup :LiBadgeCheck:
overlays etc :LiBadgeCheck: (didn't impact FPS very much at all yay!)
**foliage** :LiStarHalf:
	also waiting on a fix from interactive foliage for a leaf shading issue. wavy leaves is staying off for now.
	leaf-heavy scene benchmark at 10RD: 440
particles :LiBadgeCheck:
animations :LiBadgeCheck:
mobs :LiBadgeCheck:
item :LiBadgeCheck:
blocks :LiBadgeCheck:
create aesthetic section :LiBadgeCheck:
'other' aesthetic section :LiBadgeCheck:
LOD mods :LiBadgeCheck: (FPS sits at about 250 with Voxy RD set to 512 and vanilla RD at 5. And subdivision size at 164. These can all be tweaked for more performance, by lowering the RDs and/or raising the subdivision size.)
create actually :LiBadgeCheck: 
world generation :LiStarHalf:(performs fine, albeit I tested without LOD mods on, I'm just waiting for more streams reflowing bugs to be patched)
emission shading lighting :LiBadgeCheck:
shaders :LiBadgeCheck: (i've been testing as i go, will probably need to revisit at some point though)
balance :LiBadgeCheck:
QoL :LiBadgeCheck:
minor additional content

im starting to think i fixed the performance issue somewhere along the way without realising, that or it's related to LOD mods.


**here's to monitoring the state of things:**
	- voxy doesn't work with shaders on 1.11.4 iris, which forces a downgrade, which brings interactive foliage into an unusable state. it also doesn't render far beacon beams.
	- DH meanwhile has issues with biome colour (still) and does have poorer framerates and a generally poorer look.
	- meridian isn't even released yet; but it struggles to work correctly with shaders
	- all of them piss me off rn but i want to be able to check compatability moving forwards... ugh. i guess i'll downgrade interactive foliage and... but ugh!!!
	- no, i think i'll turn them all off in the meantime.

**it'd be so cool to have custom villager noises based on type but idk if its doable yknow**

https://github.com/Apollounknowndev/wikiful/wiki wikiful documentation
#### To-do/In Progress

**Undecided on what to do yet**

- [ ] more enchanting achievements may be in order..? though i think the structure is straight forwards enough right now. story/enchant_item <- enchant an item (good parent)
- [ ] maybe craftable trident with create's big crafter since they're so annoying to get for something kinda mid; or make it a guarantee drop
- [ ] I want to implement something similar to a Villager Trade Rebalance, but with respect for Enchancement's custom enchantments and the lack of tool durability (ergo no need for unbreaking or mending). TL:DR Biome based villager trades. encourages exploration at least before making a trading hall lmao
- [ ] regardless of if we use toroidal or not, i might want to run my seed search again for a smaller radius, it just feels a bit much at the moment. something that matches toroidal's max size, which is 4096 iirc
- [ ] i'm unsure what to do about nether mobs because there's no sky there and they feel a bit unavoidable. same curiosity about illagers and elder guardians tbh i dont even know what the nautilus or zombie nautilus do. should do something to phantoms

**In Game**
- [ ] figure out all the automatable and renewability matrices
- [ ] idk why block replacement isnt working bro
- [ ] why does getting a wikiful tip prompt a copper chain stonecutter recipe popup? related to error in logs perhaps.
- [ ] figure out if my jei hotfix respack thing worked or now
- [ ] keep working on whatever happened to the create things in jei.
- [ ] spin up a test instance with just voxy seedgen and go find a ocean monument, does it sit on top of the water? if so report bug if not why the fuck does it do that in the pack
- [ ] why are complementary's clouds so low lmao

**Between Loads**
- [ ] Refactor the QoL, Balance, and Minor Additional categories once I'm done with my testing
- [ ] why cant i diddle the god damn fog
- [ ] get snow overlays to work on top slabs at the very least
- [x] add 'adult zombies only', '-----------', 'made by sniffercraft34', 'click to enable' 'click to disable' to the chat blocking
- [ ] look through the logs for issues and tackle one by one :)
- [ ] debate adding BBE anyway, despite the chest shading issues
- [ ] make [superior smelting](https://modrinth.com/datapack/superior-smelting) and [blasting plus](https://modrinth.com/datapack/blasting-plus) and [smoking plus](https://modrinth.com/datapack/smoking-plus) recipes work in create ([guide](https://github.com/Creators-of-Create/Create/wiki/Custom-Recipes))
- [ ] mark clifftree's sky biomes in biome spreader's no touchies config entry
- [ ] the snow golem's shaved head face is broken??
- [x] grass break particle is dirt
- [x] ban baby zombies. they're bullshit and i can't be arsed making the textures for them.
- [ ] completely delete copper horse armour its too confusing with the create pack on
- [ ] Add the thing into the datapack to make ruined portals surface always
- [ ] search for 'planned' and HOLD and implement or update entries, periodically.
- [ ] add axiom, make a creative building guide wiki page
- [ ] Add overlay logic onto Create's blocks where it makes sense to do so (i.e tuff and deepslate gen next to ochrum...)
- [ ] debate setting up very minor "lore" and a starting structure, like satisfactory.
**For Release**
- [ ] I've disabled CliffTree's sky biomes for the meantime because it makes world previews difficult to see. I re-enable these once i'm done using seed preview.
- [ ] remove xaero's map, spark profiler, and seed preview/other unneeded mods
- [ ] check through the mods and resource packs and make sure they have listings here
- [ ] migrate to a resource pack management mod that lets you hide / lock things
- [ ] check for unused configs, caches, etc, and bin them.
#### Waiting for help

snowy leaves broke, waiting on help

polytone fix REI/JEI black create block issue [here](https://discord.com/channels/790151253144895508/1557581632129732689)

voxy to fix its [modern iris/sodium stack incompatibility](https://github.com/MCRcortex/voxy/issues/675)

create fly makes enchancement's burrowing crash ([here](https://github.com/ZurrTum/Create-Fly/issues/303)) if this is resolved i can take burrowing off of the blacklist. for now, efficiency is there instead. For completeness, I'm disabling all multi-block-breaking enchantments as that seems to be the root of the issue.

Waiting for BBE to fix their shading [issue](https://github.com/EdeenMC/betterblockentities/issues/145)

I might reinstate falling leaves if they fix [this](https://github.com/Fuzss/falling-leaves-plus/issues/3) but it feels overkill regardless.

waiting for interactive foliage to blacklist lichen [here](https://github.com/Kart0/mc2-interactivefoliage/issues/21)

waiting for photon to fix their [player brightness issue](https://github.com/sixthsurge/photon/issues/671)

Waiting for mellow shader to push their [weird fog issue](https://codeberg.org/TheCMK/mellow-shader/issues/232) fix to a release augh i love them so much mwah mwah mwah

https://github.com/Qendolin/better-clouds/issues/386

Waiting to see if I Like Vanilla will consider [supporting vanilla fog and sky colours](https://github.com/What42Pizza/I-Like-Vanilla/issues/51)

[voxy worldgen pause screen OOM crash](https://github.com/iSeeEthan/voxy_worldgen_v2/pull/93)
voxy worldgen is on hold until fixed

[Game close thread hang issue with Flywheel](https://github.com/ZurrTum/Create-Fly/issues/357)
Until this is resolved, I will be implementing the mentioned workaround that disables GPU rendering, however I don't want to ship this modpack until a solution is found because of the potential performance issues. when that happens, re-test shaders for compatibility.
IT'S HAPPENING OH GOD lmao uh oh. uh ohhhh
photon can be patched (photon 1.3a) but there's also [this](https://github.com/djefrey/photon) fork that keeps compat with voxy (maybe even DH is exclusive to this?) though its 5 months out of date from main
"**Tip**: it's common for shaderpacks to disable Entity Shadows or Block Entity Shadows by default. Make sure that those options are toggled if you want Create contraptions to cast lights and shadows (and don't forget to toggle the required options for light casting in the shaderpack settings !)."

[dadget's animal villagers nesting issue](https://github.com/draklorx/animalkin_villagers/issues/2)
once this is merged i can remove the fix from my own surface-level pack

fancymenu is shitting itself with Wakes. wait for wakes author to fix and then reinstate it (then i have to tell fancymenu guy to take away the incompat marker)

#### It's just cooked (becomes 'known issues')

coniferous badlands appear much more wooded in LODs than they actually are, similar issues for icebergs and eroded badlands and some structures, it just is what it is.

Air Gap Fix not working on Create blocks is a shame but create being what it is, and create fly being a fork, I don't think it's even worth reporting the issue considering I don't know precisely the problem.

Snowy leaves mod not playing nice with world generation for some reason. the author is as befuddled as I am. I don't expect a fix any time soon.
### Git/Modrinth/Version Management

Basically use Git to store listing and information but not whole mods or resourcepacks so as not to break terms.

[the git](https://github.com/123happily/Create-Lemonade)
how to push to git
git add .
git commit -m "commit name"
git push -u origin main

sick
i've never used git before
please be kind

https://gist.github.com/jeffjohnson9046/80bc182db7ae2f4a6150
my dumbass needs this

When you export from Prism, selecting the folders i.e mods, resourcepacks correctly converts them to Modrinth dependencies instead of packaging the raw files, or at least it does something close enough.

I have to zip my datapack before distributing, but my resource pack seems to make it through unharmed, which is nice. Yeah basically it modrinth links everything it can and then adds anything it couldn't as files. Nice.
### Pack Resource and Data Pack
#### Wikiful

This goes across the datapack and the resource pack actually.
wikiful's stuff is in data/lemonade/ etc etc. here's the guide on how to do that https://github.com/Apollounknowndev/wikiful/wiki

it also references icons i'm putting in the respack at assets/lemonade/textures/gui/sprites/...

this is great and ideally i can mostly bin the wiki here and just keep this page.
#### Biome Coloration - on hold... DH being annoying...
I can adjust biome-based sky, leaf, grass, and other foliage colors, and [more](https://github.com/MehVahdJukaar/polytone/wiki/Environment-Attributes), so it's probably ideal to keep track of what I've been up to...

Oak leaves for some reason eats the biome-based simple configurations alive, so I can't really use a full colormap for those. Everything else is fair game though.

I got permission to overwrite rainbow foliage's textures (see that section in aesthetics > rendering > leaves section for more information) so I'll be brightening leaves to have full control over their colour!

I've also put leaf litter under the 'foliage color' map (which is mainly for oak) decided by the biome property files. It just feels a bit easier. i can always go back and give it its own colormap if i give a shit later.

TO DO:
- update acacia, dark oak, jungle, mangrove textures to be 'bright'
- change birch default to something slightly darker for sanity
- set up their colormaps since we're knuckling down on this idea again
- run through biomes and nail down looks for them, testing with all leaves and litter for anything horrendous

Clifftree's Snowy Old Growth Taiga is a frosty blue.
Taiga is a rich green.

#### Villager Trade Rebalance - My Version

Changes are inspired by the vanilla [Villager Trade Rebalance](https://minecraft.wiki/w/Villager_Trade_Rebalance) datapack.
note that enchanted items are removed from villager pools by Enchancement. books are still sold but aren't villagertype specific, see what you can do.
#### Other Changes

I've made it so that Ruined Portals never spawn underground, effectively doubling their above-ground spawn rate, partly because I think it's cool, and partly because I have half a mind to incentivise lighting nether portals exclusively in RP frames.

## stuff i might throw in later

#### worldgen musings

I want some more structures maybe? But almost all of the mods are doing way too much
#### Gameplay

https://modrinth.com/mod/create-display-regex/gallery
not sure if its chinese when you load it

https://modrinth.com/mod/create-fly-recipe-viewer/gallery
do create fly recipes really not show in jei? they do but... look bad. mm

afaik there's no way to automatically set up a creative copy of a world, the best i could do is write wiki instructions on how to get started and then have some advancements that only trigger once you're in creative mode to explain the rest.

good leaf decay mod
https://modrinth.com/mod/leaves-us-in-peace

good if you hate maths
https://modrinth.com/mod/total-yield

Pet Changes Potentially
https://modrinth.com/mod/ppetp fixes long range teleport/stuck in unloaded chunks without performance hit (nice)
https://modrinth.com/mod/respawnable-pets adds item to mark pets as respawnable with you on sleep. no clue if it works consecutively
https://modrinth.com/mod/indypets gives pets a third roaming mode aside from just following and sitting

https://modrinth.com/mod/reliable-requiem
VERY comprehensive death penalty- WHOAH. penalties-upon-death mod
#### bugfix/util

https://modrinth.com/mod/forceexitonshutdown
need

https://github.com/D3ADK1LLSH0T/config-presets
this would be an absolute GODSEND if it was updated to 26.2. GOD. SEND. i'm following it twice lol.

definitely that thing that smartly compacts logs
https://modrinth.com/mod/log-cleaner thats a start
https://modrinth.com/mod/asynclogger not close, but still probably worth
#### graphics

more paintings would be cool

cloud respacks
https://modrinth.com/resourcepack/fluffy-fancy-clouds

'shader' respacks
https://modrinth.com/resourcepack/rey-shaders
https://modrinth.com/resourcepack/rsrp/gallery
https://modrinth.com/resourcepack/nexus-shaders/gallery no way it works
https://modrinth.com/resourcepack/outlines-contours, https://modrinth.com/resourcepack/light-outlinethe outline ones. maybe try to port. first one looks lowkey bad but thats ok. second one might actually work
https://modrinth.com/mod/cinematic-villa description scares me
https://modrinth.com/resourcepack/chunk-tweaks funi
https://modrinth.com/resourcepack/realistic-night-vision sick
https://modrinth.com/resourcepack/atmospheric-er-atmosphere/gallery inchresting
https://modrinth.com/resourcepack/no-shade-%2B-fps-boost similar to shadify
https://modrinth.com/resourcepack/blush/gallery pls
https://modrinth.com/resourcepack/neoshade/gallery they might be cooking
https://modrinth.com/shader/energy-shaders-java
https://modrinth.com/resourcepack/colored-lights-plus
https://modrinth.com/resourcepack/hue-shift-shading apparently works
https://modrinth.com/resourcepack/notvisuals try
https://modrinth.com/resourcepack/fast-gateway/gallery lmao what

https://modrinth.com/resourcepack/leaves-and-niddles might work

https://modrinth.com/resourcepack/vibrant-fog/gallery recommended to use with DH

ore shine animation that isnt emissive by default (sexy) no create
https://modrinth.com/resourcepack/spryzeens-ore-glint

emissive particles test if needed prolly wont work on modded particles
https://modrinth.com/resourcepack/emissive%2Bparticles

makes stuff shiny probably quite not performant tho no clue shader compat
https://modrinth.com/resourcepack/blooming-blocks/gallery

https://modrinth.com/resourcepack/enchantment-glint-normalization
crazy that this is even needed

punchy/hyper punchy
i'm just unsure how it'll feel. will probably need create skyhook compat whatever whatever

respack for the vanilla enchanted books that actually works

## thoughts

I do want to enable the automation of *most stuff* in the game through either Create or non-ugly Vanilla methods. That means getting a full list of items and blocks (including create's) and culling it down - first removing anything that's just a combination of other stuff, and then interrogating the sources of the remaining stuff.

featurify hopefully lets you disable pockets of lava in the nether.

I'd like to use the difficulties a bit smarter...

also maybe grab something to balance mobs. i'm thinking:
no surface mob spawns, only caves/under blocks
limit to spawning in an area...?
weaker skeletons
weaker baby zombies
weaker vexes
alternative sources of some drops

i'm not done fixing snow. snow on stairs and slabs would be great. snow settings might help here. even snow on grass, somehow.

I  want to make the end less of a headache. not dying in the void is a start, but i'm not sure if that mod is ideal cause i think you can get softlocked LMAO you could try 'NoVoid' instead which is the same idea.
otherwise increasing the rarity of end cities with structurify
shulker drops two and respawning shulkers - make the former a guaranteed 2 drop and the latter a very long timer. this makes getting shulker boxes much easier.
some tweaks to the elytra to make it less OP for long distances might be good. (Though I *did* say i wouldn't nerf it...) there's just more support for it out there. i think i'll put elytra bounce, airbrake, and a rocket debuff on it with elytra tuning
then it can be visually improved with contrails and trims and physics and bonk mod lmao

Enchanting is getting an overhaul... enchancement is seemingly alright with some config though i've had issues with its simultaneous enchantment cap. I'd like it to be 2... if only cause there's a lot of inventory clutter otherwise.
easy magic lets you put decoration around the table and keeps items in it with a cool graphic... idk if it'll work, we'll see. [this](https://modrinth.com/datapack/purpurpacks-transparent-blocks-in-enchant-area) is an alternative

# Modules
### Info
All of the mods, resource packs, and shaders are detailed here, organised into Modules based on their function.

Crediting:
The relevant link, author, license, and current state of inclusion in this pack are also noted.
For more information on licenses, see [here](https://modpack-dev-knowledgebase.github.io/modpack-dev-wiki/wiki/info/licenses/) and [here](https://www.tldrlegal.com/). Note that even ARR-licensed projects hosted on Modrinth waive their right to exclusion from modpacks per [Modrinth's Terms of Use](https://modrinth.com/legal/terms), but I will respect explicit requests for exclusion or removal where present. Please [[Contact Me\|contact me]] if you want to discuss how your work is included in this pack, or if I've made any mistakes.

Please note: This modpack is distributed with a built-in resource pack that duplicates and reorganises many assets found in other resource packs. This pack will not be distributed outside of this modpack. All original resource packs are still included in the pack so they will recieve proper crediting and download counts. Please reach out if you have any issues with this approach. Textures are not heavily modified, they are mainly renamed and their file structures changed so that they can function correctly on 26.2.

As of current, I'm planning to license this pack under GPL due to the "Viral" nature of that license and my inclusion of content using it, or similar, licensing. I'm led to believe that using LGPL projects within a GPL pack is permissable via the license, but if I am wrong on that front, please contact me!

Sections will be marked with :LiBadgeCheck: once they are unlikely to require further work. Or just... good enough for now and I should stop thinking about them.

I'm also including a list of mods at the end that *aren't* included and why.

## Create
*The core focus of the pack, thanks to Create Fly.*

[Create Fly](https://modrinth.com/mod/create-fly)
Author: ZurrTum
Type: Mod
License: CC0-1.0
Purpose in Pack: Higher-version port of Create
Status: Added

[Create - Steam n Rails Fly Port](https://modrinth.com/mod/create-fly-steam-n-rails-continued)
Author: Cat4blep
Type: Mod
License: GPL-3.0-only
Purpose in Pack: Add the features of Steam 'n' Rails
Status: Added

[Create: Fluid Burner (Fly)](https://modrinth.com/mod/create-fluid-burner)
Author: frikinjay
Type: Mod
License: JGPL-3.0-only
Purpose in Pack: Allow Blaze Burners to take fuel in the form of lava directly from pipes.
Status: Added

[Create: Refabricated Recipes](https://modrinth.com/mod/create-refabricated-recipes)
Author: tunamayo2141
Type: Mod
License: MIT
Purpose in Pack: Enable more automation
Status: Added
## Balance
*Lowering the difficulty to let you focus on expanding your factory*

[Enchancement](https://modrinth.com/mod/enchancement)
Author: MoriyaShiine, cybercat5555, RAT, EightSidedSquare, Up
Type: Mod
License: ARR
Purpose in Pack: A radical approach to enchanting that adds enchantments, changes dynamics, balances things, removes tool durability, and fixes bugs.
Status: Added
*Heavily configured to remove some nerfing behaviour for the purposes of this pack*

[Easy Mob Spawn Control](https://modrinth.com/mod/easy-mob-spawn-control)
Author: Catomon
Type: Mod
License: ARR
Purpose in Pack: Lets me alter spawn rates, conditions, and drops
Status: Added

[Custom Mob Attributes](https://modrinth.com/plugin/custom-mob-attributes)
Author: Fneifnox
Type: Mod
License: [Custom License](https://pastebin.com/E6MB5nZG) (this site shows weird ads, be warned, not Fneifnox's fault)
Purpose in Pack: Lets me alter the health, speed, size, and damage of certain mobs.
Status: Added

[Adult Zombies Only](https://modrinth.com/datapack/azo)
Author: sniffercraft34
Type: Mod
License: MIT
Purpose in Pack: Partly because of texture reasons, but mainly for gameplay reasons, we shall have no baby zombies (their spawns are replaced with adult forms).
Status: Added

[Mob Explosion Griefing Gamerule](https://modrinth.com/mod/mobexplosiongriefinggamerule)
Author: Enecske
Type: Mod
License: MIT
Purpose in Pack: Don't let creepers or endermen ruin your hard work! And stop zombies from going out of their way to crush turtle eggs. They might still do it on accident.
Status: Added

[0,5 HP](https://modrinth.com/datapack/0%2C5-hp)
Author: BizCub
Type: Mod
License: MIT
Purpose in Pack: You will survive all fall damage with half a heart.
Status: Added
## QoL
*Making things easier, making the pack work, with as few nerfs as possible*

[Just Enough Items](https://modrinth.com/mod/jei)
Author: mezz
Type: Mod
License: MIT
Purpose in Pack: View recipes, including Create's
Status: Added

[Easy Shulker Boxes](https://modrinth.com/mod/easy-shulker-boxes)
Author: Fuzs, LunaPixelStudios
Type: Mod
License: MPL-2.0
Purpose in Pack: Make it far easier to interact with shulker boxes
Status: Added

[SilkTouch+](https://modrinth.com/mod/silktouch%2B)
Author: Wheeler-Shigley
Type: Mod
License: GPL-3.0-or-later
Purpose in Pack: Allow you to silk-touch spawners, budding amethyst, and more.
Status: Added

[Call Your Happy Ghast](https://modrinth.com/datapack/call-your-happy-ghast), [Horse](https://modrinth.com/datapack/call-your-horse), and [Nautilus](https://modrinth.com/datapack/call-your-nautilus)
Author: Jodek
Type: Mod
License: MIT
Purpose in Pack: Summon a named mount with a linked Goat Horn from anywhere - even unloaded chunks!
Status: Added
*Make sure to leash entities to the Happy Ghast starting with the Happy Ghast side, and they'll be teleported too!*

[Faster Happy Ghast (FHG)](https://modrinth.com/datapack/faster-happy-ghast-fhg)
Author: Jom3a
Type: Mod
License: MIT
Purpose in Pack: Speeds up the Happy Ghast and lets you sprint with it!
Status: Added

[Small Netherite Beacons](https://modrinth.com/mod/small-netherite-beacons)
Author: bsharou
Type: Mod
License: MIT
Purpose in Pack: Sub in a netherite block under a beacon instead of having to build a full size beacon base.
Status: Added

[Enhanced Netherite Armour](https://modrinth.com/mod/enhanced-netherite-armour)
Author: SwordfishBE
Type: Mod
License: AGPL-3.0-or-later
Purpose in Pack: Gives you fire resistance when you have a full set of Netherite Armour - and it works for horse armour too (they float on lava)
Status: Added

[Harou's Netherite Shulkers](https://modrinth.com/mod/harous-netherite-shulkers)
Author: bsharou
Type: Mod
License: MIT
Purpose in Pack: Upgrade your shulker box with netherite to make it fire- and blast- proof.
Status: Added

[Blasting Plus](https://modrinth.com/datapack/blasting-plus) and [Smoking Plus](https://modrinth.com/datapack/smoking-plus)
Author: greenclaw
Type: Mod
License: GPL-3.0-only
Purpose in Pack: Make more Vanilla smelting recipes work in the Blast Furnace and Smoker.
Status: Added

[Biome Spreader](https://modrinth.com/mod/biome-spreader)
Author: Masy
Type: Mod
License: GPL-3.0-only
Purpose in Pack: Allows the crafting of potions that let you change the biome in a radius, handy for builders who want to have more control over their world
Status: Added
*Doesn't support modded biomes*

[1.16.1 Ender Pearl Rates](https://modrinth.com/mod/1.16.1-ender-pearl-rates) (A.K.A. Old Pearl Bartering)
Author: TJOAT
Type: Mod
License: MIT
Purpose in Pack: Makes Ender Pearls a more common result from bartering.
Status: Added

[Air Gap Fix](https://modrinth.com/datapack/air-gap-fix)
Author: Gurkis
Type: Mod
License: ARR
Purpose in Pack: Prompts fences, walls, glass panes, and bars to connect to more non-solid or partial blocks like banners and signs.
Status: Added
*Doesn't work with Create's building blocks, this is a 'better than nothing' situation. Make sure you're facing dead-on to the target block for this to work.*

[Mouse Tweaks](https://modrinth.com/mod/mouse-tweaks)
Author: YaLTeR
Type: Mod
License: BSD-3-Clause
Purpose in Pack: Add many QoL features to mouse inventory interactions
Status: Added

[Trinkets Updated](https://modrinth.com/mod/trinkets-updated)
Author: Patbox
Type: Mod
License: MIT
Purpose in Pack: Allow the use of trinket slots
Status: Added

[Trinkets Lantern Support](https://modrinth.com/datapack/trinkets-lantern-support)
Author: Patbox
Type: Mod
License: MIT
Purpose in Pack: Let you hang lanterns on your hip to make full use of Dynamic Lights.
Status: Added

[Ok Zoomer](https://modrinth.com/mod/ok-zoomer)
Author: Ennui
Type: Mod
License: ARR
Purpose in Pack: Highly configurable zoom mod. Will be gated to the posession of a spyglass and used with the following mod.
Status: Added

[Ok Zoomer Spyglass Slot](https://modrinth.com/mod/spyglass-trinket-slot)
Author: MinecraftGuy926
Type: Mod
License: MIT
Purpose in Pack: Gives you a spot to hold your spyglass
Status: Added

[Trinkets Elytra](https://modrinth.com/datapack/trinkets-elytra)
Author: greezlu
Type: Mod
License: MIT
Purpose in Pack: Let you wear a chestplate and elytra at the same time.
Status: Added

[Stretchy Leash](https://modrinth.com/mod/stretchy-leash)
Author: Estecka
Type: Mod
License: MIT
Purpose in Pack: Let leashes stretch more before breaking, and give led entities a step-height boost.
Status: Added
*Works so well I couldn't even get a leash to break!*

[Instant Portal Nether](https://modrinth.com/mod/instant-portal-nether) (A.K.A. Instant Nether Portal)
Author: JeanGomez
Type: Mod
License: MIT
Purpose in Pack: No more waiting 4 seconds to travel through the nether portal.
Status: Added

[Better Days](https://modrinth.com/mod/betterdays)
Author: wendall911
Type: Mod
License: LGPL-3.0-or-later
Purpose in Pack: Make days and nights a solid 20 minutes each, and lets you go to sleep a little earlier (per my config - this mod can do a lot more!)
Status: Added

[SleepWarp (Updated)](https://modrinth.com/mod/sleep-warp-updated)
Author: Patbox, Giggitybyte
Type: Mod
License: MPL-2.0
Purpose in Pack: Tick the game as you sleep so that furnaces process and crops grow. Watch the moon set and the sun rise. Makes sleeping take a little longer, but rewards you for it, instead of phantoms punishing you for not doing it.
Status: Added
## Aesthetics :LiStarHalf:
*Simple, stylistic flair and atmosphere, unified with the Create aesthetic.*
#### **Menus**

[Fancy Menu](https://modrinth.com/mod/fancymenu)
Author: Keksuccino
Type: Mod
License: DSMSLv3.1
Purpose in Pack: Allow extensive customisation of the main menu (and more!)
Status: Added
*Control + Alt + C brings up the configuration menu!*

[Fancy Toasts | Better Advancements](https://modrinth.com/mod/fancy-toasts)
Author: Bivrik
Type: Mod
License: MIT
Purpose in Pack: Greatly improve the look of advancements, customisable with resource packs.
Status: Added

[Reese's Sodium Options](https://modrinth.com/mod/reeses-sodium-options)
Author: FlashyReese
Type: Mod
License: MIT
Purpose in Pack: I'm more familiar with this layout. Feel free to remove if you don't like it.
Status: Added

[Inventory Blur](https://modrinth.com/mod/inventory-blur)
Author: enchanted-games
Type: Mod
License: CC-BY-NC-4.0
Purpose in Pack: Add a blur behind inventories.
Status: Added

[Smooth Scrolling](https://modrinth.com/mod/smooth-scroll)
Author: SmajloSlovakian
Type: Mod
License: GPL-3.0-only
Purpose in Pack: Make scrolling smooth in many menus
Status: Added
*Had to disable Sound's hotbar scrolling sounds because it was going for way too long with this mod enabled lol*

[Smooth Swapping](https://modrinth.com/mod/smooth-swapping)
Author: Schauweg, Riflusso
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Makes moving items in inventories look smooth!
Status: Added

[Raised](https://modrinth.com/mod/raised)
Author: yurisuika
Type: Mod
License: LGPL-3.0-or-later
Purpose in Pack: Lifts the hotbar off the bottom of the screen.
Status: Added

[Fresh Hearts](https://modrinth.com/resourcepack/fresh-hearts)
Author: navzary
Type: Resource Pack
License: ARR
Purpose in Pack: Make the hearts look a little nicer
Status: Added

[Hidden Recipe Book](https://modrinth.com/mod/hidden-recipe-book)
Author: Serilium
Type: Mod
License: ARR
Purpose in Pack: Hide the unneeded recipe book to encourage use of JEI!
Status: Added

[Clearer Slot Highlight](https://modrinth.com/resourcepack/clearer-slot-highlight)
Author: blockerlocker
Type: Resource Pack
License: MIT
Purpose in Pack: Puts the item highlight behind the item so it's easier to look at
Status: Added

[Better Advancements](https://modrinth.com/mod/better-advancements)
Author: way2muchnoise
Type: Mod
License: Dont Be a Jerk
Purpose in Pack: Improves the Advancements menu, which will be the main progression guide in this modpack.
Status: Added

[Plane Advancements](https://modrinth.com/mod/plane-advancements)
Author: Nettakrim
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Change the layout of advancements to avoid a strange bug where Create's went off-screen + add some cool dynamic mind-map dynamics to them.
Status: Added

[Dynamic Crosshair](https://modrinth.com/mod/dynamiccrosshair)
Author: Crendgrim
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Dynamically hide and change the crosshair depending on what you're looking at - or not looking at.
Status: Added

[Auto HUD](https://modrinth.com/mod/autohud)
Author: Crendgrim
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Hides the hotbar when it's not in use for a cleaner look.
Status: Added

[Day Counter](https://modrinth.com/mod/mc-day-counter)
Author: 02Alexis
Type: Mod
License: [Custom](https://github.com/02A1exis/02A1exis/blob/main/licenses/protective-license.md)
Purpose in Pack: Keep track of the days with a typewriter-ish counter each morning, and celebrate big milestones with sfx.
Status: Added

[Create Style Interface](https://modrinth.com/resourcepack/create-style-interface)
Author: ogabasferr
Type: Resource Pack
License: ARR
Purpose in Pack: Unify the Vanilla interfaces to be Create-themed.
Status: Added
*Many assets required copy-pasting into the modpack's resource pack to work on 26.2. I'd like to let the original pack set the textures, but for now this is the best I can do.*

[Reliable Recount](https://modrinth.com/mod/o123456789-backport) (aka O123456789)
Author: evanbones
Type: Mod
License: GPL-3.0-or-later
Purpose in Pack: Styles item numbers in Create's format/font
Status: Added
*Kindly updated to 26.2 from my request!*

[VUL's Create Cursors](https://modrinth.com/resourcepack/vuls-create-cursors)
Author: avizvul42
Type: Resource Pack
License: MIT
Purpose in Pack: Change the cursor to be Create-themed. Ported to work with Cursors Extended on 26.2 using [this tool](https://fishstiz.github.io/cursors_extended-wiki/tools/#v3-converter).
Status: Added

[Capitalized Shaded Font](https://modrinth.com/resourcepack/capitalized-shaded-font)
Author: NOEMA, Ferrlius, medn1y
Type: Resource Pack
License: ARR
Purpose in Pack: Adds a really nice font.
Status: Added

#### **Sounds** 

[Sounds](https://modrinth.com/mod/sound)
Author: IMB11
Type: Mod
License: ARR
Purpose in Pack: Improve item, UI, and block sounds.
Status: Added

[Sound Physics Remastered](https://modrinth.com/mod/sound-physics-remastered)
Author: henkelmax
Type: Mod
License: GPL-3.0-only
Purpose in Pack: Add reverb and echo to all sounds
Status: Added
*Reverb quality and volume/intensity will be tweaked for performance and preference reasons*

[Ambient Sounds](https://modrinth.com/mod/ambientsounds)
Author: creativemd
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Add nice ambience to environments
Status: Added
*Overall volume will be lowered, and particularly overwhelming tracks may also be lowered*

[Cool Rain](https://modrinth.com/mod/coolrain)
Author: Jaiz
Type: Mod
License: ARR
Purpose in Pack: Dynamic, block-based rain sounds for nice ambience.
Status: Added
*Any non-block related sounds will be disabled in favour of ambient sounds*

[Presence Footsteps Lite](https://modrinth.com/mod/presence-footsteps-lite)
Author: amiralimollaei
Type: Mod
License: MIT
Purpose in Pack: Make your footsteps sound much better. Fork with slightly less features, and therefore, dependencies, for simplicity.
Status: Added

[Raise Sound Limit Simplified](https://modrinth.com/mod/rsls)
Author: ishland
Type: Mod
License: MIT
Purpose in Pack: Make the sound engine perform better and have more capability.
Status: Added

[Silence villager](https://modrinth.com/resourcepack/silence-villager)
Author: VayLorn
Type: Resource Pack
License: ARR
Purpose in Pack: Makes villagers silent aside from trading
Status: Added
#### **General Rendering :LiStarHalf:**

##### **Setup**

[Iris](https://modrinth.com/mod/iris)
Author: coderbot, IMS
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Enable the use of shaders, and provide some performance boost.
Status: Added

[Better Biome Blend](https://modrinth.com/mod/better-biome-blend)
Author: FionaTheMortal
Type: Mod
License: Unlicense
Purpose in Pack: Speed up and greatly increase biome blend radius for smoother biome transitions.
Status: Added
*Note: I will probably shrink the blend distance.*

[Polytone](https://modrinth.com/mod/polytone)
Author: MedVahdJukaar
Type: Mod
License: GPL-3.0-or-later
Purpose in Pack: Enable the use of resource packs that rely on Polytone's wide range of features.
Status: Added

[Fusion](https://modrinth.com/mod/fusion-connected-textures)
Author: SuperMartijn642
Type: Mod
License: ARR
Purpose in Pack: Enable the use of Fusion-formatted resource packs.
Status: Added

[Continuity](https://modrinth.com/mod/continuity)
Author: Pepper_Bell
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Enable the use of Continuity (Optifine) - formatted resource packs.
Status: Added

[Respackopts](https://modrinth.com/mod/respackopts)
Author: JFronny
Type: Mod
License: MIT
Purpose in Pack: Allow configuring of resource packs that support this format.
Status: Added

[EMF](https://modrinth.com/mod/entity-model-features) and [ETF](https://modrinth.com/mod/entitytexturefeatures)
Author: Traben
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Support Fresh Animations among other things
Status: Added

[Cursors Extended](https://modrinth.com/mod/minecraft-cursor)
Author: fishstiz
Type: Mod
License: MIT
Purpose in Pack: Enable the use of custom cursors.
Status: Added

(This is where I'd put my Colorwheel. If I had one)

##### **Particles**

[Particle Rain](https://modrinth.com/mod/particle-rain)
Author: PigCart
Type: Mod
License: MIT
Purpose in Pack: Greatly improve the look of rain
Status: Added
*Configured to remove all sounds and slightly lower the intensity. Also disabled 'dust haze' for aesthetic reasons.*

[Subtle Effects](https://modrinth.com/mod/subtle-effects)
Author: MinecraftEinstein, TheEnderCore
Type: Mod
License: ARR
Purpose in Pack: Add more effects. Also fades out night vision, lowers fire overlay, somewhat clears fire overlay when you have fire resistance, somewhat clears potion particle opacity based on distance to player, and more.
Status: Added
*Many effects that I feel don't suit the look or are too intrusive have been disabled. Others have been reduced in intensity or likelihood. Will disable 'allow using blended render type' if issues around particle transparency occur. Particle culling has been disabled to reduce issues with existing particle culling mods. Some features, like the splahes, waterfalls, and fireflies, have been given to Particular.*

[Particular](https://modrinth.com/mod/particular-reforged)
Author: Leclowndu93150
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: The primary contributer of particle effects due to its vanilla-friendly pixellated look. Further particle mods will have their overlapping features disabled.
Status: Added
*Features similar to Subtle Effects will be disabled to prevent overlap aside from those mentioned above.*

[Windy](https://modrinth.com/mod/windy)
Author: Bonfire Studios
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Just adds little curls of wind. Very charming.
Status: Added

[Particle Effects](https://modrinth.com/mod/particle-effects)
Author: K-TEAM, KlashRaick, LopyMine
Type: Mod
License: CC-BY-ND-4.0
Purpose in Pack: Allows resource packs to specify particles for each kind of potion/effect
Status: Added

[Particles Updates](https://modrinth.com/resourcepack/particles-updated)
Author: zCore, zdkrr
Type: Resource Pack
License: CC-BY-NC-SA-4.0
Purpose in Pack: A resource pack for the aforementioned Particle Effects
Status: Added

##### **Animations**

[Fresh Animations](https://modrinth.com/mod/packed-packs)
Author: FreshLX
Type: Resource Pack
License: (Custom Terms of Use) + Explicit Modpack Permission Given
Purpose in Pack: Animate mobs in a whimsical style
Status: Added

[Spawn Animations](https://modrinth.com/datapack/spawn-animations)
Author: Tschipcraft
Type: Mod
License: Custom License
Purpose in Pack: Give mobs cool animations when they spawn in.
Status: Added

[Fresh Animations: Objects](https://modrinth.com/resourcepack/fresh-animations-objects)
Author: FreshLX
Type: Resource Pack
License: ARR
Purpose in Pack: Animate chests, boats, and shulkers
Status: Added

[Animated Items (emissive)](https://modrinth.com/resourcepack/animated-item-textures)
Author: shivaklans
Type: Resource Pack
License: ARR
Purpose in Pack: Animate some inventory items
Status: Added
*Note: emission isn't working, I'll come back and look at that later*
##### **Emission, Shading and Lighting**

[Fresh Animations: Emissive](https://modrinth.com/resourcepack/fresh-animations-emissive)
Author: FreshLX
Type: Resource Pack
License: (Custom Terms of Use) + Explicit Modpack Permission Given
Purpose in Pack: Add glowing textures to some mobs
Status: Added

[LambDynamicLights](https://modrinth.com/mod/lambdynamiclights)
Author: LambdAurora
Type: Mod
License: Lambda License
Purpose in Pack: Make glowing things cast light around them
Status: Added

[Glowix](https://modrinth.com/resourcepack/glowix)
Author: CreepyWe
Type: Resource Pack
License: ARR
Purpose in Pack: Add emission to some blocks
Status: Added
*Glowing ores are off by default - turn them on if you prefer that!*

##### **Overlays Etc**

[Overlay's](https://modrinth.com/resourcepack/overlays)
Author: itzSandw
Type: Resource Pack
License: Custom EULA
Purpose in Pack: Enable cool transitions between blocks
Status: Added
*I made the Respackopts integration for this even though it's Bad 😎*

[Glowy Nether Portals](https://modrinth.com/resourcepack/glowy-nether-portals)
Author: zpez
Type: Resource Pack
License: ARR
Purpose in Pack: Make nether portals look cooler
Status: Added

[Snow & Moss Overhangs](https://modrinth.com/resourcepack/snow-and-moss-overhangs)
Author: Devoxxel
Type: Resource Pack
License: MIT
Purpose in Pack: Make snow and moss layers overlay onto blocks below them.
Status: Added
##### **Mobs**

[3D Harnesses x Fresh Animations](https://modrinth.com/resourcepack/3d-harnesses-x-fresh-animations)
Author: Mtcd
Type: Resource Pack
License: CC-BY-SA-4.0
Purpose in Pack: Make the happy ghast harnesses look a little better.
Status: Added

[Freshly Creepers](https://modrinth.com/resourcepack/freshly-creepers)
Author: Eianex
Type: Resource Pack
License: MIT
Purpose in Pack: FA-compatible creeper redesign
Status: Added

[Hellay's Redone Endermans](https://modrinth.com/resourcepack/redone-endermans) & [X Fresh Animations](https://modrinth.com/resourcepack/redone-endermans-fa)
Author: \_Hellay
Type: Resource Pack
License: ARR
Purpose in Pack: Make endermen glow and look cooler
Status: Added

[Glowing Ender Dragon](https://modrinth.com/resourcepack/glowing-ender-dragon)
Author: Eianex
Type: Resource Pack
License: MIT
Purpose in Pack: Make the ender dragon glow and look cooler
Status: Added
*I made a duplicate of this in the modpack resource pack to make the emission work a little better and stop z-fighting*

[ButterBee x Fresh Animations](https://modrinth.com/resourcepack/butterbee-fresh)
Author: Konci
Type: Resource Pack
License: CC-BY-NC-SA-4.0
Purpose in Pack: FA support for ButterBee's Mob Variants
Status: Added

(Optional) [Arachnophobia Mode](https://modrinth.com/resourcepack/arachnophobia-mode-red-text)
Author: Maxsteelbro
Type: Resource Pack
License: MIT
Purpose in Pack: Give users the option to turn spiders into floating bits of text that just say 'spider' (inspired by Lethal Company)
Status: Added

[Dadget's Animal Villagers](https://modrinth.com/resourcepack/dadgets-animal-villagers)
Author: Dadget
Type: Resource Pack
License: Apache-2.0
Purpose in Pack: Change villagers from a weird stereotype to cute animals!
Status: Added

[Dadget's Animal Villagers + Fresh Animations](https://modrinth.com/resourcepack/dadgets-animal-villagers-%2B-fresh-animations)
Author: Dadget
Type: Resource Pack
License: ARR
Purpose in Pack: Self explanatory
Status: Added

[Beastial](https://modrinth.com/resourcepack/beastial)
Author: Hahchek
Type: Resource Pack
License: CC-BY-4.0
Purpose in Pack: Sit underneath Dadget's Animal Villager in the load order, and provide textures for witches and illagers
Status: Added

[Beastial -Fresh Animations Patch-](https://modrinth.com/resourcepack/beastial-fresh-animations-patch-)
Author: Hahchek
Type: Resource Pack
License: CC-BY-4.0
Purpose in Pack: Self explanatory
Status: Added

[Boy Why You So Ears](https://modrinth.com/resourcepack/boy-why-you-so-ears)
Author: JBCC
Type: Resource Pack
License: CC0-1.0
Purpose in Pack: Improves the spotted wolf to have big ears!
Status: Added

[Fresh Animations Patch - Boy Why You So Ears](https://modrinth.com/resourcepack/fresh-boy-why-you-so-ears)
Author: Dasawkem
Type: Resource Pack
License: CC0-1.0
Purpose in Pack: Self explanatory
Status: Added
##### **Items**

[Fusion Stacking Items](https://modrinth.com/resourcepack/fusion-stacking-items)
Author: SuperMartijn642
Type: Resource Pack
License: ARR
Purpose in Pack: Make inventories more interesting with amount-concious item textures
Status: Added

[Unique Goat Horns](https://modrinth.com/resourcepack/unique-goat-horns)
Author: Cubeoidal
Type: Resource Pack
License: CC-BY-NC-SA-4.0
Purpose in Pack: Make the goat horns look different
Status: Added

[Bray's Better Bow & Arrows](https://modrinth.com/resourcepack/brays-better-3d-bow)
Author: Braytonks
Type: Resource Pack
License: ARR
Purpose in Pack: Improve the look of bows and crossbows.
Status: Added

[Axolotl Buckets](https://modrinth.com/mod/axolotl-buckets)
Author: Roundaround
Type: Mod
License: MIT
Purpose in Pack: Display axolotls in buckets correctly
Status: Added

[Enchanced Books](https://modrinth.com/resourcepack/enchanced-books)
Author: teaddino
Type: Resource Pack
License: MIT
Purpose in Pack: Custom textures for Enchancements' books
Status: Added

[xali's Enchanted Books](https://modrinth.com/resourcepack/xalis-enchanted-books)
Author: xalixilax
Type: Resource Pack
License: CC-BY-NC-4.0
Purpose in Pack: Make enchanted books visually distinguishable and cool
Status: Added
*Note: A custom enchanted_book.json was created to merge this properly with the Enchanced Books resource pack; no pack files were directly modified and all download credits will still apply correctly.*

[xali's Enchanted Books - Create Addon](https://modrinth.com/resourcepack/xalis-enchanted-books-create-addon)
Author: Dimtility
Type: Resource Pack
License: CC-BY-NC-4.0
Purpose in Pack: Add custom textures for Create's enchantments
Status: Added
*Note: A similar process was used here, including adding model files to make it work on newer versions as opposed to just old version CIT/Optifine format. No texture files were reproduced and all download credits will still apply correctly.*
##### **Blocks**

[Better Enchanting Table](https://modrinth.com/resourcepack/better-enchanting-table)
Author: Jacosvaldo
Type: Resource Pack
License: CC-BY-NC-SA-4.0
Purpose in Pack: Make the enchanting table look better and glow.
Status: Added

[Beta Beacon](https://modrinth.com/resourcepack/beta-beacon)
Author: miau_the_cat
Type: Resource Pack
License: MIT
Purpose in Pack: Make beacons look a bit nicer.
Status: Added

[Glowing End Portal](https://modrinth.com/resourcepack/glowing-end-portal)
Author: AnolXD
Type: Resource Pack
License: ARR
Purpose in Pack: Makes ender portal frames look nicer
Status: Added
##### **Grass/Leaves/Plants/Ground Cover :LiStarHalf:**

[Better Snow Coverage](https://modrinth.com/mod/better-snow-coverage)
Author: ToBinio
Type: Mod
License: MIT
Purpose in Pack: Greatly improve the appearance of snow biomes by rendering fake snow layers in partial blocks that don't currently allow it.
Status: Added

[Better Snowy Leaves](https://modrinth.com/mod/better-snowy-leaves)
Author: fabiofdez
Type: Mod
License: CC0-1.0
Purpose in Pack: Improve the look of leaves in snowy biomes.
Status: Added

[Mossy's Better Dirt](https://modrinth.com/resourcepack/mossys-better-dirt)
Author: pixelmossy
Type: Resource Pack
License: ARR
Purpose in Pack: Bring dirt's texture up-to-date with modern Minecraft
Status: Added

[Rainbow's Foliage](https://modrinth.com/resourcepack/rainbows-foliage)
Author: PoeticRainbow
Type: Resource Pack
License: ARR
Purpose in Pack: Improve the fluffy look of leaves without significant performance impacts.
Status: Added
*Selected brightened versions of some textures overwritten with a separate resourcepack with permission!*
![Pasted image 20260902180814.png](/img/user/Attachments/Pasted%20image%2020260902180814.png)

[Simple Grass Flowers](https://modrinth.com/resourcepack/simple-grass-flowers)
Author: 2DWisp
Type: Resource Pack
License: ARR
Purpose in Pack: Add cute flowers to grass and similar blocks.
Status: Added

[Fast Better Grass](https://modrinth.com/resourcepack/fast-better-grass)
Author: Fabulously Optimized, robotkoer
Type: Resource Pack
License: MIT
Purpose in Pack: Make grass all-sided.
Status: Added

[Fast Better Grass for Simple Grass Flowers](https://modrinth.com/resourcepack/fast-better-grass-for-simple-grass-flowers)
Author: Jacosvaldo
Type: Resource Pack
License: CC-BY-NC-SA-4.0
Purpose in Pack: Provide compatability between the above two packs.
Status: Added

[Os's Colorful Grasses](https://modrinth.com/resourcepack/os-colorful-grasses)
Author: Oslypsis
Type: Resource Pack
License: ARR
Purpose in Pack: Make grass really bushy and lush.
Status: Added

[More Nether Roots](https://modrinth.com/resourcepack/more-nether-roots)
Author: \_daggsy\_
Type: Resource Pack
License: CC-BY-NC-ND-4.0
Purpose in Pack: Gives nether roots some cool variations.
Status: Added

[Lily Padding](https://modrinth.com/resourcepack/lily-padding)
Author: witheredwasabi
Type: Resource Pack
License: ARR
Purpose in Pack: Improve lilypads.
Status: Added

[Golden Sunflowers](https://modrinth.com/resourcepack/golden-sunflowers)
Author: DenSlendyY
Type: Resource Pack
License: ARR
Purpose in Pack: Make sunflowers look huge and golden.
Status: Added

[Val's Leaf Litter](https://modrinth.com/resourcepack/vals-leaf-litter)
Author: legovideosrock
Type: Resource Pack
License: ARR
Purpose in Pack: Make leaf litter less obviously tiled.
Status: Added
*Disable this if you're the kind of legend who uses leaf litter for floor boundary patterns*

[Interactive Foliage](https://modrinth.com/mod/mc2-interactive-foliage)
Author: Kart0, RazorPlay01
Type: Mod
License: ARR
Purpose in Pack: Make leaves and grass wave in the wind, along with moving when entities interact with them.
Status: Added

[Os's Variated Glow Lichen](https://modrinth.com/resourcepack/os-variated-glow-lichen)
Author: Oslypsis
Type: Resource Pack
License: ARR
Purpose in Pack: Make glow lichen look way cooler.
Status: Added
##### **Create**

[Redstone Link Fix](https://modrinth.com/resourcepack/create-fixed-redstone-links)
Author: CharmDragon
Type: Resource Pack
License: [CC-BY-NC-4.0](https://creativecommons.org/licenses/by-nc/4.0/)
Purpose in Pack: A slight tweak to make Redstone Links legible when under blocks.
Status: Added

[Brass Encased Elytra](https://modrinth.com/resourcepack/create-brass-encased-elytra)
Author: Ryuucchi
Type: Resource Pack
License: ARR
Purpose in Pack: Unify the Elytra with the Create aesthetic.
Status: Added
> [(Possible Alternative)](https://modrinth.com/resourcepack/create-elytra/gallery)

[Create Horse Armor](https://modrinth.com/resourcepack/create-horse-armor/gallery)
Author: Awoolanche
Type: Resource Pack
License: ARR
Purpose in Pack: Unify horse armor with the Create aesthetic.
Status: Added

[Create: No Hats](https://modrinth.com/resourcepack/no-hats-for-create)
Author: mentalxpc
Type: Resource Pack
License: GPL-3.0-Only
Purpose in Pack: Fixing the broken Create hats due to Fresh Animations.
Status: Added

##### **Other**

[Saros Worldborder Customizer](https://modrinth.com/mod/saros-worldborder-customizer)
Author: Saroscesch
Type: Mod
License: ARR
Purpose in Pack: Enable more customisation of the world border
Status: Added

[3D Skin Layers](https://modrinth.com/datapack/low-end-gravity)
Author: tr7zw
Type: Mod
License: tr7zw Protective License
Purpose in Pack: Make yourself look a little bit better.
Status: Added

[Vanilla Tweaks](https://vanillatweaks.net/picker/resource-packs/)
Author: Andre, rx, Stridey, ioblackshaw, Xisumavoid, and more!!
Type: Resource Pack
License: Custom + Modpack Permission Explicitly Given
Purpose in Pack: Provide various texture-related fixes and tweaks!
Status: Added, may be tweaked/re-downloaded in future
*Will be loaded low to avoid compatability issues - it just does so much!*

[Vanilla Experience+](https://modrinth.com/resourcepack/vanilla-exp)
Author: Kryqu
Type: Resource Pack
License: ARR
Purpose in Pack: Improve a few things like walls, items, and round logs
Status: Added
*Will be loaded low and have many features disabled via the config to just keep the best things for this pack!*

[Better Entity Shadow](https://modrinth.com/resourcepack/better-shadow-entity!)
Author: NelA470
Type: Resource Pack
License: CC-BY-NC-ND-4.0
Purpose in Pack: Make entity shadows squared instead of round
Status: Added

[Sun & Moon Fusion](https://modrinth.com/resourcepack/sun-moon-fusion)
Author: OrkaMC
Type: Resource Pack
License: CC-BY-NC-SA-4.0
Purpose in Pack: Make the sun and moon look cooler :)
Status: Added

[Cosmos](https://modrinth.com/mod/cosmos-mod)
Author: Hollowed, TheTyphothanian
Type: Mod
License: ARR
Purpose in Pack: Improve the night sky and add a north star.
Status: Added

[Bathymetry](https://modrinth.com/mod/bathymetry)
Author: ZipeStudio
Type: Mod
License: CC-BY-ND-4.0
Purpose in Pack: Changes the water surface colour based on the depth of the water. Makes oceans look less flat.
Status: Added

[Pumpkin Blur, Pixelated and Circular!](https://modrinth.com/resourcepack/pixelated-circular-pumpkin-blur)
Author: ARKK
Type: Resource Pack
License: ARR
Purpose in Pack: Make the pumpkin blur easier to see through and more vanilla-styled
Status: Added

#### **Shaders**
Boring disclaimer
	*Due to the absence of Colorwheel for 26.2, shaders won't fully integrate Create contraptions into their shadows and lights. If Colorwheel does release for 26.2, Mellow should work by default, but I can't say how well Photon will move over.*

[Photon](https://modrinth.com/shader/photon-shader)
Author: sixthsurge
Type: Shader
License: none...?
Purpose in Pack: A balance of performance and good visuals.
Status: Added

[Mellow](https://modrinth.com/shader/mellow)
Author: TheCMK
Type: Shader
License: MIT
Purpose in Pack: Provide super performant and nice visuals.
Status: Added

[Complementary Shaders](https://modrinth.com/shader/complementary-reimagined)
Author: EminGT
Type: Shader
License: [Custom](https://github.com/ComplementaryDevelopment/ComplementaryReimagined/blob/main/License.txt) + Modpack Permission Explicitely Granted
Purpose in Pack: A heavier option for those with stronger PCs.
Status: Added
*Note: Complementary is not selected by default, ergo per their license does not need a specific credit in the front-matter description of the pack.*

[Euphoria Patches](https://modrinth.com/mod/euphoria-patches)
Author: SpacEagle17
Type: Mod
License: MPL2.0
Purpose in Pack: Expand on Complementary's options and features.
Status: Added
#### **LOD mods**
*At the moment, many alternative options are in the works, but this is what I'm going with for now, it may change.*

[Voxy](https://modrinth.com/mod/voxy)
Author: cortex
Type: Mod
License: ARR + Modpack Permission Explicitly Given
Purpose in Pack: Enable ridiculously long view distances with minimal performance impact.
Status: Added
*Note: Requires 1 lower version of Iris to run*

Voxy Seedgen
Author: 
Type: Mod
License: ARR
Purpose in Pack: Allow Voxy to generate distant terrain at a fraction of the usual cost.
Status: Added
*Note: waiting on modrinth release for proper integration.*

[Voxy Extra](https://modrinth.com/mod/voxy-extra)
Author: ImGRUI
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Really to fix a fog draw distance bug.
Status: Added

[Voxy Seam Fix](https://modrinth.com/mod/voxy-seam-fix)
Author: DunneWortel
Type: Mod
License: ARR
Purpose in Pack: Fix the gaps in water in Voxy.
Status: Added
## World Generation :LiStarHalf:

Custom Seed Filter (link pending Modrinth approval)
Author: Leclowndu
Type: Mod
License: N/A
Purpose in Pack: Limit the potential world generation to a list of filtered seeds
Status: Added
*Proof of purchase*
![Pasted image 20260916145124.png|254](/img/user/Attachments/Pasted%20image%2020260916145124.png)
*Proof that I am making the logos*
![Pasted image 20260916145247.png|352](/img/user/Attachments/Pasted%20image%2020260916145247.png)
*Proof of permission to upload to Modrinth*
![Pasted image 20260916205015.png|425](/img/user/Attachments/Pasted%20image%2020260916205015.png)
A huge thanks to Leclowndu for making this mod for me!

*Information about seed filtering*
	Using a [fork](https://github.com/SunnySlopes/cubiomes-viewer) of Cubiomes, I searched for seeds with all of the following features within 4096 blocks in each direction:
	- A Woodland Mansion (Legit mansions are very rare and were slowing down the search, so instead my pack places them in a way where you shouldn't run into more than a few in any given world, but you *should* get at least one! Shout out to MCSR for introducing me to nether structure quad placement graphs which gave me the idea of how to do this.)
	- Better balanced climates with roughly 15% coverage of each climate zone
	- At least one very tall mountain i.e 180 blocks and up, ensured by a 1.5% area with -0.75 erosion
	- Particular rare or required biomes: Bamboo Jungle, Cherry Grove, Eroded Badlands, Flower Forest, Ice Spikes, Mangrove Swamp, Meadow, Mushroom Fields, Old Growth Birch Forest, Pale Garden, and Sunflower Plains
	- Cherry Grove and Mushroom Fields have a minimum size requirement
	- At least one Desert Pyramid
	The search doesn't fully reflect the changes made by mods, but CliffTree generally respects the world seed, and makes some rare biomes like Cherry Groves larger, so I don't suspect there to be issues.

[CliffTree](https://modrinth.com/datapack/clifftree)
Author: Penumbra
Type: Mod
License: CC-BY-NC-SA-4.0
Purpose in Pack: Tweaks vanilla biomes and adds some new ones. Chosen for its reasonable use of vanilla blocks, high seed parity, and fun energy.
Status: Added

[Amplified Nether](https://modrinth.com/datapack/amplified-nether)
Author: Stardust Labs
Type: Mod
License: [Custom License](https://github.com/Stardust-Labs-MC/license/blob/main/license.txt) (which includes Modpack Permission)
Purpose in Pack: Make the Nether taller, more spacious, and easier to navigate - and also looks epic!
Status: Added

[Biome Dither](https://modrinth.com/mod/biome-dither)
Author: Pufferfish
Type: Mod
License: ARR
Purpose in Pack: A biome surface-block random blender that's broadly compatible with terrain mods.
Status: Added

[Streams Reflowing](https://modrinth.com/mod/streams-reflowing)
Author: nice.john aka. noodles
Type: Mod
License: ARR
Purpose in Pack: Add differing-height lakes and flowing streams and rivers.
Status: HOLD
*It's just a bit unreliable and buggy in its current state... if it still is by the time it comes to pack release, I'll mention it as a recommended optional addition since the concept is so cool.*

[Landmarks](https://modrinth.com/mod/landmarks)
Author: orlouge
Type: Mod
License: ARR
Purpose in Pack: Add fun features to the landscape, procedural and vanilla-friendly.
Status: Added
*This has been modified with a datapack to reduce the occurence of very large rock structures. Underwater vents use campfires which I'm not obsessed with, but I can live with it.*

[Better Lava Lakes](https://modrinth.com/mod/better-lava-lakes)
Author: weboyee
Type: Mod
License: MIT
Purpose in Pack: Make surface lava lakes look much better.
Status: Added

## Minor Additional Content

[ButterBee - Mob Variants](https://modrinth.com/datapack/butterbee)
Author: Penumbra
Type: Mod
License: CC-BY-NC-SA-4.0
Purpose in Pack: Adds more mob variants to fit the biomes of CliffTree.
Status: Added

[Party Spores](https://modrinth.com/mod/party-spores)
Author: A5ho9999
Type: Mod
License: Custom License + Modpack Permission Explicitly Given
Purpose in Pack: Lets you dye spore blossoms and the particles they produce, great for builders wanting to tweak atmosphere.
Status: Added

[Reconnectible Chains](https://modrinth.com/mod/reconnectible-chains/gallery)
Author: evanbones
Type: Mod
License: LGPL-3.0-or-later
Purpose in Pack: Lets you string chains and leads between fences for decoration.
Status: Added

[Gardener's Dream](https://modrinth.com/datapack/gardeners-dream)
Author: Gurkis
Type: Mod
License: ARR
Purpose in Pack: Lets you plant all sorts of plants in all sorts of containers! It's got so many options, it's perfect for perfectionists.
Status: Added

[Banner Bedsheets](https://modrinth.com/datapack/banner-bedsheets) and [Banner Flags](https://modrinth.com/datapack/banner-flags)
Author: Gurkis
Type: Mod
License: ARR
Purpose in Pack: Allow you to use banners for bedsheets and flags.
Status: Added
*As these are really datapacks, there is some slightly janky behaviour, but the achievements do well to explain everything!*

[Many More Banners](https://modrinth.com/datapack/many-more-banners)
Author: moxvallix, wulfian
Type: Mod
License: CC-BY-SA-4.0
Purpose in Pack: Add tons of useful and cool banner pattern options without adding items. Tested to work with the above Banner Bedsheets and Flags!
Status: Added

[Transparent Blocks in Enchant Area](https://modrinth.com/datapack/purpurpacks-transparent-blocks-in-enchant-area)
Author: PurpurMC, granny, Rhythmic
Type: Mod
License: MIT
Purpose in Pack: Lets you decorate your enchanting setup without worrying about losing power.
Status: Added

[Soft Leaves](https://modrinth.com/mod/soft-leaves)
Author: Payangar
Type: Mod
License: ARR
Purpose in Pack: Leaves slow you down instead of stopping you, breaking your fall, and making riding horses easier, complete with particles and sounds.
Status: Added

[Leaves Us In Peace](https://modrinth.com/mod/leaves-us-in-peace)
Author: supersaiyansubtlety
Type: Mod
License: CC0-1.0
Purpose in Pack: Make tree leaves disappear faster, smartly
Status: Added

[Shear Leaf Litter](https://modrinth.com/datapack/shear-leaf-litter)
Author: FerranV
Type: Mod
License: MIT
Purpose in Pack: Leaf litter only drops when you shear it - no more clutter!
Status: Added

[Looting Shears](https://modrinth.com/datapack/purpurpacks-looting-shears)
Author: PurpurMC, Rhythmic
Type: Mod
License: MIT
Purpose in Pack: Lets you enchant shears with looting.
Status: Added

[Superior Stonecutter](https://modrinth.com/datapack/superior-stonecutter)
Author: proxi
Type: Mod
License: MIT
Purpose in Pack: Lets you do *way more* in the stonecutter - wood, wool, ice, clay, and all the stone types are much more translatable in a fair and balanced way.
Status: Added
*Create already has this functionality for its own blocks - so it's only fair!*

[Wandering Trader May Leave](https://modrinth.com/mod/wandering-trader-may-leave)
Author: Serilium
Type: Mod
License: ARR
Purpose in Pack: Adds a button to peacefully dismiss the Wandering Trader.
Status: Added

[Proper Pet Teleport](https://modrinth.com/mod/ppetp) A.K.A PPeTP
Author: TheEpicBlock
Type: Mod
License: LGPL-3.0-or-later
Purpose in Pack: Make pets teleport to you after being unloaded without a performance cost
Status: Added

[Respawnable Pets](https://modrinth.com/mod/respawnable-pets)
Author: MoriyaShiine, cybercat5555
Type: Mod
License: ARR
Purpose in Pack: Adds a gem that makes your pets respawn after death
Status: Added

[IndyPets - Independent Pets](https://modrinth.com/mod/indypets)
Author: Fourmisain
Type: Mod
License: MIT
Purpose in Pack: Lets you toggle pets between roaming and following with J or shift-right clicking.
Status: Added

[Shearable Vines](https://modrinth.com/mod/shearable-vines)
Author: Roundaround
Type: Mod
License: MIT
Purpose in Pack: Shear vines to stop them from growing.
Status: Added

[Axe Effective Skulls](https://modrinth.com/datapack/purpurpacks-axe-effective-skulls), [Pickaxe Effective Reinforced Deepslate](https://modrinth.com/datapack/purpurpacks-pickaxe-effective-reinforced-deepslate), [Pickaxe Effective Glass](https://modrinth.com/datapack/purpurpacks-pickaxe-effective-glass), [Pickaxe Effective Light Source Blocks](https://modrinth.com/datapack/purpurpacks-pickaxe-effective-light-source-blocks), [Hoe Effective Froglights](https://modrinth.com/datapack/purpurpacks-hoe-effective-froglights), [Hoe Effective Cactus](https://modrinth.com/datapack/purpurpacks-hoe-effective-cactus)
Author: PurpurMC, granny, Rhythmic
Type: Mod
License: MIT
Purpose in Pack: Make various tools work on various things that make sense.
Status: Added

[Axolotls Ignore Passives](https://modrinth.com/datapack/purpurpack-axolotls-ignore-passives), [Breed Axolotl With Tropical Fish](https://modrinth.com/datapack/purpurpack-breed-axolotl-with-tropical-fish-item)
Author: PurpurMC, granny, Rhythmic
Type: Mod
License: MIT
Purpose in Pack: Stop axolotls from killing harmless squids and fish! And lets you feed them with fish from your hand instead of just from a bucket.
Status: Added
## Performance/BugFixes/Utility

#### **Performance**
*A quick benchmark with no other mods at 10 render distance gets ~1000 FPS on my 3060 mid-high range system while flying around at creative speed loading chunks. Occasionally this spiked to 1400FPS+. This is satisfactory enough for me to continue development off of this standard.
Note 1: Some mods here use multi-threading, which may not work well on CPUs with fewer threads. Disable c2me and see if that improves things.
Note 2: c2me OpenCL engine should fallback correctly for incompatible systems, but if you have issues with chunk generation, try disabling it entirely.*

[Sodium](https://modrinth.com/mod/sodium)
Author: CaffeineMC
Type: Mod
License: Polyform Shield 1.0.0
Purpose in Pack: Greatly improve performance.
Status: Added

[Lithium](https://modrinth.com/mod/lithium)
Author: CaffeineMC
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Speed up game logic like mob AI and block ticking among other things.
Status: Added

[ImmediatelyFast](https://modrinth.com/mod/immediatelyfast)
Author: RaphiMC
Type: Mod
License: LGPL-3.0-or-later
Purpose in Pack: Provide further conditional performance boosts on top of Sodium and Iris.
Status: Added

[Optimised Block Entities](https://modrinth.com/mod/obe)
Author: maDU59\_
Type: Mod
License: LGPL-3.0-or-later
Purpose in Pack: Make block entities render faster
Status: Added

[Gnetum](https://modrinth.com/mod/gnetum)
Author: decce6
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Improve HUD rendering by smartly dropping HUD framerate. 
Status: Added

[ScalableLux](https://modrinth.com/mod/scalablelux)
Author: ishland
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Actually to reduce bottlenecking on new chunk generation.
Status: HOLD (it's being weird)

[FerriteCore](https://modrinth.com/mod/ferrite-core)
Author: malte0811
Type: Mod
License: MIT
Purpose in Pack: Improve memory usage.
Status: Added

[ServerCore](https://modrinth.com/mod/servercore)
Author: Wesley1808
Type: Mod
License: MIT
Purpose in Pack: Introduce some patches and optimisations that don't affect gameplay by default.
Status: Added

[More Culling](https://modrinth.com/mod/moreculling)
Author: FX, 1Foxy2
Type: Mod
License: GPL-3.0-only
Purpose in Pack: Cull many things, mainly leaves
Status: Added

[fastnoise](https://modrinth.com/mod/zfastnoise)
Author: Reverie Projects, ZenXArch
Type: Mod
License: MPL-2.0
Purpose in Pack: Slight improvements to chunk generation speed, with Vanilla and Modded worldgen parity.
Status: Added

[C2ME](https://modrinth.com/mod/c2me-fabric)
Author: ishland, duplexsystem
Type: Mod
License: ARR
Purpose in Pack: Greatly speed up world generation by using multiple CPU cores.
Status: Added

[C2ME OpenCL Acceleration Module](https://modrinth.com/mod/c2me-ocl)
Author: ishland
Type: Mod
License: ARR
Purpose in Pack: Utilise the GPU on certain systems to aid C2ME's chunk generation boost.
Status: Added
*'`openclAccel.allowIncompatibilityFallback`' is set here, so systems with incompatible GPUs shouldn't experience any issues. Key word shouldn't - remove this mod if world generation isn't working right for you.*

[Structure Layout Optimizer](https://modrinth.com/mod/structure-layout-optimizer)
Author: TelepathicGrunt
Type: Mod
License: MIT
Purpose in Pack: Speed up structure generation.
Status: Added

[Ixeris](https://modrinth.com/mod/ixeris)
Author: decce6
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Improve menu and view lag when using a high-polling-rate mouse. I can't test this improvement because I'm using a Logitech MX4, iykyk.
Status: Added

[Quick-Pack](https://modrinth.com/mod/quick-pack)
Author: DrexHD
Type: Mod
License: MIT
Purpose in Pack: Improve resource and data pack loading times, particularly for large packs.
Status: Added

[Particle Core](https://modrinth.com/mod/particle-core)
Author: fzzyhmstrs
Type: Mod
License: MIT
Purpose in Pack: Smartly cull and optimise particles.
Status: Added

[Async Particles](https://modrinth.com/mod/asyncparticles)
Author: Harvey\_Huskey
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Further particle optimisation plus collision with Create contraptions as a bonus.
Status: Added

[Alternate Current](https://modrinth.com/mod/alternate-current)
Author: Space Walker
Type: Mod
License: MIT
Purpose in Pack: Improve processing of redstone wire. Feel free to remove/disable if you have issues with locationality.
Status: Added

[XP Stream](https://modrinth.com/mod/xp-stream)
Author: Jed-Tech
Type: Mod
License: CC-BY-NC-ND-4.0
Purpose in Pack: Improve the performance of large amounts of XP by letting the player absorb as much as fast as possible.
Status: Added

[Async Logger](https://modrinth.com/mod/asynclogger)
Author: decce6
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Makes logging asynchronous and therefore less impactful.
Status: Added

#### **Utility/Information**

[Mod Menu](https://modrinth.com/mod/modmenu)
Author: Terraformers
Type: Mod
License: MIT
Purpose in Pack: Allow configuration of mods from in-game.
Status: Added

[Chat Filters](https://modrinth.com/mod/chatfilters)
Author: spzla
Type: Mod
License: GPl-3.0-only
Purpose in Pack: Silence the automated messages from datapacks when a world is loaded
Status: Added

[Preferred Gamerules](https://modrinth.com/mod/preferred-gamerules)
Author: Estecka
Type: Mod
License: MIT
Purpose in Pack: Pre-sets gamerules on each world
Status: Added

[Language Reload](https://modrinth.com/mod/language-reload)
Author: Jerozgen
Type: Mod
License: MIT
Purpose in Pack: Speed up language swapping and add a search bar. If you mainly speak another language, look for Create Mod translation resource packs.
Status: Added

[Console Spam Fix: Reborn](https://modrinth.com/plugin/console-spam-fix-reborn)
Author: Author87668
Type: Mod
License: ARR
Purpose in Pack: Lets me filter out irrelevant/annyoing log lines that threaten to bloat log files and make them harder to read.
Status: Added

[Spark](https://modrinth.com/mod/spark)
Author: lucko
Type: Mod
License: GPL-3.0-only
Purpose in Pack: Help diagnose performance issues. Will be removed before release.
Status: Added

[Packed Packs](https://modrinth.com/mod/packed-packs)
Author: fishstiz
Type: Mod
License: MIT
Purpose in Pack: Help to manage resource packs.
Status: Added

[Yeetus Experimentus](https://modrinth.com/mod/yeetus-experimentus)
Author: Sunekaer, ErrorMikey, Nanite
Type: Mod
License: ARR
Purpose in Pack: Remove the 'Experimental Settings' warning
Status: Added

[Log Cleaner](https://modrinth.com/mod/log-cleaner)
Author: altrisi
Type: Mod
License: GPL-3.0-only
Purpose in Pack: Deletes old, untouched logs.
Status: Added
#### **Bug Fixes**

[ModernFix-mVUS](https://modrinth.com/mod/modernfix-mvus)
Author: Coredex
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Fix bugs, reduce memory usage, and speed up loading. Modern-version fork of Modern Fix.
Status: Added

[Worldgen Patches](https://modrinth.com/mod/worldgen-patches)
Author: Apollo
Type: Mod
License: MIT
Purpose in Pack: Fix steep surface condition, generation of snow on and under trees, among other things
Status: Added

[NetherPortalFix](https://modrinth.com/mod/netherportalfix)
Author: BlayTheNinth
Type: Mod
License: ARR
Purpose in Pack: Fix the weird thing where you can go in one nether portal and come out another.
Status: Added

## Will Not Include

[Dynamic FPS](https://modrinth.com/mod/dynamic-fps)
Isn't as needed on versions post-1.21.1 because Vanilla introduces a similar feature. You're welcome to add this if you prefer the functionality and customisability of Dynamic FPS, which can also give you battery alerts for laptop users.

[Nvidium](https://modrinth.com/mod/nvidium)
Since this modpack uses shaders by default, and this expects a Nvidia GPU, it won't be usable most of the time. If you are a Nvidia user with a series 20xx or higher and don't intend to play with shaders enabled, feel free to add this. Be warned it may cause crashes.

[Entity Culling](https://modrinth.com/mod/entityculling)
I've been told that the performance increases here are situational, and at times detrimental. Feel free to include it if you are making huge mob farms that are hidden behind walls; I think that's the main use case of this mod.

[Packet Fixer](https://modrinth.com/mod/packet-fixer) and similar network stack improvements
I don't have friends to test whether this modpack performs well in multiplayer; you're welcome to add these kinds of mods if you like.

[Inventory Particles](https://modrinth.com/mod/inventory-particles)
I just think it's too distracting, I've tried turning down the particle counts but then they sort of come out of nowhere. You're welcome to include it, it's a well-made mod.

[Particle Interactions](https://modrinth.com/mod/particle-interactions/gallery)
Causes Particle Rain's rain to disappear for some reason.

[Nvidium](https://modrinth.com/mod/nvidium)
I wasn't seeing such shocking frame increases to risk potentially upsetting a non-Nvidia user. c2me OpenGL's impact is much greater so it *is* included for now despite card-specific requirements.

[Nature's Compass](https://modrinth.com/mod/natures-compass)
The UI doesn't mesh with the vision I have for this pack, though I agree that this functionality could be very helpful. I'll keep an eye out for alternatives.

[Wavify](https://modrinth.com/mod/wavify/gallery)
They flow upstream sadly

[Fast Surface](https://modrinth.com/mod/zfastsurface)
Has some conflict with ModernFix
