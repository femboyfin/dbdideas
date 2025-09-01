# Miscellaneous and Basekit Changes

Here we'll include changes to other features that don't fit into the categories of perks/items/addons/powers. Often this means UI changes, adjustments to or additional basekit features, or more typically making an existing feature partially or fully basekit.

*Note this is not yet structured in an official fashion.*


## Basekit changes


### Partially basekit Kindred

This one has been suggested a lot, but having the survivor-aura portion of Kindred (Whenever any Survivor is hooked, the Auras of all Survivors are revealed to each other). This would substantially reduce the solo-queue guesswork as to whether or not your teammate is actually going for the save, and allow for much more coordinated two-man saves without communication.


### Refined serum blight trail on all Haste effects

The survivor Halloween event add-on [Refined Serum](<https://deadbydaylight.wiki.gg/wiki/Refined_Serum>) both applies Haste and "Creates a Blight trail behind the affected Survivor", this is a very distinct visual effect that clearly portrays to the killer and that survivor's teammates that they've used a Refined Serum and have the haste effect. Repurposing this visual effect would be a great way to convey to other players that a given player has Haste at the moment, and the strength of the effect could even be based upon the strength of the Haste, making it possible to identify Haste stacking. This allows players to make more informed decisions, for example, deciding not to chase a Hope user, identify Hex: No One Escapes Death at the beginning of end-game, or confirming Boon: Dark Theory.


### Automatic dying state recovery ⏲️

Automatically recover up to 95% (or 99% if allowed via perks) while not crawling. This prevents slugged survivors from forgetting to recover or griefing by refusing the recover.


### Change self-recovery action to an active ability button ⏲️

This one is quite simple, similar to the 2v8 Scout ability, instead of fully filling your recovery bar, you gain an active ability button to recover yourself once you're eligible to do so, instead of filling the bar. This ensures self-recovery is more deliberate, and works in tandem with the above automatic recovery change.


### Anti-power-proxy-camp mechanics

Progress the anti-camp meter at a faster rate based on killer power proximity. Would take more than one stage, say 90 seconds, to fully fill the anti-camp meter, meaning in practice, it primarily prevents the killer from proxying with power and then face camping to secure the stage progression. Would be somewhat tricky for certain killers like Huntress and Ghoul, although less effective, there could be checks on whether the hatchet is held down and aimed within a 90 degree cone towards the hook from the killer's position, same going for Ghoul power with his power held up ready to leap. This definitely would vary in effectiveness killer to killer, but overall would definitely be an improvement if tuned well.


### Anti-camp stage secure prevention

During the final portion (e.g. 10-20 seconds) of each hook stage, the other-survivor penalty is temporarily disabled, preventing the hooked survivor from being punished by a teammate attempting to go for an unhook while the killer is trying to secure the stage.


### Anti-camp chronic camping adjustment

Modify the normal 7-second grace period based on the average progression of the anti-camp meter per hook stage.


### Tie running grunts to grunts of pain

There is an additional sound layer to players running called "running grunts" that begin playing after sprinting continuously for ~5 steps. Currently there is nothing that effects the existence nor volume of these. Tying the volume of Running Grunts to the Grunts of Pain adjustments done by Iron Will, Off the Record, Stridor, etc. would provide these otherwise injured-only effects a more general minor benefit.


### Striped auras for objects that would be highlighted in multiple different colors

If for example a Generator should be highlighted in both White and Yellow, this would be shown as horizontal white and yellow striping.


### Clearly mark the escape boundary in exit gates

Over time a variety of new gate designs have been introduced to better suit different maps. This is great thematically and in certain maps the traditional gates would definitely clash/feel jarring. However this has introduced the issue where it is sometimes unclear exactly where the line to escape is, leading to some awkward situations where you may think you're in a safe position stalling for time but you actually aren't, or think you're safe from a given exit gate blocker addon because the escape boundary is farther than you intuitively thought. Having some sort of subtle glow or fog emanate from the line would make this much clearer, including for killers at a distance before their exit gate blockers are shown, making it easier to gauge whether hitting someone will knock them out or not before the swing.


## UI

### Mid-match text chat

Enables Keyboard & Mouse players to communicate with one another mid match, without the need for voice communication nor the moderation issues that accompany it, while still reducing the impact of survivors playing with voice chat.


### Quick messages menu

This will function similar to DBD Mobile's implementation, providing you with a variety of customizable preset messages to send to your teammates (e.g. via the above mid-match chat).


### Teammate loadout previews

Show the loadouts (perks, offerings, items, and addons) of survivors to one another, allowing survivors to play into each others perks. This is [partially planned](<https://x.com/DeadbyDaylight/status/1956094946320007554>), but only for perks and only once survivors are in the match, meaning you cannot plan your build around others (e.g. you may still have multiple healing players, multiple Open-Handed's, 4 Kindreds, etc and only realize this once you're in-game).


### Status effects in survivor HUD

This comes in two parts:
1. Similar to the broken icon that shows up for broken teammates, display other status hud effects alongside it like Exhausted, Hindered, and so on.
2. Display the timer for all effects, even though the timer is currently not present for Broken


### Display heal progress for injured survivors

This can use the same bar used for hook states/deep wound, simply displaying how healed a survivor is so you can tell if they're 99ed, have resurgence, etc. remotely. The decreasing deep wound timer could be changed to display as an outline around the bar, allowing the bar itself to display the mend progress consistent with the injured heal progress display.


### Display anti-camp self-unhook progress

This could be implemented similarly to the above change to the deep wound display, where there would be an outline around the hook stage bar indicating how close the survivor is to filling their anti-camp meter, making it easier to play around a camping killer and know if the killer is camping without other sorts of communication.


### Enable chat for console players

At worst this means console players can read chat but will have a hard time responding, at best this means they can respond on keyboard and mouse just like the other keyboard and mouse players on PC. This opens up the opportunity for pre-game planning and camaraderie, as well as post-game tips to help console players learn and grow.


### Display all encountered perks post-interaction

As of right now, a limited set of perks are displayed to the opposing role in the upper right when they're encountered. This means post interaction, sometimes it's unclear exactly what effect applied. This is particularly true in the case of Endurance effects, as it can be nearly impossible to tell if the survivor that got picked up died getting their final Mettle stack, had Soul Guard, or if the healer had We're Gonna Live Forever. This creates an unfortunate game of guesswork even among highly experienced players, and makes it more difficult for newer players to catch onto what effects are being used against them mid-game. Some easy examples are perks that cause survivors to scream, Endurance effects (and mettle), Breakout if it assists in a wiggle, Saboteur if it's used to successfully sabotage a hook, the cause of a generator explosion, and so-on.


### Display identified perks to all survivors

Currently, if one survivor encounters a perk like Dead Man's Switch or Oppression that show up in the upper right, this is only displayed to the survivor that encountered it, meaning it can be communicated to teammates in SWFs but not in solo queue. This could very easily be changed to also display it to other survivors once it's encountered.


### Revealed status effect in 1v4

In 2v8, Survivor Aura reveal is done via a Status Effect known as Revealed. This clearly communicates to the user that their Aura is being revealed. This is tremendously good for the new player experience, as absent equipping either Distortion (4,500 IS) or Object of Obsession (500 AC), there is no way to know if your Aura is being revealed to the opposing side. This could be done to both roles, meaning Killers would gain the Revealed effect as well. This would result in less confusion and allow for more opposing-side perk identification where it's otherwise impossible in many cases (Kindred, Wiretap, I'm All Ears, Bitter Murmur, etc).


### Display Perk/Addon/Power Icon for the source of Status Effects

Currently, the strength percentage values of certain effects like Haste & Hindered are both shown in the corner of those effects. This could be extended to display the icon of whatever caused it in the upper left corner. This means if you received the Mangled status from from Sloppy Butcher, you'll see the Sloppy Butcher icon in the corner of the Mangled icon in your HUD. This allows you to identify the source of an effect if you miss the initial cause of it in the upper right of the HUD, makes inflicting status effects more clear to the user, and makes it easier to identify if you're being affected by a perk's other  effects in cases where Aura reveal and other effects are triggered at once (think Babysitter, Gearhead).


### Display names of Perk/Addon/Powers in the upper right for effects shown in the Player Effects section of the HUD

Buff/debuff Player Effects currently don't always identify themselves by name in the upper right, making it more difficult to recognize and learn them for new players. For experienced players, they have the icon visible and can identify it visually, but there's no way for a new player to ask their friend what it does mid-match, or google it while working on generator/as you hook using a voice assistant. There is effectively no downside to this as you're not introducing new information, instead serving existing information in an additional way, making this primarily an accessibility and new player experience change.


## Settings

### Independently adjustable sliders for different types of audio

Separate the master and sound effects volume sliders into multiple sliders, for example:
- Menu/Lobby sound effects (e.g. doctor laugh, Jonesey meow, etc.)
- Terror Radii & Lullaby
- Chase Music
- Screams
- Killer Power Sound Effects (Blight rush, global Wraith cloak, Biopod ambient noise, etc.)


### Independently adjustable graphics settings

Enable changing the graphics settings Scalability Groups from the GameUserSettings.ini file directly through the in-game UI, opening up this customization to more PC players and to console players. Currently this consists of Resolution, View Distance, Anti-Aliasing, Shadows, Global Illumination, Reflections, Post-Processing Effects, Textures, Visual Effects, Foliage, Shading, Animation, and Landscape.
