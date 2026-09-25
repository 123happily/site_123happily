---
{"dg-publish":true,"permalink":"/Create Lemonade/","dgShowToc":true,"created":"2026-08-04T07:52:07.603+09:30","updated":"2026-09-25T19:30:10.238+09:30"}
---

Welcome to my main working document! Here you can see my thought processes and all credits for everything used in the modpack. Click here to go back to the wiki: [[Create Lemonade Wiki\|Create Lemonade Wiki]]
# Workings

I want to implement something similar to a Villager Trade Rebalance, but with respect for Enchancement's custom enchantments and the lack of tool durability (ergo no need for unbreaking or mending). TL:DR Biome based villager trades. encourages exploration at least before making a trading hall lmao

maybe try atmospheric, if you really feel the urge...

Enchancement needs heavy config but thats very much a balance thing


#### To-do/In Progress

- [ ] find a way to shut up datapacks on world load/test if they show on survival world load
- [ ] make [superior smelting](https://modrinth.com/datapack/superior-smelting) and [blasting plus](https://modrinth.com/datapack/blasting-plus) and [smoking plus](https://modrinth.com/datapack/smoking-plus) recipes work in create
- [x] add/fix enchantment table UI create style... probably its because of enchancements
- [x] furnaces have stopped rotating to face the player... its that gosh darn rotations pack... maybe just get rid of it.
- [ ] mark clifftree's sky biomes in biome spreader's no touchies config entry
- [ ] make clifftree biomes (of note) for https://modrinth.com/mod/biome-spreader, note recipes for wiki because they dont show in JEI.
- [ ] find a sound control mod to identify wtf is making a ding when you pull back a bow??
- [x] test if happy ghast calling works on survival
- [x] upload the custom seed filter to modrinth, yeah?
- [x] test whether reliable replacer is getting rid of powdered snow
- [ ] set create's schematicannon to be Fast
- [ ] trading with a piglin in the overworld sometimes results in them absolutely spewing gold everywhere but thats probably just vanilla being vanilla
- [ ] the snow golem's shaved head face is broken??
- [ ] grass break particle is dirt
- [x] Start making an alternate wiki or section here that explains the changes to gameplay without explaining all the mods in such detail, for players who want to know what's going on
- [ ] mess with buttons on pause screen
- [ ] Look into custom advancements ... i,e trade with every villager type... things completionists would want to do. it might be my only option aside from a wiki, which sucks, i just cant find a good option
- [ ] ban baby zombies. they're bullshit and i can't be arsed making the textures for them.
- [x] Add the thing into the datapack (do i even have one of those) to make ruined portals surface always
- [x] fix inventory spyglass slot to have the correct background colour
- [ ] search for 'planned' and implement or update entries, periodically.
- [ ] Leaving the game paused and alt-tabbed, and coming back, makes the fog come super close. it fades back to reasonable after a few seconds. NO clue what that's about.
- [ ] make the lantern hip slot a smaller proper lantern instead of the GIGACHAD BRICK it is rn lol
- [ ] add more stupid log things to the log cleaner where suitable
- [ ] I've disabled CliffTree's sky biomes for the meantime because it makes world previews difficult to see. I can probably re-enable these once i'm done using seed preview.
- [x] Finalise a pack description and unify it between modrinth, and github, clearing it from here, making sure you include a link to this page and a credit explanation section
- [x] remake vanilla tweaks using website to take out twinkling stars, hunger apples, GUI buttons, tool durabilities, and tooltip, and clean up the dupe file while you're there
- [ ] Add overlay logic onto Create's blocks where it makes sense to do so (i.e tuff and deepslate gen next to ochrum...)
- [ ] migrate to a resource pack management mod that lets you hide / lock things for the full release
- [x] fix up the create gui buttons to match the 26.2 format
- [ ] debate setting up very minor "lore" and a starting structure, like satisfactory.

#### Waiting for help

Waiting for BBE to fix their shading [issue](https://github.com/EdeenMC/betterblockentities/issues/145)

waiting for interactive foliage to blacklist lichen [here](https://github.com/Kart0/mc2-interactivefoliage/issues/21)

Waiting for mellow shader to fix their [weird fog issue](https://codeberg.org/TheCMK/mellow-shader/issues/232)

https://github.com/anyttng/toroidal_world/issues/48
map atlas toroidal compat request

DH + toroidal stack is nearly complete, but i want to test how map atlas will respond, and i lowkey just have to wait for them to look into leaf colouring...

https://github.com/Qendolin/better-clouds/issues/386
better clouds just fully shit itself so that's nice

sandw of Overlay's may implement my changes... if not i can ask for permission to use my changed version of the beta. we'll see.

Waiting to see if I Like Vanilla will consider [supporting vanilla fog and sky colours](https://github.com/What42Pizza/I-Like-Vanilla/issues/51)

Waiting for Saros worldborder customiser to fix its version reporting

[voxy worldgen pause screen OOM crash](https://github.com/iSeeEthan/voxy_worldgen_v2/pull/93)
voxy worldgen is on hold until fixed

[Game close thread hang issue with Flywheel](https://github.com/ZurrTum/Create-Fly/issues/357)
Until this is resolved, I will be implementing the mentioned workaround that disables GPU rendering, however I don't want to ship this modpack until a solution is found because of the potential performance issues. when that happens, re-test shaders for compatibility.
IT'S HAPPENING OH GOD lmao uh oh. uh ohhhh
i like vanilla will be fine, but
photon can be patched (photon 1.3a) but there's also [this](https://github.com/djefrey/photon) fork that keeps compat with voxy (maybe even DH is exclusive to this?) though its 5 months out of date from main
"**Tip**: it's common for shaderpacks to disable Entity Shadows or Block Entity Shadows by default. Make sure that those options are toggled if you want Create contraptions to cast lights and shadows (and don't forget to toggle the required options for light casting in the shaderpack settings !)."

[dadget's animal villagers nesting issue](https://github.com/draklorx/animalkin_villagers/issues/2)
once this is merged i can remove the fix from my own surface-level pack

fancymenu is shitting itself with Wakes. wait for wakes author to fix and then reinstate it (then i have to tell fancymenu guy to take away the incompat marker)

#### It's just cooked

https://github.com/Qendolin/better-clouds/issues/385
if this is fixed it MIGHT be worth trying to get them working but like its so much work for this lol

Air Gap Fix not working on Create blocks is a shame but create being what it is, and create fly being a fork, I don't think it's even worth reporting the issue considering I don't know precisely the problem.

Snowy leaves mod not playing nice with world generation for some reason. the author is as befuddled as I am. I don't expect a fix any time soon.

waiting for permission from dr7 (or no permission, depending) on using the 26.2 sodium port in the pack. apparently they've been MIA for a while now.
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

afaik there's no way to automatically set up a creative copy of a world, the best i could do is write wiki instructions on how to get started and then have some advancements that only trigger once you're in creative mode to explain the rest.

Pet Changes Potentially
https://modrinth.com/mod/ppetp fixes long range teleport/stuck in unloaded chunks without performance hit (nice)
https://modrinth.com/mod/respawnable-pets adds item to mark pets as respawnable with you on sleep. no clue if it works consecutively
https://modrinth.com/mod/indypets gives pets a third roaming mode aside from just following and sitting
https://modrinth.com/mod/petprotect pet damage prevention really meant for multiplayer environments (will break balance by allowing wolves to attack zombies without taking any damage for instance)

https://modrinth.com/mod/reliable-requiem
VERY comprehensive death penalty- WHOAH. penalties-upon-death mod
#### bugfix/util

https://github.com/D3ADK1LLSH0T/config-presets
this would be an absolute GODSEND if it was updated to 26.2. GOD. SEND. i'm following it twice lol.
#### graphics

punchy/hyper punchy
i'm just unsure how it'll feel. will probably need create skyhook compat whatever whatever
#### Waiting/'maybe'/misc

https://modrinth.com/mod/mc-day-counter
https://modrinth.com/mod/betterdays
https://modrinth.com/mod/sleep-warp-updated
it'd be great if these all worked together. Betterdays i would use to make days and nights much longer. sleep warp properly ticks things overnight which should play nice with create one hopes. the day counter is just really cute.
apparently sleepwarp breaks the formatting of fusz mods config screen text??? lmao. anyway

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

Please note: This modpack is distributed with a built-in resource pack that duplicates and reorganises many assets found in other resource packs. This pack will not be distributed outside of this modpack, and all rights go to the original texture owners. Textures are not heavily modified, mainly renamed and their file structures changed so that they can function correctly on 26.2. All original resource packs are still included in the pack so they will recieve proper crediting and download counts. Please reach out if you have any issues with this approach.

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
## Balance/QoL
*Making things easier, making the pack work, with as few nerfs as possible*

[Enchancement](https://modrinth.com/mod/enchancement)
Author: MoriyaShiine, cybercat5555, RAT, EightSidedSquare, Up
Type: Mod
License: ARR
Purpose in Pack: A radical approach to enchanting that adds enchantments, changes dynamics, balances things, removes tool durability, and fixes bugs.
Status: Added
*Heavily configured to remove some nerfing behaviour for the purposes of this pack*

[0,5 HP](https://modrinth.com/datapack/0%2C5-hp)
Author: BizCub
Type: Mod
License: MIT
Purpose in Pack: You will survive all fall damage with half a heart.
Status: Added

[World Border](https://modrinth.com/mod/world-border)
Author: Serilium
Type: Mod
License: ARR
Purpose in Pack: Loop the player around the world when they contact the world border
Status: HOLD (may not be needed)

[Just Enough Recipes](https://modrinth.com/mod/jei)
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
Author: 
Type: Resource Pack/Mod/Other
License: MIT/Public Domain/GNU GPL/LGPL/ARR/Custom/Modpack Permission Explicitly Given
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
*I will modify this to have some CliffTree biomes accessible as well :)*

[1.16.1 Ender Pearl Rates](https://modrinth.com/mod/1.16.1-ender-pearl-rates)
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
*Doesn't work with Create's building blocks, this is a 'better than nothing' situation*

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

[Instant Portal Nether](https://modrinth.com/mod/instant-portal-nether)
Author: JeanGomez
Type: Mod
License: MIT
Purpose in Pack: No more waiting 4 seconds to travel through the nether portal.
Status: Added

[Better Days](https://modrinth.com/mod/betterdays)
Author: wendall911
Type: Mod
License: LGPL-3.0-or-later
Purpose in Pack: Make days and nights a solid 20 minutes each, and lets you sleep a little earlier (per my config - this mod can do a lot more!)
Status: Added

[SleepWarp (Updated)](https://modrinth.com/mod/sleep-warp-updated)
Author: Patbox, Giggitybyte
Type: Mod
License: MPL-2.0
Purpose in Pack: Tick the game as you sleep so that furnaces process and crops grow. Watch the moon set and the sun rise. Makes sleeping take a little longer, but rewards you for it, instead of phantoms punishing you for not doing it.
Status: Added
## Aesthetics
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

[Immersive Hotbar](https://modrinth.com/mod/immersive-hotbar)
Author: DerpDerpling
Type: Mod
License: MIT
Purpose in Pack: Improve and spice up the hotbar
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
Status: Planned

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
Purpose in Pack: Improves the Advancements menu, which (pending some drastic changes) will be the main progression guide in this modpack.
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

[Day Counter](https://modrinth.com/mod/mc-day-counter)
Author: 02Alexis
Type: Mod
License: [Custom](https://github.com/02A1exis/02A1exis/blob/main/licenses/protective-license.md)
Purpose in Pack: Keep track of the days with a typewriter-ish counter each morning, and celebrate big milestones with sfx.
Status: Added

[Smooth Swapping](https://modrinth.com/mod/smooth-swapping)
Author: Schauweg, Riflusso
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Makes moving items in inventories look smooth!
Status: Added

[Create Style Interface](https://modrinth.com/resourcepack/create-style-interface)
Author: ogabasferr
Type: Resource Pack
License: ARR
Purpose in Pack: Unify the Vanilla interfaces to be Create-themed.
Status: Added
*Many assets required copy-pasting into the modpack's resource pack to work on 26.2. I'm not sure why. If someone knows, I'd like to let the original pack set the textures, but for now this is the best I can do.*

[Reliable Recount](https://modrinth.com/mod/o123456789-backport)
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

#### **Sounds** :LiBadgeCheck: 

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

#### **General Rendering**

##### **Setup**

[Iris](https://modrinth.com/mod/iris)
Author: coderbot, IMS
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Enable the use of shaders, and provide some performance boost.
Status: Added

[Voxy](https://modrinth.com/mod/voxy)
Author: cortex
Type: Mod
License: ARR + Modpack Permission Explicitly Given
Purpose in Pack: Enable ridiculously long view distances with minimal performance impact.
Status: HOLD in favour of:
*Note: Requires 1 lower version of Iris to run, should probably try dropping back a version and see if that fixes the leaf colours*

[Distant Horizons](https://modrinth.com/mod/distanthorizons)
Author: jeseibel and many more!
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Enable long view distances, now quickly proactively generated with 3.3's extra features. In tests, this actually performed better than Voxy in terms of framerate, and had comparable visuals.
Status: Added

[Voxy Worldgen](https://modrinth.com/mod/voxy-worldgen)
Author: iSeeEthan
Type: Mod
License: iSeeEthan Custom License (I have checked this and am abiding by the modpack terms)
Purpose in Pack: Allow distant chunks to automatically generate and integrate with Voxy. Disable this in favour of pre-generation with Chunky if it causes you performance issues.
Status: HOLD
*Waiting for a PR to be merged that fixes an OOM bug.*

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

[EMF](https://modrinth.com/mod/entity-model-features)
Author: Traben
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Support Fresh Animations among other things
Status: Added

[ETF](https://modrinth.com/mod/entitytexturefeatures)
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

[Entity View Distance](https://modrinth.com/mod/entity-view-distance)
Author: Patbox
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Lets you see entities further away, to compensate for low vanilla render and high LOD render distance.
Status: Added
*Feel free to increase it in the video settings if you feel it isn't enough*

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

[Wakes](https://modrinth.com/mod/wakes)
Author: Goby56
Type: Mod
License: GPL-3.0-only
Purpose in Pack: Add neat wakes to water when interacted with
Status: HOLD
*Has breaking incompatibility with FancyMenu...*

[Falling Leaves Plus](https://modrinth.com/mod/falling-leaves-plus)
Author: Fuzs
Type: Mod
License: MPL-2.0
Purpose in Pack: Provide varied and well animated falling leaves.
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
Type: Resource Pack/Mod/Other
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

[Animated Items](https://modrinth.com/resourcepack/animated-items)
Author: palettemc
Type: Resource Pack
License: CC-BY-NC-4.0
Purpose in Pack: Add some fun animations to various items in the inventory.
Status: Added
##### **Emission, Shading and Lighting**

[Fresh Animations: Emissive](https://modrinth.com/resourcepack/fresh-animations-emissive)
Author: FreshLX
Type: Resource Pack/Mod/Other
License: (Custom Terms of Use) + Explicit Modpack Permission Given
Purpose in Pack: Add glowing textures to some mobs
Status: Added

[LambDynamicLights](https://modrinth.com/mod/lambdynamiclights)
Author: LambdAurora
Type: Mod
License: Lambda License
Purpose in Pack: Make glowing blocks cast light around them
Status: Added

[Glowix](https://modrinth.com/resourcepack/glowix)
Author: CreepyWe
Type: Resource Pack
License: ARR
Purpose in Pack: Add emission to some blocks
Status: Added
*Glowing ores are off by default - turn them on if you prefer that!*

##### **Overlays, Variations, and Connected Textures**
*Due to technical limitations, overlays don't work with connected textures via Continuity or Fusion, so overlays are being prioritised for the forseeable future*

[Overlay's](https://modrinth.com/resourcepack/overlays)
Author: itzSandw
Type: Resource Pack
License: Custom EULA
Purpose in Pack: Enable cool transitions between blocks
Status: Added; **Waiting for update to be pushed**

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

[Natural Textures](https://modrinth.com/resourcepack/natural-textures)
Author: spiderbat
Type: Resource Pack
License: ARR
Purpose in Pack: Provide variation to various blocks by rotating them in a vanilla-friendly way.
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
##### **Grass/Leaves/Plants/Ground Cover**

[Better Snow Coverage](https://modrinth.com/mod/better-snow-coverage)
Author: ToBinio
Type: Mod
License: MIT
Purpose in Pack: Greatly improve the appearance of snow biomes by rendering fake snow layers in partial blocks that don't currently allow it.
Status: Added

[Mossy's Better Dirt](https://modrinth.com/resourcepack/mossys-better-dirt)
Author: pixelmossy
Type: Resource Pack
License: ARR
Purpose in Pack: Bring dirt's texture up-to-date with modern Minecraft
Status: Added

[Better Snowy Leaves](https://modrinth.com/mod/better-snowy-leaves)
Author: fabiofdez
Type: Mod
License: CC0-1.0
Purpose in Pack: Improve the look of leaves in snowy biomes, since the solid snow layer on top of bushy leaves looks really awkward.
Status: HOLD
*Note: Currently waiting for compatibility with Worldgen Patches*

[Rainbow's Foliage](https://modrinth.com/resourcepack/rainbows-foliage)
Author: PoeticRainbow
Type: Resource Pack
License: ARR
Purpose in Pack: Improve the fluffy look of leaves without significant performance impacts.
Status: Added
*Selected brightened versions of some textures overwritten with the pack's resource pack with permission!*
![Pasted image 20260902180814.png](/img/user/Attachments/Pasted%20image%2020260902180814.png)

[Simple Grass Flowers](https://modrinth.com/resourcepack/simple-grass-flowers)
Author: 2DWisp
Type: Resource Pack
License: ARR
Purpose in Pack: Add cute flowers to grass and similar blocks
Status: Added

[Fast Better Grass](https://modrinth.com/resourcepack/fast-better-grass)
Author: Fabulously Optimized, robotkoer
Type: Resource Pack
License: MIT
Purpose in Pack: Make grass all-sided.
Status: Added
> Previously was using Simple Lower Grass Sides, but it was going to require manual texture work with the overlay packs I was using, and I'm lazy. That's a great pack, definitely check it out.

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
Purpose in Pack: Make lilypads flower
Status: Added

[Golden Sunflowers](https://modrinth.com/resourcepack/golden-sunflowers)
Author: DenSlendyY
Type: Resource Pack
License: ARR
Purpose in Pack: Make sunflowers look huge and golden
Status: Added

[Val's Leaf Litter](https://modrinth.com/resourcepack/vals-leaf-litter)
Author: legovideosrock
Type: Resource Pack
License: ARR
Purpose in Pack: Make leaf litter less obviously tiled
Status: Added
*You might notice that leaf litter follows biome colour - that's actually my pack sitting on top and changing the colormap with Polytone!*

[Interactive Foliage](https://modrinth.com/mod/mc2-interactive-foliage)
Author: Kart0, RazorPlay01
Type: Mod
License: ARR
Purpose in Pack: Make leaves and grass wave in the wind, along with moving when entities interact with them
Status: HOLD
*Waiting for 2.0 to release*
##### **Create**

[Create Ultra](https://modrinth.com/resourcepack/create-ultra-pbr)
Author: MrUltra
Type: Resource Pack
License: ARR
Purpose in Pack: LabPBR for Create, particularly for Complementary/Euphoria Patches
Status: Added

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
Status: HOLD (may not need)

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
Author: 
Type: Resource Pack/Mod/Other
License: MIT/Public Domain/GNU GPL/LGPL/ARR/Custom/Modpack Permission Explicitly Given
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

[Better Clouds](https://modrinth.com/mod/better-clouds)
Author: qendolin
Type: Mod
License: MPL-2.0
Purpose in Pack: Improve the look of clouds by making them dynamic and fluffy whilst still keeping a blocky style.
Status: HOLD (sort of buggy atm)

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
	*Due to the absence of Colorwheel for 26.2, shaders won't fully integrate Create contraptions into their shadows and lights. If Colorwheel does release for 26.2, Mellow should work by default, but I can't say how well Photon will move over*

[Photon](https://modrinth.com/shader/photon-shader)
Author: sixthsurge
Type: Shader
License: none...?
Purpose in Pack: A balance of performance and good visuals
Status: Added

[Mellow](https://modrinth.com/shader/mellow)
Author: TheCMK
Type: Shader
License: MIT
Purpose in Pack: Provide super performant and nice visuals
Status: Added

## World Generation

Custom Seed Filter (link pending)
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
	Using a [fork](https://github.com/SunnySlopes/cubiomes-viewer) of Cubiomes, I searched for seeds with all of the following features within 5120 blocks in any direction:
	- All (vanilla) village types
	- At least one Mansion
	- At least 20% area covered by snowy, desert/badland, 'cold', and 'lukewarm' biomes, for good distribution
	- At least 2% area with -0.75 erosion to ensure at least one very tall mountain i.e 180 blocks and up
	- Particular rare or required biomes: Bamboo Jungle, Cherry Grove, Eroded Badlands, Flower Forest, Ice Spikes, Mangrove Swamp, Meadow, Mushroom Fields, Old Growth Birch Forest, Pale Garden, and Sunflower Plains
	- Mushroom Fields and Pale Garden needed to take up 0.02% of world space - an attempt to make sure they are of reasonable size, though there can still be many small instances
	The search doesn't reflect changes made by mods. I suspect these will play nice with CliffTree as it's quite responsive to the world seed.

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
Purpose in Pack: A biome surface-block random blend that's broadly compatible with terrain mods.
Status: Added

[Streams Reflowing](https://modrinth.com/mod/streams-reflowing)
Author: nice.john aka. noodles
Type: Mod
License: ARR
Purpose in Pack: Add differing-height lakes and flowing streams and rivers.
Status: Added

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
*I tried to confirm this was working, but couldn't find a surface lava pool, oh well*

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
## Performance/BugFixes/Utility/Other
*The boring stuff that keeps it all working under the hood. I won't document the dependencies in this pack.*
#### **Performance :LiBadgeCheck:**
*A quick benchmark, with no other mods, at 10 render distance gets ~800 FPS on my 3060 mid-high range system. This is satisfactory enough for me to continue development off of this standard. Note that some mods here use multi-threading, which may not work well on CPUs with fewer threads. Disable c2me and see if that improves things.*

[Sodium](https://modrinth.com/mod/sodium)
Author: CaffeineMC
Type: Mod
License: Polyform Shield 1.0.0
Purpose in Pack: Greatly improve performance. Specific version will be used to ensure compatibility with Voxy, Colorwheel, and more.
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

[Better Block Entities](https://modrinth.com/mod/better-block-entities)
Author: cseden, Adre278
Type: Mod
License: LGPL-3.0-or-later
Purpose in Pack: Greatly improve the performance of block entities.
Status: HOLD

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
Status: Added

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

[Sodium Leaf Culling - Unofficial](https://modrinth.com/mod/sodiumleafculling-unofficial)
Author: pepe\_yu
Type: Mod
License: MIT
Purpose in Pack: Unofficial port of Sodium Leaf Culling. Will be changed to the official version if it reaches 26.2 Fabric.
Status: Added

[fastnoise](https://modrinth.com/mod/zfastnoise)
Author: Reverie Projects, ZenXArch
Type: Mod
License: MPL-2.0
Purpose in Pack: Slight improvements to chunk generation speed, with Vanilla and Modded worldgen parity.
Status: Added (on hold for incompatibility with Toroidal World)

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
*This depends heavily on your system setup. I'm as of yet undecided if this should go in the full release; I'm unsure how it responds to incompatible setups.

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

[BadOptimizations](https://modrinth.com/mod/badoptimizations)
Author: thosea
Type: Mod
License: MIT
Purpose in Pack: Slightly improve FPS by caching some things to do with lighting. Sky caching is automatically disabled due to the inclusion of Polytone. May remove as benefits seem minimal.
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

#### **Utility/Information**

[Mod Menu](https://modrinth.com/mod/modmenu)
Author: Terraformers
Type: Mod
License: MIT
Purpose in Pack: Allow configuration of mods from in-game.
Status: Added

[Starter Items, Messages, and Commands](https://modrinth.com/mod/starter-items)
Author: spoorn
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Enable certain commands to be run on world start.
Status: Added

[Crash Assistant](https://modrinth.com/mod/crash-assistant)
Author: KostromDan
Type: Mod
License: KostromDam MML 1.1.3
Purpose in Pack: Help with diagnosis after a crash. Hopefully won't come up too often...!
Status: Added

[Seed Viewer](https://modrinth.com/mod/seed-viewer)
Author: Acenia
Type: Mod
License: MIT
Purpose in Pack: Help me to dial in world generation settings. Will most likely be removed in releases as it provides 'world map' functionality.
Status: Added

[Sodium Extra](https://modrinth.com/mod/sodium-extra)
Author: FlashyReese
Type: Mod
License: LGPL-3.0-only + Modpack Permission Explicitly Given
Purpose in Pack: Remove toasts. Also gives you more granular control over various things rendered on screen.
Status: Added
*Using this to disable vanilla falling leaves due to conflicts.*

[Reese's Sodium Options](https://modrinth.com/mod/reeses-sodium-options)
Author: FlashyReese
Type: Mod
License: MIT
Purpose in Pack: I'm more familiar with this layout. Feel free to remove if you don't like it.
Status: Added

[Language Reload](https://modrinth.com/mod/language-reload)
Author: Jerozgen
Type: Mod
License: MIT
Purpose in Pack: Speed up language swapping and add a search bar. If you mainly speak another language, look for Create Mod translation resource packs to fully apply it.
Status: Added

[Disable Narrator](https://modrinth.com/mod/disable-narrator)
Author: fmg1925
Type: Mod
License: MIT
Purpose in Pack: Removed narrator entirely, including the large logs it tends to print on Linux. Remove this mod if you use the narrator!
Status: HOLD
*Crashes for some unknown reason.*

[Console Spam Fix: Reborn](https://modrinth.com/plugin/console-spam-fix-reborn)
Author: Author87668
Type: Mod
License: ARR
Purpose in Pack: Silence irrelevant/unneeded log spamming messages.
Status: Added

[Spark](https://modrinth.com/mod/spark)
Author: lucko
Type: Mod
License: GPL-3.0-only
Purpose in Pack: Help diagnose performance issues. May be removed before release.
Status: Added

[Configured Defaults](https://modrinth.com/mod/configured-defaults)
Author: Fuzs
Type: Mod
License: MPL-2.0
Purpose in Pack: Ship default files with the modpack.
Status: HOLD
*Honestly I have next to no clue why I need this or what it does. Kumbayah*

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

#### **Bug Fixes**

[ModernFix-mVUS](https://modrinth.com/mod/modernfix-mvus)
Author: Coredex
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Fix bugs, reduce memory usage, and speed up loading. Modern-version fork of Modern Fix.
Status: Added

[Max Health Fix](https://modrinth.com/mod/max-health-fix)
Author: DarkHax
Type: Mod
License: LGPL-2.1-only
Purpose in Pack: Fix an issue with maximum health over 20 when joining the game. Required if I choose to allow health over 20.
Status: Planned

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

[More Culling](https://modrinth.com/mod/moreculling)
I'm unsure of stability and compatability with other mods in this pack. Feel free to try it yourself.

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
