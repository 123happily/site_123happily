---
{"dg-publish":true,"permalink":"/Create Lemonade/"}
---

Here's the wiki for Create Lemonade;
It's also my main working document, so apologies for the mess.
I may split my personal workings to a separate document if required.

## Description/Pitch

CREATE: LEMONADE
When life gives you lemons, create lemonade!

Minecraft players have developed tons of farms, cheeses, exploits, and more. These allow you great progression, but can make the game feel aesthetically and logically incoherent. I don't want to use these techniques, but I don't want to play the 'hard' way either! This modpack aims to reduce the need for these exploits by offering alternatives, not trying to ban or nerf them. It leverages Create's fantastic design and many other gameplay tweaks to focus on factory building and expansion, with most typical challenges of Minecraft's (questionably balanced) gameplay removed. It's heavily inspired by Satisfactory; the focus is on automation, building, and relaxing through easy progression rather than PvE, punishing losses, or hardcore challenges.

Key words: Automation, QoL, Vanilla-ish, Simplicity, Fun, Casual

## Workings

https://modpack-dev-knowledgebase.github.io/modpack-dev-wiki/wiki/useful-mods/performance/26.1/fabric/
handy wiki!

### mods i might throw in later

https://modrinth.com/mod/wikiful
show pop-ups with handy info when the user finds an item, and add a menu-accessible wiki. handy to explain changes in the pack in-game, but might cause headaches with my create gui theming.

https://modrinth.com/mod/spark
check for cpu, ram performance issues and diagnose.

https://www.curseforge.com/minecraft/mc-mods/realistic-waves
Non-shader water tweaks, interesting

https://modrinth.com/mod/instant-feedback
this has a lot of great ideas, i wouldn't want to implement them all in one go though because. issues.

https://modrinth.com/mod/reliable-requiem
VERY comprehensive death penalty- WHOAH. penalties-upon-death mod

https://www.curseforge.com/minecraft/mc-mods/modest-magic
an option for enchantments...

https://modrinth.com/resourcepack/animated-items
neat

https://modrinth.com/resourcepack/3d-harnesses-x-fresh-animations
if the create ones don't support fresh, this will *have* to go on

https://modrinth.com/resourcepack/better-ghast-x-fresh-animation
idk whats the difference

https://modrinth.com/resourcepack/shadify
might be handy?

https://modrinth.com/resourcepack/vanilla-exp/gallery
some cool things, some unneeded things, configurable with respackopts anyhow.

https://modrinth.com/resourcepack/clearer-slot-highlight
great if this works with the scrolling

