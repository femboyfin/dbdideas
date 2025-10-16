# Miscellaneous and Basekit Changes

Here we'll include changes to other features that don't fit into the categories of perks/items/addons/powers. Often this means UI changes, adjustments to or additional basekit features, or more typically making an existing feature partially or fully basekit.

*Note this is not yet structured in an official fashion.*


## Basekit changes


### Partially Basekit Kindred

- While a Survivor is on hook, the Aura of all Survivors are revealed to each other

***DEV NOTE**: It's not secret that coordinating Unhooks can be difficult for Survivors outside of a party. Kindred has long been a go-to perk for solo survivors to make coordinating Unhooks smart and reliable. This change should help both in determining whether or not to go for an Unhook, as well as for setting up multi-survivor Unhooks, reducing the gap between solo queue survivors and coordinated teams.*


### Haste Transparency

- All players affected by the Haste effect now create a Blight trail behind the affected player

***DEV NOTE**: Finding out your opponent had the Haste status effect without your knowledge can be frustrating for both new and experienced players. Our goal is to decrease the frequency of these frustrating interactions while making it clear what our new players are going up against.*


### Slugging Reduction

- Haemorrhage no longer affects healing survivors in the dying state
- Perks charged by spending time in the killer's Terror Radius while not in chase can now be charged while in the Dying State

<!-- TODO: Needs note -->

### Proxy-Camp Prevention

- Survivors' on-hook resolve meters now fill slowly based on how closely the killer is looking at the hooked Survivor
- This additional resolve fills at a rate of **1 charge per second** while aiming directly at the hooked survivor, decreasing by **0.1 charges** per **10 degrees** away the killer is aiming.
- This mechanic is disabled while the killer is farther than **32 meters** from the hooked survivor

***DEV NOTE**: We know it can be frustrating to see a killer walk just far enough away to not provide anti-camp resolve, camping as close as possible to the hook while subverting the existing anti-face camp system. Our goal with this change is to discourage killers from trying to circumvent the existing anti-camp systems, without punishing killers for solely keeping an eye on the hook from a distance if they aren't participating in other forms of camping.*


### Stage Securing Prevention

- Survivors' on-hook resolve meter is no longer slowed by nearby Survivors during final **10 seconds** of each Hook stage

***DEV NOTE**: In certain situations, survivors approaching a hook that's been camped from a slight distance can prevent the hooked survivor from filling their resolve meter, creating situations where the killer ends up being able to aggressively face-camp for the final portion of a survivor's hook stage. This change aims to reduce frustration surrounding this tactic, without unfairly punishing killers opportunistically returning to the hook from afar, as at most this will fill half of the anti-camp bar during this final 10 seconds.*


### Chronic Camping Prevention

- The 7-second resolve meter grace period is now permanently disabled once a survivor's resolve meter has been filled

***DEV NOTE**: We understand how frustrating it can be to have a killer repeatedly camp survivors on hook throughout the same trial. This change shouldn't unfairly punish killers who aren't doing this, and gives camping a single a hook a lasting penalty.*


### Running Grunts Improvement

- Running grunts are now affected by the volume of Grunts of Pain

***DEV NOTE**: Running Grunts are a little-known mechanic that adds a layer of grunting after continuously sprinting for a short period of time. Previously, there has never been any way to adjust this audio layer, this should provide a minor while-healthy benefit to Grunts of Pain reducing unlockables, increasing their typically relatively low strength level.*


### Multicolor Aura Striping

- Players and Objects revealed in more than one color of Aura are now striped with both colors

***DEV NOTE**: In situations where multiple unlockables that grant different color auras are in play (Déjà Vu, Blast Mine anyone?), it currently make its more difficult to determine which objects are under the effects of your perks. This ensures it's always possible to determine this, by highlighting the object in both colors at once.*


### Escape Boundary Designation

- The Exit Gate escape boundary is now visually marked with a smoky line

