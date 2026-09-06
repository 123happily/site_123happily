---
{"dg-publish":true,"permalink":"/Create Lemonade/","dgShowToc":true,"created":"2026-08-04T07:52:07.603+09:30","updated":"2026-09-06T10:19:12.172+09:30"}
---

Here's the wiki for Create Lemonade;
It's also my main working document, you have my apologies for the mess.

## Description/Pitch/Surface-level Credits

CREATE: LEMONADE
When life gives you lemons, create lemonade!

Minecraft players have developed tons of farms, cheeses, exploits, and more. These allow you great progression, but can make the game feel aesthetically and logically incoherent. I don't want to use these techniques, but I don't want to play the 'hard' way either! This modpack aims to reduce the need for these exploits by offering alternatives, not trying to ban or nerf them. It leverages Create's fantastic design and many other gameplay tweaks to focus on factory building and expansion, with most typical challenges of Minecraft's (questionably balanced) gameplay removed. It's heavily inspired by Satisfactory; the focus is on automation, building, and relaxing through easy progression rather than PvE, punishing losses, or hardcore challenges.

Key words: Automation, QoL, Vanilla-ish, Simplicity, Fun, Casual

AI Declaration:
Though I cannot speak for the contents of this modpack (i.e mods, resource packs, datapacks) I can clarify that I don't use AI content or coding (such as LLM output or image/video/audio generation models) in my works.
My single use-case is using DeepSeek's free model to diagnose crash logs. I always read the relevant error first and do my own research before asking an LLM, which means I rarely have to resort to this method.

Explicit Credits; full listing via the wiki page:
Vanilla Tweaks: https://vanillatweaks.net/
Title generator: https://ewanhowell.com/plugins/minecraft-title-generator/ ("Bubble" template texture modified with Photopea)
Complementary Shaders: https://modrinth.com/shader/complementary-reimagined
# Workings

#### To-do/In Progress