**worldgen problem lmao**
[map](https://map.jacobsjo.eu/?)

*world density*

terralith feels too american

i think tectonic looks kinda dooky

lithosphere is good for trains, flattening everything out and smoothing it, if a bit repetitive ...? i think this increases world height, and it probably hits performance pretty hard. barely any surface caves which is sort of lame too.
https://www.reddit.com/r/minecraft_configs/comments/1oc4lbt/how_can_i_decrease_lithospheres_continent_sizes/
this has some advice on how to adjust the continent sizes, it seems lithosphere already has those.

'deeper oceans' is cool if i'm not doing any other world density stuff

https://modrinth.com/mod/underground-rivers
as advertised. they're kind of annoying to mine in tho
and probably dont like streams reflowing if i had to guess

https://modrinth.com/mod/streams-reflowing
this looks SICK, looks like Create waterwheels work as well!

continents is really neat, if i'm not using anything else... people are reporting some tiny mountain bugs, and it may be frustrating if i'm nerfing elytra for long distance. it just doesn't scream 'trains' to me. lol. but its cool...

*biomes/features*

https://modrinth.com/datapack/larger-biomes
probably wont work with other worldgen stuff that's too drastic, it touches the climate noises

sensible biomes has a few issues. a couple biomes make no sense, it messes with terrain shape just enough that it probably isnt super compatible with anything else. and its lower versioned. but the ... *sigh* the concept is good.

https://modrinth.com/mod/landmarks
these are really sick, but i'd want to remove some of the more ridiculous ones if at all possible.

geophilic is so reliable and sexy i love it so much.

https://modrinth.com/mod/latitude/gallery
climate banding, with built-in world size limitation (with a 'sandstorm' on east/west and i think a snowstorm on north/south). i dont think the biome or terrain mod compat is very good though, it's not really meant to be. it would be so cool if this worked with other things but its not a priority.
of course, natural temperature is another option, but i'm not convinced of the value to the game in general

https://modrinth.com/datapack/clifftree
cool for a more surprising one.
has animal variants that have a fresh animations pack too. i worry about the andesite situation though lmao otherwise this looks SICK!

https://modrinth.com/mod/wwoo/gallery
new stuff and transitions, but the trees can get sort of big... they're not *that bad* though. adds autumn-inspired forests. and it has some extra stuff you can enable in config. Lots of great biomes actually, looking more into it, with great hints as to underground biomes based on surface features. Gets quite cheeky with block placement (shrub on top of tall grass, leaf litter on top of water...) has a weird thing with 2-block-high walls...
it doesn't touch any terrain gen. could maybe use a replacer to go in and deal with areas with SUPER HUGE trees.
I don't want to add a treechopper because create covers for this functionality natively...!
https://modrinth.com/datapack/treeplacer-wythers-addon
has treeplacer support :D

https://modrinth.com/datapack/better-trees/gallery
interesting... does make some trees HUGE which i don't love

https://modrinth.com/datapack/taller-forests/gallery
just makes them a bit taller. geophilic does this iirc

https://modrinth.com/mod/falldropbackport/gallery
an option for autumn. obviously compat issues + adds shit i dont think i want to encourage like the cushions and wool stairs lmao

https://modrinth.com/datapack/austins-biomes-expansion/gallery
this is... cool, but it has some issues. there's no andesite variations of the 'other stone type' cave and beach biomes. a lot of the ideas are really great, though! and its lower versioned i guess.

need to make sure whatever i pick fits with![Pasted image 20260821170329.png](/img/user/Attachments/Pasted%20image%2020260821170329.png)or have to get rid of that.
i mean its probably fine anyway let's be honest

### thoughts

I like the idea of 'Let's Create!' or 'Just Create', a focus on the features of Create without complicating it with other stuff. possibly entirely disabling the end dimension. A really forgiving minimum difficulty (with Apathy or InControl or both). worldgen that's forgiving to train networks. encouragement of nether hubs/industry by making it a bit safer. general QoL.

I don't like the enchanting overhaul that I did, but I still want a better system.

i've learnt that complementary with euphoria actually makes for a decent vanilla+ look! and it's really too annoying to try doing it any other way, so. bah humbug.

featurify hopefully lets you disable pockets of lava in the nether.

you'll wanna mess with the config for the health mod and see if enchanting items loses you hearts. if it does, that's lame and i dont like it.

also maybe grab something to balance mobs. i'm thinking:
no surface mob spawns, only caves/under blocks
less spawning in general
weaker skeletons
weaker baby zombies
weaker vexes

the issue with completely disabling the end is the access to certain items/resources. end stone, chorus fruit, purpur, dragon egg, dragon head, and of course the big ones being shulkers and elytra.
So instead I might want to make the end less of a headache. not dying in the void is a start, but i'm not sure if that mod is ideal cause i think you can get softlocked LMAO you could try 'NoVoid' instead which is the same idea.
alternatively, the Dragon Drops Elytra - though I think it's lame that it has a text message about it
otherwise increasing the rarity of end cities with structurify
shulker drops two and respawning shulkers - make the former a guaranteed 2 drop and the latter a very long timer. this makes getting shulker boxes much easier.
some tweaks to the elytra to make it less OP for long distances might be good. there's just more support for it out there. i think i'll put elytra bounce, airbrake, and a rocket debuff on it with elytra tuning
then it can be visually improved with contrails and trims and physics and bonk mod lmao

i'm still having issues with closing the game, random stutters, voxy doesn't like it when i'm messing with shader settings (that's kind of fine though)
**makes me think I should rebuild this gradually.**

I lost track of my huge list very quickly. sorry. do it later when checking for modpack perms and organising things into 'modules' of balancing/content/graphics.

