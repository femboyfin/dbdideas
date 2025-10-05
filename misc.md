# Miscellaneous and Basekit Changes

Here we'll include changes to other features that don't fit into the categories of perks/items/addons/powers. Often this means UI changes, adjustments to or additional basekit features, or more typically making an existing feature partially or fully basekit.

*Note this is not yet structured in an official fashion.*


## Basekit changes


### Partially Basekit Kindred

This one has been suggested a lot, but having the survivor-aura portion of Kindred (Whenever any Survivor is hooked, the Auras of all Survivors are revealed to each other). This would substantially reduce the solo-queue guesswork as to whether or not your teammate is actually going for the save, and allow for much more coordinated two-man saves without communication.


- While a Survivor is on hook, the Aura of all Survivors are revealed to each other


### Haste Transparency

The survivor Halloween event add-on [Refined Serum](<https://deadbydaylight.wiki.gg/wiki/Refined_Serum>) both applies Haste and "Creates a Blight trail behind the affected Survivor", this is a very distinct visual effect that clearly portrays to the killer and that survivor's teammates that they've used a Refined Serum and have the haste effect. Repurposing this visual effect would be a great way to convey to other players that a given player has Haste at the moment, and the strength of the effect could even be based upon the strength of the Haste, making it possible to identify Haste stacking. This allows players to make more informed decisions, for example, deciding not to chase a Hope user, identify Hex: No One Escapes Death at the beginning of end-game, or confirming Boon: Dark Theory.


- All players affected by the Haste effect now create a Blight trail behind the affected player


### Proxy-Camp Prevention

Progress the anti-camp meter at a faster rate based on killer power proximity. Would take more than one stage, say 90 seconds, to fully fill the anti-camp meter, meaning in practice, it primarily prevents the killer from proxying with power and then face camping to secure the stage progression. Would be somewhat tricky for certain killers like Huntress and Ghoul, although less effective, there could be checks on whether the hatchet is held down and aimed within a 90 degree cone towards the hook from the killer's position, same going for Ghoul power with his power held up ready to leap. This definitely would vary in effectiveness killer to killer, but overall would definitely be an improvement if tuned well.


- Survivors' on-hook Resolve meter now fills slowly while the Killer is aiming at the hook


### Stage Securing Prevention

During the final portion (e.g. 10-20 seconds) of each hook stage, the other-survivor penalty is temporarily disabled, preventing the hooked survivor from being punished by a teammate attempting to go for an unhook while the killer is trying to secure the stage.


- Survivors' on-hook Resolve meter is no longer slowed by nearby Survivors during final 10 seconds of each Hook stage


### Chronic Camping Prevention

Modify the normal 7-second grace period based on the average progression of the anti-camp meter per hook stage.


- The 7-second Resolve meter grace period is now permanently disabled for all Survivors once a Survivor's Resolve meter is filled


### Running Grunts Improvement

There is an additional sound layer to players running called "running grunts" that begin playing after sprinting continuously for ~5 steps. Currently there is nothing that effects the existence nor volume of these. Tying the volume of Running Grunts to the Grunts of Pain adjustments done by Iron Will, Off the Record, Stridor, etc. would provide these otherwise injured-only effects a more general minor benefit.


- Running grunts are now affected by the volume of Grunts of Pain


### Multicolor Aura Striping

If for example, a Generator should be highlighted in both red and yellow, this would be shown as diagonal red and yellow striping.


- Players and Objects revealed in more than one color of Aura are now striped with both colors


### Escape Boundary Designation

Over time a variety of new gate designs have been introduced to better suit different maps. This is great thematically and in certain maps the traditional gates would definitely clash/feel jarring. However this has introduced the issue where it is sometimes unclear exactly where the line to escape is, leading to some awkward situations where you may think you're in a safe position stalling for time but you actually aren't, or think you're safe from a given exit gate blocker addon because the escape boundary is farther than you intuitively thought. Having some sort of subtle glow or fog emanate from the line would make this much clearer, including for killers at a distance before their exit gate blockers are shown, making it easier to gauge whether hitting someone will knock them out or not before the swing.


- The Exit Gate escape boundary is now visually marked with a smoky line


### Haste & Hindered Stacking

Haste stacking is a controversial issue, Behaviour has previously attempted to address this in the [8.7.0 PTB](<https://forums.bhvr.com/dead-by-daylight/kb/articles/501-8-7-0-ptb-patch-notes>) but it was removed following community backlash. There were effectively two groups of people at the time, proponents of keeping Haste stacking generally cited either the incentive to use off-meta perks or the build diversity benefits from unique synergies on otherwise low-strength Haste perks, whereas those against Haste stacking generally cited balancing problems where having to adjust every new Haste element (perks, powers, and addons) with the possibility of of it being used with any combination of existing Haste sources was limiting the potential Haste elements we could receive, because Haste can become very problematic when the numbers get too high. Both of these schools of thought are on their, correct, people were in effect arguing which of these factors were more important. The problem with Behaviors approach of outright disabling any type of Haste stacking was the all-or-nothing solution to such a polarizing issue. With the backstory out of the way, a likely better remediation to prevent extremely case scenarios, is to prevent stacking of 15% Haste on both sides. This stops Survivors from exceeding the base speed of a 4.6m/s killer, allowing them and even a 4.4m/s killer to catch up using Bloodlust, while also limiting non-bloodlust killers from exceeding the typical speed allowed by maximum Bloodlust (Bloodlust 3 = 15% movement speed increase). Notably this would take the highest strength Haste source into account first, and then only increase Haste up to this 15% cap at maximum. A few notable examples of cases where this middle-ground approach shrines are; Sprint Burst and other Exhaustion perks grant 50% Haste, if we outright cap Haste at 15%, this fundamentally breaks the Exhaustion perk concept of high speed balanced out by a short duration. So instead we apply the Haste from Sprint Burst, then if the survivor also is in range of Boon: Dark Theory, we see we're already above 15% so we stay at the 50% Haste from Sprint Burst rather than increasing it further to 53%. On the other hand, when activating Blood Pact and Power of Two, we see the 7% Haste from Blood pact is under the 15% cap, allowing us to add the 5% Haste from from Power of Two on top of it because that 12% is still under the cap, but if we suddenly both activate Hope, we're now limited to 15% instead of the full 19% from the +7% Haste, preventing us from moving faster than the killer in a straight line.


- The effects of Haste and Hindered no longer stack beyond 15%
- While multiple Haste or Hindered effects are active and they total higher than 15%, the percentage is set to 15%
- While multiple Haste or Hindered effects are active and one is above 15%, the largest percentage for each is used


### Match Reconnection

This is a long requested feature that has been previously dismissed under the guise that given the relatively short nature of Dead by Daylight trials, it would rarely serve much benefit. However in modern DBD, everyone has been in matches that lasted for an extended period of time- based on the official stats tracker, the average duration of my last 10 matches is 10.4 minutes, more than enough time to reconnect and take control over the bot that took my place (for reference it takes me 1 minute and 8 seconds to get from DBD's Steam library page to the main menu past the login steps on 5-6 year old hardware). The game crashes on occasion- all games do, internet and power can drop out on people, their computer itself can crash, their game could be experiencing a problem that requires a restart, and so on. This could provide a way to wait out some of your penalty by playing the match you disconnected from (potentially even earning bonus credit towards the remainder of your penalty for doing so), it would allow you to rejoin your friends after instead of waiting for their match to finish, enable the potential to take over the place of someone else's bot once you die, and so on. This can also work to disable queuing for the duration of the match as the user now has a way to play the game in front of them, extending DC penalties appropriately when their reason for disconnecting is because they object to something being used, played, or done, rather than out of frustration or out-of-game obligations. This prevents situations where someone can disconnect against a given character (e.g. Skull Merchant the moment they get past the camera pan and see her unique character portrait backgrounds) knowing that the match will likely last longer than 5 minutes and their penalty will only be 5 minutes. They now will have to wait out the duration of the match at minimum (the same amount of time the other players in that lobby had a degraded experience for), removing this awkward edge case where players who understand the system can abuse it, reducing DC rates overall.


- Players who have disconnected from a still-ongoing trial now have the option to Reconnect in place of the "Ready Up" button


### Bloodlust Reduction

A common community request over time has been some form of nerf to Bloodlust. Bloodlust's original purpose was to mitigate problematic "infinites" where the survivor could theoretically loop a structure or combination of structures for an unlimited amount of time without any possibility of the killer being able to injure the survivor, particularly in the case of basic attack-only killers. Common arguments for the removal of Bloodlust are that improved balancing of individual tiles and tile generation as a whole have naturally reduced the potential of infinites drastically, that the existence of window entity blockers have largely mitigated infinites on their own, and that higher tiers of Bloodlust are unnecessary to counter infinites. Common arguments against the removal of Bloodlust are that the time inefficiency of using higher tiers of Bloodlust to get an injury cancels out the benefit, that the removal disproportionately affects weaker killers as most chase powers reset Bloodlust on use making it primarily beneficial on killers with less beneficial chase powers, and that it serves as an important safety net in the rare case where tile generation does provide survivors with such a strong setup that it is (or at least almost is) an infinite even with the other systems in place. With that said, the outright removal of Bloodlust is likely not the best route to go, at least without playtesting the removal of higher tiers of bloodlust first. The third tier of bloodlust practically doesn't function as a needed safety net as even on a 4.4m/s killer, 120% movement speed is enough to maintain chase forcing entity blockers on window in effectively every tile setup, providing a feature that rewards players for playing inefficiently without a separate reason for such feature to exist is harmful to the growth of less experienced players, and needing anything beyond Bloodlust 2 to get a down is less of a low-tier killer problem and more of a low level of experience on that killer problem, leaving Bloodlust to serve as a secondary path to brute-force an injury for short term benefit without requiring the player to learn how to use that killer to get their injury in the traditional fashion with that killer's abilities. Bloodlust 2 is generally unneeded, but because it can be an important safety net for 4.4m/s movement killers in certain situations where they're unable to use their power to get an injury on a given loop, removing this altogether could have potential negative ramifications. Bloodlust 1 is still rarely needed, but does serve to benefit lower tier killers more than higher tier killers.


- Removed Bloodlust tier 3
- Increased chase time required to reach Bloodlust tier 2 to **30 seconds** *(was 25)*


### Exhausted Penalty

Currently, there is no basekit penalty for being Exhausted, making Exhausted-inflicting perks and addons on the killer side meaningless if the survivor doesn't have a perk equipped that's affected by Exhausted. Additionally, Exhaustion perks are among the strongest survivor perks in the game by a disproportionate margin, effectively being a must-run for all players if you're aiming for builds with the strongest perks.


- Now increases survivor volume by **50%** while Exhausted
- Now causes running grunts to played for twice as long


### Flashlight Changes

The previous two patches changing flashlights were 6.3.0 and 6.4.0, these were aimed at improving accessibility around photosensitivity and decreasing annoyance of flashlight clicking, but had a number of negative side effects. Clicking a flashlight has long been a non-verbal method of communicating with teammates who aren't in comms. The minimum hold time was intended to reduce the potential of "clicky spam" where survivors spam-clicked their flashlights extremely fast (sometimes using macros), causing an extremely loud clicking noise, as well as reduce the frequency of sudden flashing lights to avoid triggering strobing photosensitivity problems. The negative consequence of this change was increasing the amount of charges lost for clicking a survivor, before you'd lose one frame (~1/120th of a charge), whereas now you lose an actually noticeable amount. The actual lost charges is not very much, less than one charge, but over the course of a solo queue match where you're using your flashlight to point things out to your teammates quickly, it can add up and potentially cost you a blind. The other negative consequence of this is flashlights feeling a lot more clunky now than they used to. You're forced into walking speed for the duration of the minimum hold-time even after releasing right click, leading to your movement speed penalty being disconnected from your inputs which feels quite poor.


- Reduced stun buffer at the end of the killer pick-up animation to **0.1 seconds** *(was 0.4)*
- Now fades flashlight beams in and out when clicking and un-clicking
- Removed minimum flashlight beam on-and-off hold-time
- Added a brief delay before you can re-click a flashlight after turning it off


### Bloodpoint Adjustments

- Removed bloodpoint Category caps *(was 10,000)*
- Added a new combined cap of **50,000** *(was uncapped)* bloodpoints total per match before offerings
- Survivors in chase now receive **25%** of the Objectives and Altruism score their teammates receive during the duration of the chase
- All category-specific bloodpoint offerings are now all-player offerings
  - Category-specific bloodpoint offerings now boost the opposite-roles categories as follows; Objectives:Brutality, Survival:Sacrifice, Altruism:Deviousness, and Boldness:Hunter.
- Increased the effects of all category-specific bloodpoint offerings by **+100%**
- Survivor Pudding and Escape Cakes now provide bonus bloodpoint to all players
- Decreased Survivor Pudding and Escape Cake bloodpoint bonuses to **50%**
- Added dynamic bloodpoint bonuses for killers based on their playrate ranging from **+25%** to **+250%**
- Added **+50%** bloodpoint bonus while using perks currently in the Shrine of Secrets
- Added a weekly **+50%** bloodpoint bonus to the lowest play rate addons for each Item and Power from the previous week
- Decreased the P100 Bloodweb to renew at **Level 25**

### Player Loyalty Customizations

- Added unique Badge Borders based on player Devotion
- Added the option to equip prestige crests from previous prestiges

### Prestige Sacrifice

- Added the ability for characters at P100 to sacrifice their current prestige up to 6 times with the following benefits:
  - Sacrificed Torso/Weapon, Sacrificed Legs/Body, Sacrificed Head/Mask, Sacrificed First Perk Charm, Sacrificed Second Perk Charm, then Sacrificed Third Perk Charm. Sacrificed cosmetics are similar to the Legacy pattern but use a light blue color.
- Sacrificing a P100 character will result in the loss of all non-event and non-retired unlockables

## Inventory Quality Of Life

- Now automatically equips one of the pre-equipped starter add-ons if you don't de-equip your previous one after running out

## UI

### Text Chat

Enables Keyboard & Mouse players to communicate with one another mid match, without the need for voice communication nor the moderation issues that accompany it, while still reducing the impact of survivors playing with voice chat.


- Text chat is now available during Trials


### Quick Communications

This will function similar to DBD Mobile's implementation, providing you with a variety of customizable preset messages to send to your teammates (e.g. via the above mid-match chat). An 8-axis system is usable via D-pad, controller stick, mouse flick, and unique-key keybindings.


- Added an 8-axis quick communication wheel to send customizable preset messages to your teammates


### Teammate Loadout Previews

Show the loadouts (perks, offerings, items, and addons) of survivors to one another, allowing survivors to play into each others perks. This is [partially planned](<https://x.com/DeadbyDaylight/status/1956094946320007554>), but only for perks (no offerings, items, or addons) and only once survivors are in the match, meaning you cannot plan your build around others. This means you may still have multiple players with unhook perks, non-stacking perks such as Open-Handed, or conflicting offerings (e.g. two separate Hatch/Basement offerings or contradictory reagents).


- Survivors can now see other Survivors' loadouts in the lobby screen


### Survivor HUD Status Effects

This comes in two parts:
1. Similar to the broken icon that shows up for broken teammates, display other status hud effects alongside it like Exhausted, Hindered, and so on.
2. Display the timer for all effects, even though the timer is currently not present for Broken


- All status effects affecting other survivors are now shown in the portraits portion of the survivor HUD
- Status effects shown in the portraits portion of the survivor HUD now display timers


### Heal Progress Display

This can use the same bar used for hook states/deep wound, simply displaying how healed a survivor is so you can tell if they're 99ed, have resurgence, etc. remotely. The decreasing deep wound timer could be changed to display as an outline around the bar, allowing the bar itself to display the mend progress consistent with the injured heal progress display.


- The survivor progress bar now displays partial healing and mend progress in the HUD
- The existing deep wound bleed-out timer is now an outline around the bar itself


### Anti-Face Camp HUD Improvements

This could be implemented similarly to the above change to the deep wound display, where there would be an outline around the hook stage bar indicating how close the survivor is to filling their anti-camp meter, making it easier to play around a camping killer and know if the killer is camping without other sorts of communication.


- Hooked survivor's anti-face camp resolve meter is now shown as an outline around the hook stage bar for all survivors


### Text Chat Accessibility

At worst this means console players can read chat but will have a hard time responding, at best this means they can respond on keyboard and mouse just like the other keyboard and mouse players on PC. This opens up the opportunity for pre-game planning and camaraderie, as well as post-game tips to help console players learn and grow.


- Enabled text chat for players on Xbox, Playstation, and Nintendo Switch
- Added speech-to-text for text chat, allowing players to hold a button to dictate what they'd like to send


### Perk Notifications

As of right now, a limited set of perks are displayed to the opposing role in the upper right when they're encountered. This means post interaction, sometimes it's unclear exactly what effect applied. This is particularly true in the case of Endurance effects, as it can be nearly impossible to tell if the survivor that got picked up died getting their final Mettle stack, had Soul Guard, or if the healer had We're Gonna Live Forever. This creates an unfortunate game of guesswork even among highly experienced players, and makes it more difficult for newer players to catch onto what effects are being used against them mid-game. Some easy examples are perks that cause survivors to scream, Endurance effects (and mettle), Breakout if it assists in a wiggle, Saboteur if it's used to successfully sabotage a hook, the cause of a generator explosion, and so-on.


- Added notifications for more perks post-encounter


### Global Perk Identification Notifications

Currently, if one survivor encounters a perk like Dead Man's Switch or Oppression that show up in the upper right, this is only displayed to the survivor that encountered it, meaning it can be communicated to teammates in SWFs but not in solo queue. This could very easily be changed to also display it to other survivors once it's encountered.


- Now shows killer perk notifications to all survivors whenever someone encounters one for the first time


### Revealed Status Effect

In 2v8, Survivor Aura reveal is done via a status effect known as Revealed. This clearly communicates to the user that their Aura is being revealed. This is tremendously good for the new player experience, as absent equipping either Distortion (4,500 IS) or Object of Obsession (500 AC), there is no way to know if your Aura is being revealed to the opposing side. This could be done to both roles, meaning Killers would gain the Revealed effect as well. This would result in less confusion and allow for more opposing-side perk identification where it's otherwise impossible in many cases (Kindred, Wiretap, I'm All Ears, Bitter Murmur, etc).


- All forms of Aura reveal now inflict the Revealed status effect for the duration


### Player Effects Unlockable Notifications

Buff/debuff Player Effects currently don't always identify themselves by name in the upper right, making it more difficult to recognize and learn them for new players. For experienced players, they have the icon visible and can identify it visually, but there's no way for a new player to ask their friend what it does mid-match, or google it while working on generator/as you hook using a voice assistant. There is effectively no downside to this as you're not introducing new information, instead serving existing information in an additional way, making this primarily an accessibility and new player experience change.


- The names of icons shown in the Player Effects section are now shown in the upper right corner of the HUD upon first encounter


## Settings

### Volume Sliders

Separate the master and sound effects volume sliders into multiple sliders, for example:
  - Menu/Lobby sound effects (e.g. doctor laugh, Jonesey meow, etc.)
  - Terror Radii & Lullaby
  - Chase Music
  - Screams
  - Killer Power Sound Effects (Blight rush, global Wraith cloak, Biopod ambient noise, etc.)


- Added independent volume sliders for different types of sounds


### Independently adjustable graphics settings

Enable changing the graphics settings Scalability Groups from the GameUserSettings.ini file directly through the in-game UI, opening up this customization to more PC players and to console players. Currently this consists of Resolution, View Distance, Anti-Aliasing, Shadows, Global Illumination, Reflections, Post-Processing Effects, Textures, Visual Effects, Foliage, Shading, Animation, and Landscape.


- Added separate quality settings for different types of visuals


### Killer HUD Portrait

One sizeable benefit of playing in a party with out-of-game communication is the ability to call out who the killer is upon first interaction. This allows the other survivors to reposition themselves on their generators, decide which generators to focus on, create a plan for where to go if they're interrupted, determine how early they need to run from Terror Radius, or if there's even going to be a Terror Radius warning at all. Currently, the HUD contains four survivor portraits, with blank space above them up to the top of the screen. A simple and intuitive method of portraying the killer to survivors would be to add the killer above the four survivors in the HUD, populating their character portrait once someone enters chase with the killer.


- Added the killer to the player HUD on the left-hand side of the screen
- Now displays the killer's portrait to all survivors once a survivor has entered chase with them for the first time