- [ ] Add MIT credits to the credit.txt? find out if i even need to for things stored on modrinth?
- [ ] make the lantern hip slot a smaller proper lantern instead of the GIGACHAD BRICK it is rn lol
- [ ] add more stupid log things to the log cleaner where suitable
- [ ] I've disabled CliffTree's sky biomes for the meantime because it makes world previews difficult to see. I can probably re-enable these once i'm done using seed preview.
- [ ] Finalise a pack description and unify it between modrinth, and github, clearing it from here, making sure you include a link to this page and a credit explanation section
- [ ] remake vanilla tweaks using website to take out twinkling stars, hunger apples, GUI buttons, and tooltip, and clean up the dupe file while you're there
- [ ] Add overlay logic onto Create's blocks where it makes sense to do so (i.e tuff and deepslate gen next to ochrum...)
- [ ] look into a decent PBR pack to pair with shaders, or dont fucking bother yknow
- [ ] whatever resource pack manager mod you use, you should be able to make a preset or hide irrelevant packs or lock in packs or something, so do that
- [ ] I'd like variations or at least random rotation of the ice texture for places like ice spikes.
- [ ] make a suitable GUI for the crafter (not mission critical)
- [ ] Continue and wrap up the biome colorations in my pack
- [ ] fix up the create gui buttons to match the 26.2 format
- [ ] make a suitable locator bar resource edit for the [gui](https://mcasset.cloud/26.2/assets/minecraft/textures/gui/sprites/hud) (idk how to test it lmao)
- [ ] debate setting up very minor "lore" and a starting structure, like satisfactory.
- [ ] maybe reinstate voxy worldgen on release even though it has the OOM bug. casual players are unlikely to run into it...

#### Waiting for help

Deep Origins Stripped Log Fix
no action required in the meantime really

[voxy worldgen pause screen OOM crash](https://github.com/iSeeEthan/voxy_worldgen_v2/pull/93)
voxy worldgen is on hold until fixed

[Game close thread hang issue with Flywheel](https://github.com/ZurrTum/Create-Fly/issues/357)
Until this is resolved, I will be implementing the mentioned workaround that disables GPU rendering, however I don't want to ship this modpack until a solution is found because of the potential performance issues. when that happens, re-test shaders for compatibility.

Snowy leaves mod not playing nice with world generation for some reason. the author is as befuddled as I am so it's probably something to just live with.

fancymenu is shitting itself with Wakes. wait for wakes author to pony tf up and then reinstate it (may have to tell fancymenu guy to take away the incompat marker)

I put in a bug report to ARTSHADE for the fusion overlay misbehaviour, they saw it, we wait and see.

waiting for permission from dr7 (or no permission, depending) on using the 26.2 sodium port in the pack. if you spot them online, maybe ping them in the server.

#### Problem Solving

- [ ] Leaving the game paused and alt-tabbed, and coming back, makes the fog come super close. it fades back to reasonable after a few seconds. NO clue what that's about.
#### It's just cooked

Air Gap Fix not working on Create blocks is a shame but create being what it is, and create fly being a fork, I don't think it's even worth reporting the issue considering I don't know precisely the problem.

### Git

https://modpack-dev-knowledgebase.github.io/modpack-dev-wiki/wiki/useful-mods/performance/26.1/fabric/
handy wiki!

Basically use Git to store listing and information but not whole mods or resourcepacks so as not to break terms.

[the git](https://github.com/123happily/Create-Lemonade)
how to push to git (DO IT AFTER YOU CHANGE THE FILES LMAO):
git add .
git commit -m "commit name"
git push -u origin main

sick
i've never used git before
please be kind

the recommended method is pushing to a branch for changes (git branch -M whateverthebranchnameis) and then merging to main when you're happy, but lowkey i dont think i need to do this?
i might make two branches for shader or no shader if i can't figure out a way to swap in-game
grim situation though

*don't include shaders in your pushes, but do include their configs, with a smart gitignore!!!!!!!*

### Modrinth

When you export from Prism, selecting the folders i.e mods, resourcepacks correctly converts them to Modrinth dependencies instead of packaging the raw files, or at least it does something close enough.

I have to zip my datapack before distributing, but my resource pack seems to make it through unharmed, which is nice. Yeah basically it modrinth links everything it can and then adds anything it couldn't as files. Nice.

### Pack Resource and Data Pack

I can adjust biome-based sky, leaf, grass, and other foliage colors, and [more](https://github.com/MehVahdJukaar/polytone/wiki/Environment-Attributes), so it's probably ideal to keep track of what I've been up to...

Oak leaves for some reason eats the biome-based simple configurations alive, so I can't really use a full colormap for those. Everything else is fair game though.

I got permission to overwrite rainbow foliage's textures (see that section in aesthetics > rendering > leaves section for more information) so I'll be brightening leaves to have full control over their colour!

I've also put leaf litter under the 'foliage color' map (which is mainly for oak) and decided by the biome property files. It just feels a bit easier. i can always go back and give it its own colormap if i give a shit later.

TO DO:
- update acacia, dark oak, jungle, mangrove textures to be 'bright'
- change birch default to something slightly darker for sanity
- set up their colormaps since we're knuckling down on this idea again
- run through biomes and nail down looks for them, testing with all leaves and litter for anything horrendous
- muck around with adding https://modrinth.com/mod/falling-leaves-plus which is better than subtle effects' in that it has leaf-type-specificity and high customisability and worse in that they don't land on water but I think we'll all be ok. they honestly still might if it works how i imagine.

Clifftree's Snowy Old Growth Taiga is a frosty blue.
Taiga is a rich green.

## mods i might throw in later

I don't want realms but i'm gonna muck with the menu later so I'll be able to piss it off.

https://modrinth.com/resourcepack/capitalized-shaded-font
Font alternative to vanilla tweaks

os's colorful grasses are alright but also a bit much at times and hard to work with with extreme biome colorings. so...
https://modrinth.com/resourcepack/rads-lush-foliage
maybe we can hit it with a bit of this and a bit of
https://modrinth.com/resourcepack/foliage-tint
and a bit of
https://modrinth.com/resourcepack/slightly-better-foliage-colors.

https://modrinth.com/resourcepack/vanilla-exp/gallery has variated grass and hopefully the ability to turn most of the rest of the stuff off,

https://modrinth.com/resourcepack/colorful-fleurs/gallery
this might work with 
https://modrinth.com/resourcepack/foliage-tint/gallery
neither of which would work with https://modrinth.com/resourcepack/better-foliage/gallery which is pretty cool though. i wonder if it would spawn the same one for each 'cluster' (it will)

https://modrinth.com/resourcepack/flower-clusters
can't forget this!

https://modrinth.com/resourcepack/more-nether-roots also...

https://modrinth.com/resourcepack/createful-plaques

https://modrinth.com/resourcepack/os-variated-glow-lichen
would have to change vanilla tweaks so its not a 3d model in there anymore

https://modrinth.com/mod/wikiful
show pop-ups with handy info when the user finds an item, and add a menu-accessible wiki. handy to explain changes in the pack in-game, but might cause headaches with my create gui theming.

the thing to get wandering traders to go away lol

https://www.planetminecraft.com/texture-pack/3d-breaking/
this is so old there's no way right

https://modrinth.com/datapack/call-your-happy-ghast
fym 'needs cheats to work'. test.

https://modrinth.com/mod/not-enough-pots/gallery
this is doing *too much* but i cant find anything better

https://modrinth.com/resourcepack/white-leavesgrass-in-snow-biomes-winter-foliage
could be cool.

https://modrinth.com/datapack/simple-homing-xp
https://modrinth.com/mod/instant-xp-gain
one of these. the former is probably heavier but more widely compatible and less confusing so i'm leaning towards that

https://modrinth.com/mod/appleskin
should probably just do this even if i dont like the exhaustion bar... vanilla tweaks has a food refill indication though which is simple enough i think

https://modrinth.com/datapack/low-end-gravity
kinda a wicked idea for something with 6 fucking downloads

https://modrinth.com/mod/mc-day-counter
https://modrinth.com/mod/betterdays
https://modrinth.com/mod/sleep-warp-updated
it'd be great if these all worked together. Betterdays i would use to make days and nights much longer. sleep warp properly ticks things overnight which should play nice with create one hopes. the day counter is just really cute.
apparently sleepwarp breaks the formatting of fusz mods config screen text??? lmao. anyway

https://modrinth.com/mod/better-advancements
just seems worth it

https://modrinth.com/mod/reliable-requiem
VERY comprehensive death penalty- WHOAH. penalties-upon-death mod

https://www.curseforge.com/minecraft/mc-mods/modest-magic
an option for enchantments...

https://modrinth.com/resourcepack/shadify
might be handy?

https://modrinth.com/resourcepack/vanilla-exp/gallery
some cool things, some unneeded things, configurable with respackopts anyhow.

https://modrinth.com/mod/shadeandsaturation/gallery
could be handy

https://modrinth.com/mod/nomorepowder
pros: gets rid of powdered snow without fully removing it from the game
cons: AI slop

https://modrinth.com/mod/mc2-interactive-foliage
kinda sick

punchy/hyper punchy
i'm just unsure how it'll feel. will probably need create skyhook compat whatever whatever

https://modrinth.com/resourcepack/particles-updated/gallery
particle... effects ... poti... on...

https://modrinth.com/resourcepack/brays-better-3d-bow/gallery
if i care

https://modrinth.com/mod/datapack-injector
mm

https://modrinth.com/mod/bathymetry
looks sick. intelligently changes water surface colour based on depth.

## thoughts

I do want to enable the automation of *most stuff* in the game through either Create or non-ugly Vanilla methods. That means getting a full list of items and blocks (including create's) and culling it down - first removing anything that's just a combination of other stuff, and then interrogating the sources of the remaining stuff.

in terms of visuals, I don't want to give up on the idea of a shaders + non-shaders approach. I suppose I could make two versions of the pack, but that makes it difficult to update things. There isn't a quick toggling mod that can do what i need. i could maybe distribute an alternative sodium-options json somehow, though the instructions will doubtless be as complicated as doing it manually.
So what *do* I need to do manually?
Well... I need to toggle shaders, toggle brightness. Ideally that's all. let's build out the non-shader version of this, then add shaders, and see if anything else crops up that needs fiddling with.

featurify hopefully lets you disable pockets of lava in the nether.

you'll wanna mess with the config for the health mod and see if enchanting items loses you hearts. if it does, that's lame and i dont like it.

also maybe grab something to balance mobs. i'm thinking:
no surface mob spawns, only caves/under blocks
less spawning in general
weaker skeletons
weaker baby zombies
weaker vexes

i'm not done fixing snow. snow on stairs and slabs would be great. snow settings might help here.

the issue with completely disabling the end is the access to certain items/resources. end stone, chorus fruit, purpur, dragon egg, dragon head, and of course the big ones being shulkers and elytra.
So instead I might want to make the end less of a headache. not dying in the void is a start, but i'm not sure if that mod is ideal cause i think you can get softlocked LMAO you could try 'NoVoid' instead which is the same idea.
otherwise increasing the rarity of end cities with structurify
shulker drops two and respawning shulkers - make the former a guaranteed 2 drop and the latter a very long timer. this makes getting shulker boxes much easier.
some tweaks to the elytra to make it less OP for long distances might be good. there's just more support for it out there. i think i'll put elytra bounce, airbrake, and a rocket debuff on it with elytra tuning
then it can be visually improved with contrails and trims and physics and bonk mod lmao

# Modules
### Info
All of the mods, resource packs, and shaders are detailed here, organised into Modules based on their function.

Crediting:
The relevant link, author, license, and current state of inclusion in this pack are also noted.
For more information on licenses, see [here](https://modpack-dev-knowledgebase.github.io/modpack-dev-wiki/wiki/info/licenses/) and [here](https://www.tldrlegal.com/). Note that even ARR-licensed projects hosted on Modrinth waive their right to exclusion from modpacks per [Modrinth's Terms of Use](https://modrinth.com/legal/terms), but I will respect explicit requests for exclusion or removal where present. Please [[Contact Me\|contact me]] if you want to discuss how your work is included in this pack, or if I've made any mistakes.

As of current, I'm planning to license this pack under GPL due to the "Viral" nature of that license and my inclusion of content using it, or similar, licensing. I'm led to believe that using LGPL projects within a GPL pack is permissable via the license, but if I am wrong on that front, please contact me!

Template, chord 'tem' to insert
```
Author: 
Type: Resource Pack/Mod/Other
License: MIT/Public Domain/GNU GPL/LGPL/ARR/Custom/Modpack Permission Explicitly Given
Purpose in Pack:
Status: Planned/Added
```
'Planned' means the resource may or may not be included in future
'Added' means it is included in the pack
'HOLD' means it would be great to include, but I'm waiting on development changes or bug fixes

Sections will be marked with :LiBadgeCheck: once they are unlikely to require further work. Or just... good enough for now and I should stop thinking about them.

I'm also including a list of mods at the end that *aren't* included, why, and whether I suggest them to you or not.

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
*Removing stress and challenge, to let you focus on creativity and factory-building.*

[Just Enough Recipes](https://modrinth.com/mod/jei)
Author: mezz
Type: Mod
License: MIT
Purpose in Pack: View recipes, including Create's
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

## Aesthetics
*Simple, stylistic flair and atmosphere, unified with the Create aesthetic.*
#### **Menus**

[Fancy Menu](https://modrinth.com/mod/fancymenu)
Author: Keksuccino
Type: Mod
License: DSMSLv3.1
Purpose in Pack: Allow extensive customisation of the main menu (and more!)
Status: Added

[SpiffyHUD](https://modrinth.com/mod/spiffyhud)
Author: Keksuccino
Type: Mod
License: DSMSLv3.1
Purpose in Pack: Allow extensive customisation of the in-game hud
Status: Added
*This doesn't work with the improved hotbar mod, but Raised doesn't work with FancyMenu, so I sort of have to choose one or the other. I've just left this disabled for now.*

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

[Dynamic Crosshair](https://modrinth.com/mod/dynamiccrosshair)
Author: Crendgrim
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Dynamically hide and change the crosshair depending on what you're looking at - or not looking at.
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
> [(Possible Alternative)](https://modrinth.com/resourcepack/create-gui/gallery)

[Reliable Recount](https://modrinth.com/mod/o123456789-backport)
Author: evanbones
Type: Mod
License: GPL-3.0-or-later
Purpose in Pack: Styles item numbers in Create's format/font
Status: Added
*Kindly ported to 26.2 upon request!*

[VUL's Create Cursors](https://modrinth.com/resourcepack/vuls-create-cursors)
Author: avizvul42
Type: Resource Pack
License: MIT
Purpose in Pack: Change the cursor to be Create-themed. Ported to work with Cursors Extended on 26.2 using [this tool](https://fishstiz.github.io/cursors_extended-wiki/tools/#v3-converter).
Status: Added
> [(Possible Alternative 1)](https://modrinth.com/resourcepack/create-brass-style-cursors), [(Possible Alternative 2)](https://modrinth.com/resourcepack/nerfs-fancy-cursor)

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
Purpose in Pack: Enable ridiculously long view distances with minimal performance impact. If you have performance issues, keep this and set it to like 32 chunks and your real render distance to like 5, and it'll still be better than playing without it.
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
Status: Planned
*Many effects that I feel don't suit the look or are too intrusive have been disabled. Others have been reduced in intensity or likelihood. Will disable 'allow using blended render type' if issues around particle transparency occur. Particle culling has been disabled to reduce issues with existing particle culling mods. Some features, like the falling leaves, splahes, waterfalls, and fireflies, have been given to Particular.*

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

[Sunbathing Godrays](https://modrinth.com/resourcepack/sunbathing-godrays)
Author: MedVahdJukaar, BeagleNF404
Type: Resource Pack
License: MIT
Purpose in Pack: Add godrays even when shaders aren't enabled
Status: Added

##### **Overlays, Variations, and Connected Textures**
*Due to technical limitations, overlays don't work on connected textures via Continuity or Fusion, so overlays are being prioritised for the forseeable future*

[Deep Origins Overlays](https://modrinth.com/resourcepack/deep-origins-overlays)
Author: Devoxxel
Type: Resource Pack
License: MIT
Purpose in Pack: Add smooth and creative overlays between blocks.
Status: Added + Tweaked with a pack loaded on top for compat reasons

[Connected Bricks (Fusion)](https://modrinth.com/resourcepack/connected-bricks-(fusion)/gallery)
Author: Jacosvaldo
Type: Resource Pack
License: CC-BY-NC-SA-4.0
Purpose in Pack: Make bricks overlap each other nicely
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

[ButterBee x Fresh Animations](https://modrinth.com/resourcepack/butterbee-fresh)
Author: Konci
Type: Resource Pack
License: CC-BY-NC-SA-4.0
Purpose in Pack: FA support for ButterBee's Mob Variants
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

##### **Blocks**

[Better Enchanting Table](https://modrinth.com/resourcepack/better-enchanting-table)
Author: Jacosvaldo
Type: Resource Pack
License: CC-BY-NC-SA-4.0
Purpose in Pack: Make the enchanting table look better and glow
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
*By default this will be loaded lowest to avoid compatability issues - it just does so much!*

[Better Entity Shadow](https://modrinth.com/resourcepack/better-shadow-entity!)
Author: NelA470
Type: Resource Pack
License: CC-BY-NC-ND-4.0
Purpose in Pack: Make entity shadows squared instead of round
Status: Added

[Better Clouds](https://modrinth.com/mod/better-clouds)
Author: qendolin
Type: Mod
License: MPL-2.0
Purpose in Pack: Improve the look of clouds by making them dynamic and fluffy whilst still keeping a blocky style.
Status: Added

[Cosmos](https://modrinth.com/mod/cosmos-mod)
Author: Hollowed, TheTyphothanian
Type: Mod
License: ARR
Purpose in Pack: Improve the night sky and add a north star.
Status: Added

#### **Shaders**
*Focused on gameplay with a requirement of stable 60FPS on my system in ideal conditions (standing still in a plains biome). These have been configured for a Vanilla/Dungeons inspired look.*
==Note: Rainbow's Foliage causes decent performance hits with shaders enabled.==
Some of these shaders may be tossed to the wayside at a later date because of a lack of Colorwheel support.

[Complementary Shaders](https://modrinth.com/shader/complementary-reimagined) with [Euphoria Patches](https://modrinth.com/mod/euphoria-patches)
*Complementary*
Author: EminGT
Type: Shaderpack
License: Custom + Permission with Credit Granted
Purpose in Pack: Provide high-end, customisable visuals
Status: Added

*Euphoria*
Author: SpacEagle17
Type: Mod
License: MPL-2.0
Purpose in Pack: Allow further customisation and features
Status: Added

here's where i'd put my artshade... RAGH

[BSL](https://modrinth.com/shader/bsl-shaders)
Author: CaptTatsu
Type: Shaderpack
License: ARR
Purpose in Pack: A bright, fun look.
Status: Added
*You will want to disable Better Clouds in the mod menu in-game! BSL also doesn't respect Clifftree's custom sky colours, so it may make biomes feel more same-y. It's just here to give you another option if you'd like.*
## World Generation
*Changes to terrain and biomes, without adding any modded blocks or items, keeping a vanilla-ish feel. Currently in heavy / messy development.*

#### **Major Changes**

[Tectonic](https://modrinth.com/datapack/tectonic)
Author: Apollo
Type: Mod
License: MIT
Purpose in Pack: Change the terrain shape.
Status: Added
*This has been tweaked slightly from the default values, shrinking continent sizes, compressing biomes to reduce travel requirements, and prioritising flatter terrain.*

[CliffTree](https://modrinth.com/datapack/clifftree)
Author: Penumbra
Type: Mod
License: CC-BY-NC-SA-4.0
Purpose in Pack: Tweaks vanilla biomes and adds some new ones. Chosen for its reasonable use of blocks, lack of extra content, and fun energy. Will be checked and/or tweaked to ensure access to andesite for Create's progression.
Status: Added
*also look for autumn biomes, and backport the fall drop stuff if possible*
*There are shore biomes with plenty of andesite*

#### **Minor Changes**

[Biome Dither](https://modrinth.com/mod/biome-dither)
Author: Pufferfish
Type: Mod
License: ARR
Purpose in Pack: A biome surface-block random blend that's broadly compatible with terrain mods.
Status: Added

[Streams Reflowing](https://modrinth.com/mod/streams-reflowing)
Author: nice.john
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
*It's not possible to tweak the rarity, shaping, or sizing of landmarks as of current. It also uses campfires in underwater vents. This may go on HOLD until the ability to configure them is added, or may be modified to remove rocks entirely.*

## Minor Additional Content

[ButterBee - Mob Variants](https://modrinth.com/datapack/butterbee)
Author: Penumbra
Type: Mod
License: CC-BY-NC-SA-4.0
Purpose in Pack: Adds more mob variants to fit the biomes of CliffTree.
Status: Added

[Party Spore](https://modrinth.com/mod/party-spores)
Author: A5ho9999
Type: Mod
License: Custom License + Modpack Permission Explicitly Given
Purpose in Pack: Lets you dye spore blossoms and the particles they produce, great for builders wanting to tweak atmosphere.
Status: Planned
## Performance/BugFixes/Utility/Other
*The boring stuff that keeps it all working under the hood. I won't document the dependencies in this pack.*
#### **Performance :LiBadgeCheck:**
*A quick benchmark, with no other mods, at 10 render distance gets ~800 FPS on my 3060 mid-high range system. This is satisfactory enough for me to continue development off of this standard.*

[Sodium](https://modrinth.com/mod/sodium)
Author: CaffeineMC
Type: Mod
License: Polyform Shield 1.0.0
Purpose in Pack: Greatly improve performance. Specific version will be used to ensure compatibility with Voxy, Colorwheel, and more.
Status: Added
*On Version 0.9.1 until Voxy shifts its support to newer versions*

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

#### **Utility/Information**

[Mod Menu](https://modrinth.com/mod/modmenu)
Author: Terraformers
Type: Mod
License: MIT
Purpose in Pack: Allow configuration of mods from in-game.
Status: Added

[Crash Assistant](https://modrinth.com/mod/crash-assistant)
Author: KostromDan
Type: Mod
License: KostromDam MML 1.1.3
Purpose in Pack: Help with diagnosis after a crash. Hopefully won't come up too often...!
Status: Planned

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
Status: Planned

[Disable Narrator](https://modrinth.com/mod/disable-narrator)
Author: fmg1925
Type: Mod
License: MIT
Purpose in Pack: Removed narrator entirely, including the large logs it tends to print on Linux. Remove this mod if you use the narrator!
Status: Planned

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
#### **Game Tweaking**

[Featurify](https://modrinth.com/mod/featurify)
Author: faboslav
Type: Mod
License: CC BY NC ND 4.0
Purpose in Pack: Mainly to remove random pockets of lava in the Nether.
Status: Planned

[Structurify](https://modrinth.com/mod/structurify)
Author: faboslav
Type: Mod
License: CC BY NC ND 4.0
Purpose in Pack: Tweak the rarity, placement, and distribution of structures as required. This can encourage villages to spawn on flatter terrain, for example.
Status: Planned

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

## Extra Credits
*I didn't end up using these things, or assets from these things, in the modpack, but I used them for reference, or wanted to give shoutouts...!*

https://modrinth.com/resourcepack/ashen-trinkets-support
For guidance/reference on how to customise the trinket slots

https://modrinth.com/resourcepack/create-style-interface
I used this style/palette as guidance/reference for some more textures to keep everything organised :)

https://modrinth.com/resourcepack/dark-coffe-gui
For guidance/reference on how to get GUI resource packs to work properly on 26.2

https://modrinth.com/resourcepack/elytra-slot-retexture
For the idea more than anything :)