***DEV NOTE**: With the increase in unique map-specific gate designs over time, situations where survivors accidentally leave the trial or don't quite make it out have increased with this added variety. It's an all too common occurrence where it's difficult to tell exactly where the line you have to cross is, this should remediate these situations and prevent survivors from getting caught off guard by exactly where this boundary lies.*


### Haste & Hindered Stacking

- The effects of Haste and Hindered no longer stack beyond 15%
- While multiple Haste or Hindered effects are active and they total higher than 15%, the percentage is set to 15%
- While multiple Haste or Hindered effects are active and one is above 15%, the largest percentage for each is used

***DEV NOTE**: As explained in the [April 2025 Developer Update](<https://forums.bhvr.com/dead-by-daylight/kb/articles/500-developer-update-april-2025>), the stacking of status effects like Haste and Hindered have historically led to problematic circumstances with certain combos, resulting in these unlockables being far more powerful than intended. We heard the concerns the community shared during the [8.7.0 PTB](<https://forums.bhvr.com/dead-by-daylight/kb/articles/501-8-7-0-ptb-patch-notes>) about the first round of Haste & Hindered Stacking changes, and agree that it's important to maintain stacking for loadout synergy and variety. These revised changes should only limit extreme cases of stacking, without preventing the use of multiple Haste or Hindered perks in the same loadout.*


### Trial Drop-In

- Players who have disconnected from a still-ongoing trial now have the option to Reconnect in place of the "Ready Up" button for the duration of the trial
- Added a check-box next to the Ready Up button to opt-in to being queued into on-going trials, where you will take control of an existing bot with their loadout after a player has disconnected from the trial for a Bloodpoint bonus
- Added the option to take control of Bots while spectating after dying for a Bloodpoint bonus
- Enabled killer bots, enabling usage of the above system for killer while providing survivors the Abandon option in the meantime
- Survivors who have received 3 AFK Crows are now automatically replaced by a bot

***DEV NOTE**: Trial reconnection is one of the longest requested features, and it's implementation has opened up the potential for multiple drop-in mechanics. There are a variety of reasons why someone may need to disconnect from a Trial due to unforeseeable problems, and having a way to continue playing with your team once everything is sorted decreases the amount of time waiting for friends to finish up as well as the amount of time players spend playing with bots. This also provides an option for sacrificed survivors to hop in and keep helping their team by taking the place of an existing bot, and for players who don't mind the unpredictable loadout and situation to find a trial quicker all while gaining extra Bloodpoints.*


### Abandon Options

- Added the following abandon scenarios:
  - As Killer: once the End Game Collapse has started
  - As Survivor: once the sacrifice animation has started
  - As Survivor: once the mori animation has started
  - As Survivor: if all other survivors are bots

***DEV NOTE**: The abandon system has been a great success so far and in the interest of respecting player time, we've decided to add some additional options. All of these conditions are meant to enable abandoning once your presence in the match no longer affects it's conclusion.*


### Bloodlust Reduction

- Removed Bloodlust tier 3
- Increased chase time required to reach Bloodlust tier 2 to **30 seconds** *(was 25 seconds)*

***DEV NOTE**: In the years since Bloodlust was introduced, it's main purpose has decreased in necessity through the addition of window entity blockers and improvements to tile generation. These changes should incentivize killers to use their power more in chase, while ensuring Bloodlust still functions as a safety net in tile generation edge-cases, even for lower movement speed killers.*


### Exhausted Penalty

- Now increases survivor volume by **50%** while Exhausted
- Now causes running grunts to played for twice as long

***DEV NOTE**: Previously there was no direct penalty for being Exhausted, resulting in Exhausted-inflicting unlockables having no effect if the survivor doesn't have a perk disabled by Exhausted equipped. This change resolves this edge-case, slightly increasing the strength of Exhausted-inducing unlockables and slightly decreasing the strength of perks that cannot activate while Exhausted.*


### Flashlight Quality of Life

- Reduced stun buffer at the end of the killer pick-up animation to **0.1 seconds** *(was 0.4 seconds)*
- Now fades flashlight beams in and out when clicking and un-clicking
- Removed minimum flashlight beam on-and-off hold-time
- Added a brief delay before you can re-click a flashlight after turning it off

***DEV NOTE**: These changes are intended to address the main pain points surrounding flashlights while playing both roles. For killer, flashlight rescues have long been easier to accomplish than avoid particularly at lower experience levels, this decrease in stun buffer will require more precise timing from survivors to succeed a flashlight rescue attempt. For survivors, photosensitivity safety measures have been adjusted to allow for extremely brief flashlight clicks, enabling their use as communication tools for survivors outside of a party, and improving the feel of using them across the board.*


### Bloodpoint Adjustments

- Removed bloodpoint Category caps *(was 10,000)*
- Added a new combined cap of **50,000** *(was uncapped)* bloodpoints per trial before offerings
- Survivors in chase now receive **25%** of the Objectives and Altruism score their teammates receive during the duration of the chase
- Retired Bound Envelope
- All offerings now grant bonus Bloodpoints to all players
- Category-specific bloodpoint offerings now boost the matching opposing-role category
- Increased the effects of all category-specific bloodpoint offerings by **+100%**
- Decreased Survivor Pudding and Escape Cake bloodpoint bonuses to **50%**
- Added dynamic bloodpoint bonuses for the **10** lowest playrate killers, ranging from **+250%** to **+25%**
- Added **+50%** bloodpoint bonus while using perks currently in the Shrine of Secrets
- Added a weekly **+50%** bloodpoint bonus to the lowest play rate addons for each Item and Power from the previous week
- Decreased the P100 Bloodweb to renew at **Level 25** *(was 50)*

***DEV NOTE**: The existing Bloodpoint cap currently doesn't reward players for excelling in a specific category of score events, these changes should ensure players are rewarded for everything they do. The chase changes should reward survivors taking chase at high-importance times to buy their teammates time for generators, rescues, and heals, while also communicating the idea that they should do as much of these actions as possible while a teammate is in chase. The changes to personal and category-specific Bloodpoint offerings are intended to encourage more diverse Bloodpoint offering usage, while giving newer players with fewer offerings faster progression. Unlockable-specific Bloodpoint bonuses should incentivize usage of less-played characters increasing diversity in trials and guiding players to try different unlockables than what they're used to, while giving newer players a method of hastening their progression while gathering more diverse experience with a variety of unlockables. As a result of these changes and to encourage item and addon diversity at high MMR, the P100 Bloodweb now resembles a Level 25 Bloodweb instead of Level 50.*


### Shrine of Secrets Improvements

- Perks belonging to original characters no longer appear in the Shrine of Secrets
- Perks in the Shrine of Secrets now rotate in a consistent order
- Universal Perks now appear in the Shrine of Secrets
- Perks in the Shrine of Secrets can now also be unlocked for **125 Auric Cells** per tier

***DEV NOTE**: It's been a long time since the Shrine of Secrets has received many changes, and we want to give it an overdue update. These changes are intended to make the availability of licensed perks through the shrine more consistent and provide an alternate solution to players who are only interested in a small number of a licensed character's perks, and not the character themselves.*


### Player Loyalty Customizations

- Added unique Badge Borders based on player Devotion
- Added the option to equip prestige crests from previous prestiges

***DEV Note**: We know experienced players are always looking for ways to show off their accomplishments. While we are limited in what customization options can be made available across all original and licensed characters, these additions should provide more customization options and allow players to show off their general experience level in a non-character specific way.*


### Prestige Sacrifice

- Added the ability to Sacrifice Prestige 100 characters up to 6 times, resetting them to Prestige 9 and unlocking one of the following cosmetics each time:
  - Sacrificed Torso/Weapon, Sacrificed Legs/Body, Sacrificed Head/Mask, Sacrificed First Perk Charm, Sacrificed Second Perk Charm, then Sacrificed Third Perk Charm. Sacrificed cosmetics (including charms) are similar to the character's default cosmetics, but with a blue variant of the Legacy pattern.
- Sacrificing a P100 character will result in the loss of all non-event and non-retired unlockables
- Grants **1,000,000** Bloodpoints per **10,000** sacrificed unlockables, up to a maximum of **75,000,000 Bloodpoints**

***DEV NOTE**: It has been a long time since new prestige cosmetics have been implemented, and we've seen players' commitment to gathering multiple P100 characters! We want to provide players who've gone above and beyond a way to display the love and commitment they have for their favorite characters. Learning from the legacy prestige system years ago, we wanted to ensure players didn't lose their relics of the past, and give players who continued pouring Bloodpoitns into a character past the maximum prestige a head-start.*


### Inventory Quality Of Life

- Now automatically equips a starter add-on when finding a trial if you have an add-on equipped that has zero remaining.

***DEV NOTE**: Everyone has had that moment of loading into the trial only to realize one of your add-ons is missing. This change should remediate this by ensuring you at least have something in it's place.*


### Maze Tile Quality of Life

- Maze Tiles are now guaranteed to have a unique number of pallets and windows

***DEV NOTE**: The recent changes making all Realms draw from the same pool of maze tiles has provided significantly more tile options to select from across different maps. This has made it realistic to not only ensure no repeat tiles, but ensure that all tiles have a unique number of pallets and windows. This should reduce repetition per trial by increasing maze tile diversity, and decrease the likelihood of an overwhelming number of very strong or very weak tiles.*


### Pallet Density Quality of Life Improvements

- Adjusted the MacMillan Estate, Autohaven Wreckers, Crotus Prenn Asylum, Haddonfield, Backwater Swamp, Red Forest, Ormond, and The Decimated Borgo realms in the following ways:
  - Reduced the maximum number of pallets and further reduced the minimum number of pallets
  - Enforced a maximum distance between pallets

***DEV NOTE**: We've heard your feedback surrounding the recent Pallet Density Quality of Life Improvements from 9.2.0 and have made some changes accordingly. We've reduced the number of pallets, while enforcing a maximum distance between pallets to reduce the presence of deadzones while keeping the total number of pallets in check.*


### Match Disconnection Quality of Life

- All players without any disconnection penalty points:
  - Now receive a 10,000 Bloodpoint bonus when completing a trial
  - Are placed in a priority queue based on the number of out-of-party players who disconnected from their previous trial
  - Are placed at the front of a Priority Queue if an out-of-party player disconnects while loading

***DEV Note**: Players disconnecting early is never fun, these changes are intended provide an incentive to players who don't disconnect, while easing the blow on players in trials with disconnections.*


### Totem Improvements

- Blessing Boon Totems and Cleansing Hex Totems now display a variable level of glow based on the action progress
- Existing Boon Totems can be Blessed at **+100%** speed to add effects from previouisly missing Boon perks

***DEV NOTE**: It's not secret that over time Boon perks have become overshadowed by other perk options. Our goal with these changes is to increase the viability of running one or two Boon perks, enabling survivors to spread a full "Boon build" across multiple survviors without putting all of their eggs in one basket.*


## UI

### Communication Improvements

- Enabled text chat for players on Xbox, Playstation, and Nintendo Switch
- Text chat is now available during Trials
- Added speech-to-text dictation, allowing players to hold the Voice button to dictate what they'd like to send
- Added an 8-axis quick communication wheel to send customizable preset messages to your teammates
- Updated several Survivor and Killer perks to account for these changes

***DEV NOTE**: One of the major difficulties faced while balancing survivor and killer is the difference in coordination between four solo survivors and a full team. These changes should ensure that everyone, regardless of party size or platform, is able to communicate with each other effectively, enabling much better balance at the high level without diminishing uncoordinated survivors' potential to win.*


### Teammate Loadout Previews

- Survivors can now see other survivors' loadouts in the lobby screen
- Updated several Survivor perks to account for these changes

***DEV NOTE**: We know the lack of information about out-of-party teammates' loadouts can be frustrating, especially when knowledge of a perk or item could have changed the outcome of a Trial. This change should prevent these situations going forward, enabling solo survivors to play around each other's perks as if they're in a coordinated team. This has the added benefit of enabling perk balance around the idea of all players being aware the perk is in play, and we've adjusted some perks with that in mind.*


### Player Portrait HUD Improvements

- Added the killer's portrait above the survivor portraits, revealed to all survivors upon first chase
- Added a persistent loadout display to the player portraits portion of the HUD, displaying perks, items, and addons as they're encountered
- Status effects shown in the portraits portion of the survivor HUD now display timers
- Survivor status effects are now shown to all survivors in the portraits portion of the HUD
- Status effects that are killer-inflicted or associated with a perk notification are now shown to the killer with timers in the portraits portion of the HUD
- Updated several Survivor and Killer perks to account for these changes

***DEV NOTE**: The HUD has only shown the Broken status effect for a long time, this now supports all status effects, with timers. Additionally, once a survivor first enters chase, all survivors will now be able to see the killer's portrait in the HUD, further increasing available information with communciation. These changes are aimed at reducing the difference in information available to solo survivors compared to full teams, making balancing easier overall. To compensate, killers are now able to see the status effects they inflict (with timers) and some perks have been adjusted accordingly.*


### HUD Bar Improvements

- The HUD bar now displays partial healing and mend progress persistently
- The deep wound bleed-out timer is now an outline around the bar itself
- Survivors' resolve meter is now shown as an outline around the hook stage bar to all survivors
- Updated several Survivor perks to account for these changes

***DEV NOTE**: These changes are intended to reduce the difference in information available between solo survivors and full teams, and keep the bar behavior consistent between different interactions. This should reduce how often survivors attempt to unhook while the killer is nearby, slowing resolve progress.*


### Perk Notification Improvements

- Added notifications for more perks on first encounter
- Now shows killer perk notifications to all survivors on first encounter
- The names of icons shown in the Player Effects section are now shown in the upper right corner of the HUD on first encounter

***DEV NOTE**: We know it can be frustrating to not understand why something happened, or need to guess between a few potential unlockables. Our intention with these changes it reduce the frequency where you end and interaction without knowledge of what affected it, helping both new and experienced players grasp the unlockables at play in a given Trial and what they do, while reducing the difference in information available to solo survivors compared to full teams.*


### Revealed Status Effect

- All forms of aura reveal now inflict the Revealed status effect for the duration
- Updated several Survivor and Killer perks to account for these changes

***DEV NOTE**: The Revealed status effect has been a major success in 2v8, helping new players recognize they're visible to the opposing role and experienced players identify what is revealing them. It's time for this status effect to be introduced into 1v4, some aura-related perks have been adjusted accordingly.*


### Settings Improvements

- Added independent volume sliders for different types of audio
- Added an audio quality option to audio settings
- Added separate quality settings for different categories of visuals
- Added an Aim Assist section under Accessibility, with "Prompts", "Basic Attacks", and "Killer Power" options

***DEV NOTE**: PC players already had the ability to manually edit their saved settings and adjust specific quality levels, these changes should ensure all players are able to do so, regardless of platform. Additionally the audio customization should increase accessibility for players who are hard of hearing or misophonic, helping existing players and opening the door for new players to come into the fog. We've also included the option to selectively disable Aim Dressing/Aim Assist for the following scenarios; 1) Interacting with a prompt (such as a window, pallet, hatch, or generator) based on look-angle rather than proximity, 2) Automatically swinging when within range of a survivor as well as smoothing the camera towards the center of the survivor on-swing, and 3) Killer power aim-assist interactions, such as during the Ghoul's Kagune-Leap.*


### Queue Time Estimates

- Added an estimated queue time while searching for a trial

***DEV NOTE**: This was first trialed in 2v8 v5 and worked extremely well, you can now expect to see this in your 1v4 matches as well!*