## Modules
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
Status: Planned/Added/Integrated
```
'Planned' means the resource may or may not be included in future
'Added' means it is in testing and awaiting config changes
'Integrated' means no more work is required

I'm also including a list of mods at the end that *aren't* included, why, and whether I suggest them to you or not.

### Create
*The core focus of the pack, thanks to Create Fly.*
### Balance
*Removing stress and challenge, to let you focus on creativity and factory-building.*

### Aesthetics
*Simple, stylistic flair and atmosphere, unified with the Create aesthetic.*

This is sorted into three main categories: **Menus, Sounds** and **Gameplay**. The latter is further broken down into a few *sub-categories*.

**Menus**

[Fancy Menu](https://modrinth.com/mod/fancymenu)
Author: Keksuccino
Type: Mod
License: DSMSLv3
Purpose in Pack: To allow the creation of custom Main and Pause menu screens.
Status: Planned

[Drippy Loading Screen](https://modrinth.com/mod/drippy-loading-screen)
Author: Keksuccino
Type: Mod
License: DSMSLv3
Purpose in Pack: To further customise the loading screen, as an extension of Fancy Menu.
Status: Planned

[Create Style Interface](https://modrinth.com/resourcepack/create-style-interface)
Author: ogabasferr
Type: Resource Pack
License: ARR
Purpose in Pack: Unify the Vanilla interfaces to be Create-themed.
Status: Planned
> [(Possible Alternative)](https://modrinth.com/resourcepack/create-gui/gallery)

[Create Style Tooltip](https://modrinth.com/resourcepack/create-style-tooltip)
Author: MangoJellyPudding
Type: Resource Pack
License: ARR
Purpose in Pack: Unify tooltips to be Create-themed. May remove for legibility concerns.
Status: Planned

[VUL's Create Cursors](https://modrinth.com/resourcepack/vuls-create-cursors)
Author: avizvul42
Type: Resource Pack
License: MIT
Purpose in Pack: Change the cursor to be Create-themed. Ported to work with Cursors Extended on 26.2 using [this tool](https://fishstiz.github.io/cursors_extended-wiki/tools/#v3-converter).
Status: Planned
> [(Possible Alternative 1)](https://modrinth.com/resourcepack/create-brass-style-cursors), [(Possible Alternative 2)](https://modrinth.com/resourcepack/nerfs-fancy-cursor)


*(PLACEHOLDER!)*
[Plains panorama with shaders](https://modrinth.com/resourcepack/plains-panorama-with-shaders)
Author: GAMING\_SHORTS(RAMA)
Type: Resource Pack
License: CC-BY-4.0
Purpose in Pack: A placeholder until I sort out a Create-themed Panorama.
Status: Planned

[Create Voice Chat Icons](https://modrinth.com/resourcepack/create-voice-chat-icons)
Author: JackCoin
Type: Resource Pack
License: ARR
Purpose in Pack: Unify the look of Simple Voice Chat, *if added to the pack by me or the end user*.
Status: Planned

**Sounds**

[Sounds x Create](https://modrinth.com/resourcepack/sounds-x-create)
Author: GamingFervor
Type: Resource Pack
License: MIT
Purpose in Pack: Help Create integrate properly with the Sounds mod
Status: Planned

**Gameplay**

- *General Rendering*

[Iris](https://modrinth.com/mod/iris)
Author: coderbot, IMS
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Enable the use of shaders, and provide some performance boost
Status: Planned

[Voxy](https://modrinth.com/mod/voxy)
Author: cortex
Type: Mod
License: ARR + Modpack Permission Explicitly Given
Purpose in Pack: Enable ridiculously long view distances with minimal performance impact. A beautiful mod. Stop complaining that there's no JAR distribution for forks, you can learn to build from Github. Sorry. Just needed to get that off my chest.
Status: Planned

[Better Biome Reblend](https://modrinth.com/mod/better-biome-blend)
Author: FionaTheMortal
Type: Mod
License: Unlicense
Purpose in Pack: Speed up and greatly increase biome blend radius for smoother biome transitions.
Status: Planned

- *Mobs, Entities, Armour*

[Brass Encased Elytra](https://modrinth.com/resourcepack/create-brass-encased-elytra)
Author: Ryuucchi
Type: Resource Pack
License: ARR
Purpose in Pack: Unify the Elytra with the Create aesthetic.
Status: Planned
> [(Possible Alternative)](https://modrinth.com/resourcepack/create-elytra/gallery)

[Create Horse Armor](https://modrinth.com/resourcepack/create-horse-armor/gallery)
Author: Awoolanche
Type: Resource Pack
License: ARR
Purpose in Pack: Unify horse armor with the Create aesthetic.
Status: Planned

[Create-Themed Happy Ghast Goggles](https://modrinth.com/resourcepack/create_themed_happy_ghast_goggles/gallery)
Author: Clamber-Cloud
Type: Resource Pack
License: MIT
Purpose in Pack: Cutely theme the Happy Ghast to the Create aesthetic.
Status: Planned

[Create: No Hats](https://modrinth.com/resourcepack/no-hats-for-create)
Author: mentalxpc
Type: Resource Pack
License: GPL-3.0-Only
Purpose in Pack: Fixing the broken Create hats due to Fresh Animations.
Status: Planned

- *Specific Blocks and Items*

[Redstone Link Fix](https://modrinth.com/resourcepack/create-fixed-redstone-links)
Author: CharmDragon
Type: Resource Pack
License: [CC-BY-NC-4.0](https://creativecommons.org/licenses/by-nc/4.0/)
Purpose in Pack: A slight tweak to make Redstone Links legible when under blocks.
Status: Planned


### World Generation
*Changes how the terrain generates, without adding any modded blocks or items, keeping a vanilla-ish feel*

[Biome Dither](https://modrinth.com/mod/biome-dither)
Author: Pufferfish
Type: Mod
License: ARR
Purpose in Pack: A biome surface-block random blend that's broadly compatible with terrain mods.
Status: Planned
### Performance/Dependencies/BugFixes/Utility/Other
*The boring stuff that keeps it all working under the hood. I probably won't document the dependencies in great detail...*

**Performance**

[Sodium](https://modrinth.com/mod/sodium)
Author: CaffeineMC
Type: Mod
License: Polyform Shield 1.0.0
Purpose in Pack: Greatly improve performance. Specific version will be used to ensure compatibility with Voxy, Colorwheel, and more.
Status: Planned

[Lithium](https://modrinth.com/mod/lithium)
Author: CaffeineMC
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Speed up game logic like mob AI and block ticking among other things.
Status: Planned

[ImmediatelyFast](https://modrinth.com/mod/immediatelyfast)
Author: RaphiMC
Type: Mod
License: LGPL-3.0-or-later
Purpose in Pack: Provide further conditional performance boosts on top of Sodium and Iris.
Status: Planned

[Gnetum](https://modrinth.com/mod/gnetum)
Author: decce6
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Improve HUD rendering by smartly dropping HUD framerate. 
Status: Planned

[FerriteCore](https://modrinth.com/mod/ferrite-core)
Author: malte0811
Type: Mod
License: MIT
Purpose in Pack: Improve memory usage.
Status: Planned

[Sodium Leaf Culling - Unofficial](https://modrinth.com/mod/sodiumleafculling-unofficial)
Author: pepe\_yu
Type: Mod
License: MIT
Purpose in Pack: Unofficial port of Sodium Leaf Culling. Will be changed to the official version if it reaches 26.2 Fabric.
Status: Planned

[fastnoise](https://modrinth.com/mod/zfastnoise)
Author: Reverie Projects, ZenXArch
Type: Mod
License: MPL-2.0
Purpose in Pack: Slight improvements to chunk generation speed, with Vanilla and Modded worldgen parity.
Status: Planned

[Ixeris](https://modrinth.com/mod/ixeris)
Author: decce6
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Improve menu and view lag when using a high-polling-rate mouse. I can't test this improvement because I'm using a Logitech MX4, iykyk.
Status: Planned

[Quick-Pack](https://modrinth.com/mod/quick-pack)
Author: DrexHD
Type: Mod
License: MIT
Purpose in Pack: Improve resource and data pack loading times, particularly for large packs.
Status: Planned

[Particle Core](https://modrinth.com/mod/particle-core)
Author: fzzyhmstrs
Type: Mod
License: MIT
Purpose in Pack: Smartly cull and optimise particles.
Status: Planned

[Async Particles](https://modrinth.com/mod/asyncparticles)
Author: Harvey\_Huskey
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Further particle optimisation plus collision with Create contraptions as a bonus.
Status: Planned

[BadOptimizations](https://modrinth.com/mod/badoptimizations)
Author: thosea
Type: Mod
License: MIT
Purpose in Pack: Slightly improve FPS by caching some things to do with lighting. Sky caching is automatically disabled due to the inclusion of Polytone. May remove as benefits seem minimal.
Status: Planned

[Alternate Current](https://modrinth.com/mod/alternate-current)
Author: Space Walker
Type: Mod
License: MIT
Purpose in Pack: Improve processing of redstone wire. Feel free to remove/disable if you have issues with locationality.
Status: Planned

**Utility/Information**

[Crash Assistant](https://modrinth.com/mod/crash-assistant)
Author: KostromDan
Type: Mod
License: KostromDam MML 1.1.3
Purpose in Pack: Help with diagnosis after a crash. Hopefully won't be needed for the end user!
Status: Planned

[Voxy Worldgen](https://modrinth.com/mod/voxy-worldgen)
Author: iSeeEthan
Type: Mod
License: iSeeEthan Custom License (I have checked this and am abiding by the modpack terms)
Purpose in Pack: Allow distant chunks to automatically generate and integrate with Voxy. Disable this in favour of pre-generation with Chunky if it causes you performance issues.
Status: Planned

[Sodium Extra](https://modrinth.com/mod/sodium-extra)
Author: FlashyReese
Type: Mod
License: LGPL-3.0-only + Modpack Permission Explicitly Given
Purpose in Pack: Remove toasts. Also gives you more granular control over various things rendered on screen.
Status: Planned

[Reese's Sodium Options](https://modrinth.com/mod/reeses-sodium-options)
Author: FlashyReese
Type: Mod
License: MIT
Purpose in Pack: I'm more familiar with this layout. Feel free to remove if you don't like it.
Status: Planned

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

**Game Tweaking**

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

**Bug Fixes**

[ModernFix-mVUS](https://modrinth.com/mod/modernfix-mvus)
Author: Coredex
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Fix bugs, reduce memory usage, and speed up loading. Modern-version fork of Modern Fix.
Status: Planned

[Max Health Fix](https://modrinth.com/mod/max-health-fix)
Author: DarkHax
Type: Mod
License: LGPL-2.1-only
Purpose in Pack: Fix an issue with maximum health over 20 when joining the game. Required if I choose to allow health over 20.
Status: Planned

[Simple Snowy Fix](https://modrinth.com/mod/simple-snowy-fix-(forge-fabric))
Author: KostromDan
Type: Mod
License: LGPL-3.0-only
Purpose in Pack: Fixes an annoying bug where snow on trees breaks over chunk borders. *I will also enable the 'snow on leaves under leaves' feature!*
Status: Planned

[Snow Under Trees](https://modrinth.com/mod/snow-under-trees-remastered)
Author: IMB11
Type: Mod
License: ARR (there is a specific modpack distribution guideline, but the link is dead. They're a developer at Modrinth, so I think they'll be OK with Modrinth's own terms-of-purpose re: modpacks.)
Purpose in Pack: Generates snow *under* trees, too! Widely compatible with worldgen mods, though I'll need to check that.
Status: Planned
> [(Alternative that fixes both of these along with steep surface rule bug)](https://modrinth.com/mod/worldgen-patches/gallery)

### Will Not Include

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

[Scalable Lux](https://modrinth.com/mod/scalablelux)
According to the devs, though it still has performance improvements over Vanilla, it isn't as severe as it used to be and isn't as needed on client anymore. I'm aware that in singleplayer you are simultaneously the server and the client, so if you think this would help, go for it, it looks well maintained.