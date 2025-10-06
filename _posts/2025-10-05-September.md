---
layout: post
title: "Inching Through September"
date: 2025-10-05
tags: [Life,Research,Gaming]
---

# Steady Progress in Research Land
While I've been awaiting approval of my (Run 3) simulation files, I've been steadily working away at the other parts of my analysis. I took the advice from the PAG
and revisited my pairing and cut analyses. While validating typos in my particle reconstruction (pairing code), I accidently found a large collection of MC (Simulation)
samples that neither I nor my advisor were aware existed. Apparently, his old student at Rutgers had commissioned more files to be generated than we were aware of.
Thankfully, this speeds things along significantly. 

We went from having only a couple mass hypotheses for Run 2, to a whole range (200-3000 GeV) becoming available. This means we can do fun things like make predictions/set initial limits on cross sections. 
Upon getting access to these additional files, further complications did come though. 

We came to find the pairing algorithm we had been using prior, does not work very well for these higher mass signal hypotheses. 
My way of resolving this was making a very crude classification algorithm that determines which reconstruction method to use based on the angular separation of each pair of photons. I also redid the cut analysis following this. I found that rather than one "best cut" applying to all my signal files, I have two signal regions to apply cuts on.

Along the way of revisiting these parts of my analysis I converted all my research code to using Coffea/uproot. It was rather impressive how much of an performance uplift I got. My "best cut" gridsearch code now takes vastly less time (< 10 minutes is great). The file processing is amazing now as well. I can plot the best cut of 1 fb<sup>-1</sup> of ECAL data (> 30 GB) in only a minute. 

I have done some attempts at preliminary limits to varying degrees of success. One issue I got after realizing a typo in my code is that my statistics were extremely low. So, rather than apply a PhotonID (it's a Machine Learning/MVA tag trained on resolved/merged photons) to every photon, I just started applying to leading photons in each event. After getting some solid results for this, I started looking for a real starting point. 

This led to a trigger analysis. This involves downloading an unbiased dataset (such as datasets that trigger for Electrons or Muons) and comparing the trigger I'm using for my analysis relative to another trigger in another dataset. After doing this it seems I need to start my analysis around 250 GeV (so guess we're missing out on the SM Higgs to Pseudoscalar). 

Overall, things are progressing smoothly. It won't be long until we start looking to ask for the full dataset. FNAL work is steadily moving along but there haven't been any significant jumps forward. We're still waiting on other aspects of panel construction to catch up.

# Other happenings
I ran back through the NW Ohio area for my usual 'once a month' trip last weekend (for my dad's birthday). It was good time, saw family and caught up with friends. Had originally planned a second trip earlier (for my mom's birthday), but schedules didn't quite line up. There was also an on campus game night earlier this month, that was pretty fun. It wasn't the most eventful month but things are going fine. 

Next month I have a bunch of people asking me to do things so we'll see how eventful that gets. 

I do have an update on my weight loss though. I'm at just about 40 lbs (~18 kg) lost since May. I'm sitting around 185-186 pounds right now. 

# Game Updates 


## Assassin's Creed Odyssey

![](https://i.imgur.com/crogrhR.png style="width:50%")

This game sits in a strange spot for me. Contrary to initial expectations I quite enjoyed Origins. This game isn't bad, but I enjoyed it to a lesser degree.

Gameplay wise, it built upon the gameplay elements of Origins for the most part. Occasionally one could tell they just haphazardly tossed a gameplay element from Origins (or other AC games) with little thought to it making sense. The combat sometimes feels like an improvement, while other times doesn't (due to bugs). It normally feels pretty standard but I think there are three aspects worth discussion; mercenaries, ship combat, and the quest system. 

Of all the gameplay elements, the Mercenaries system feels to me like it had the most potential for greatness. Unfortunately, it doesn't quite get there and that's likely due to the Nemesis system existing in the Middle-Earth games and being copyrighted. One can clearly see the inspiration in the Mercenaries system which has evolved from the Bounties system that has been in AC since AC2. I actually quite like the concept for the Mercenaries system here and how they play a role in the war battles. I found myself thinking this would be perfectly at home in a <i>Berserk</i> game. The biggest thing weighing down on the execution of this system is the HP/stat bloating of mercenaries and the spamming of them in sometimes obtuse combinations. They feel more like a chore at times.

The ship combat makes a return in this game. Ship combat very clearly peaked in Black Flag. It disappeared after BF/Rogue for a time before coming back very shortly in Origins. Here, we see a barely upgraded rendition of the ship combat that briefly appeared in Origins. The ship combat here would be more acceptable had we not experienced the highs of Black Flag. However, here we feel like we're playing objectively worse gameplay. Fortunately, I can give them the benefit of the doubt on this being narratively sensible. It's passable, but not great here though. 

Perhaps one of the worst aspects of this game is the amount of dogwater tier side content. This is especially evident in the side quests be them the ones Ubisoft 'curated' or the user-created ones. The amount of times they reused lines/concepts and just had generic quests of "kill them all, it will solve everything" drove me up a damn wall. The user created quests were not any better. I completely agree with the concept of them existing, but the majority of them were a complete waste of time. 

Now, let's talk story. I played as Kassandra and during the mandatory story quests she's solidly written most of the time. When the game keeps the current day and past portions separate, it does well. It isn't the most revolutionary narrative but it gets decent marks. Unfortunately, this is thrown away by the introduction of plot elements that effectively retcon the entire AC series while also bringing every past event into question. 

I left this game feeling conflicted, but to the degree that I'm ready to stop playing the series. The best I can give this is **7/10**.

## Tony Hawk's Pro Skater 3+4

![](https://i.imgur.com/sbj0Sef.png style="width:50%")

There was a lot of fun had here, but admittedly was not a perfect remake. At its core the Pro Skater 3+4 remakes are more of the same clean gameplay we saw in the Pro Skater 1+2 remakes, with some minor differences. The core gameplay is very clean with very solid challenge and multiplayer options. 

The two biggest points of contention are the handling of the Pro Skater 4 content, and the soundtrack. The music choice in this game is a bit of back and forth. I think perhaps the weirdest addition was the "stream-friendly" music which all sounds like generic corporate slop. The pidgeonholing of Pro Skater 4's gameplay in the Pro Skater 1-3 mold does indeed leave a bad taste in the mouth. Particularly, the reduction of levels like Kona and Zoo into just competition levels. That being said the new levels are quite fun. 

Perhaps a larger gripe is that the content reduction in the Pro Skater 4 levels (such as the reduction of stat and money pickups) drastically reduces the amount of time required to clear levels. This is partially remedied by the existence of Pro Goals. However, I feel the existence of Pro Goals and additional challenges already served as a consolation prize for the lack of the character specific goals in Pro Skater 4.
However, the game is still a lot of fun. It's a shame the studio that made it got shuttered basically immediately upon release. It is getting a **8/10** from me.

## God of War (2018)

![](https://i.imgur.com/bZ3X94B.png style="width:50%")

This game was solid. God of War has always been a 'middle shelf' tier series for me, and this continued here. 

The first thing worth noting here is that in terms of tone and gameplay, it is a stark departure from the original trilogy. This is not necessarily a bad thing, but it has to be acknowledged. The difference is something you confront when judging ones expectations. 

The characters and writing existing in such contrast with the original trilogy is what makes it work. Kratos' evolution as a character is one of the core high points of this game. In terms of characterization, the main gripe I had here is the pacing of character interactions. This is best exemplified in the interactions of Atreus and the blacksmith brothers with Kratos. Often what I observed is that the character arcs, behavior, and/or tendencies of each character in this game tend to go on for just long enough to get grating. This was especially apparent with Atreus' edginess around mid to late-game. 

One aspect of the characterization in this game that I have more mixed feelings about is the usage of Kratos and Atreus as a mirror for the player. In theory, I think it is sort of smart to use the conversations that the lead duo have as a feedback system for the player. However, just like pacing sometimes it goes a bit too far; such as in Atreus solving a riddle that should be left to the player to solve. It's definitely a fine line that's hard to walk correctly.

The overall story the game was telling I found quite solid, although it is definitely a hard ask for one to compare this game to the highs of GoW 2 or 3. However, there is a bit of back and forth between the old and newer games in terms of what qualities each does better. While this game is objectively a prettier, better looking game than anything in the previous games it has much less in terms of spectacle fights. 

This now brings us back in the direction of gameplay. I found the gameplay to be solid, but not quite as satisfying to play as the older games. My main arguments for this would be the lack of enemy/boss variety, occasional HP bloat of certain enemies/bosses, and some more general combat design issues (weird hitbox placements, stunlock potential, etc.).

I definitely enjoyed this game though and will be playing the sequel. 

This one gets **8.5/10**

## Marvel's Spiderman (2018)

![](https://i.imgur.com/S6DaR6Q.png style="width:50%")

This was a short but sweet experience. Ironically, the best aspect of this game for me has little to do with the common praises. 

To be quite frank, in terms of the core gameplay and character for Peter this game does little that hasn't already been done to death by prior Spiderman games. In fact, I booted up one of my old favorites, <i>Ultimate Spiderman</i> to verify this; The webslinging has always played like this. Legitimately, the core difference is on the level of button binding differences. The combat is different for a Spiderman game, but not new to superhero games in general. The counter based mechanics are at home in the Arkham series, which went on to inspire countless other games. 

In actuality the biggest things I give this game props for is in developing the genius side of Peter Parker, and in propping up Miles Morales to come onto the scene. In fact the best aspect of this game, is actually the scientific minigames. They're not so accurate as to be taken literally, but are rather competent. The spectroscopy minigame took me right back to my days in the lab as an undergrad. 

The biggest crime is in the game having so little content for a Spiderman game. Personally, I would prefer a more stylized/comic art game than photorealism though. I'm giving this an **8/10**.

## Bloodstained: Ritual of the Night 

![](https://i.imgur.com/wUc0bCR.png style="width:50%")

This was another mixed bag of a game. My first impression of this game was rather rough, as the first level/region borderline gave me motion sickness due to the artstyle (and the swaying). This improved significantly with time before coming back down for entirely different reasons. 

If all you want is more of what you got in Aria/Dawn of Sorrow, this will be your jam. If you want something novel, that moves the medium forward look elsewhere. 

While this game has a lot of interesting ideas, none of them are executed well enough to raise this game to its fullest potential. In fact many of the ideas expressed in this game do naught but make the game easier to cheese (Optimizer and Invert bust the hell out of this game).

This is also not helped by retreading so much of the same character concepts and plot beats from prior CV games, that you'd be hard pressed not to accidently confuse details. 

It was alright, but I would honestly recommend just playing Aria or Dawn again over this. **7/10**

## Katana Zero

![](https://i.imgur.com/URsiafS.png style="width:50%")

This was a short but very sweet experience. I don't have much to say as there was little to criticize. 

The only criticism I have is that doing stealth on the Prison level sucked.

It had great gameplay, art, music, characters, and story. My biggest gripe is that I have to wait for a DLC to get the true conclusion. **8.5/10**

## Control

![](https://i.imgur.com/Pf62HAH.png style="width:50%")

I went in here with tempered expectations and left with a very mixed impression. I'm well aware that Control is part of a shared universe with <i>Alan Wake</i>,
which I also have mixed opinions on. I have similar mixed opinions of Control for a variety of different reasons. 

Ironically, my first impressions of Control were vastly better than those I had with Alan Wake. It's a beautiful game, that normally isn't all that frustrating
to play. The execution of the mysterioius and unknown is even reminiscent of <i>The X-Files</i> and <i>SCP</i>. However, as the playtime racked up it lost its
luster. 

The gameplay upon a glance is fine, but does get repetitive and tiring with time. This is a consequence of maintaining the style of 'waves of enemies' that Remedy often does. I oftentimes found myself being more annoyed that there were still waves of enemies coming than anything else. This is definitely less frustrating to deal with as opposed to the resource management in the original AW though (I never played the remake). My larger issue is with what actually HAPPENS in the game (or lack thereof).

Over the course of the game we are working alongside Jesse as she tries to save her brother. Jesse as a character is explored to a competent depth, but the same does not extend to everyone else. In fact the game goes out of the way to portray Jesse as not caring of the plights of those working for the Bureau. She also is portrayed as not caring to understand what's actually happening either. It all made it very difficult for me to care about anything that was going on in the game after a certain point. 

This was further cemented when upon concluded the game's main story, nothing is really concluded. 
This was a really weird game, and I get that THAT's the point (being weird-fiction and all). However, there is something to be said of there being as much as there is to the game but still being left feeling like "What actually happened in this game?" I understand that if you take all external media into account there is supposed to be some greater meaning to be had here, but judging it on its own merits leaves it questionable at best. 

I think a possible high point is artistic execution though. The color space utilization in this game is definitely next level, and the more surrealistic level design was pretty cool.

Overall, my opinion was that it has better gameplay than Alan Wake but worse writing. Personally, **7/10**.

There were other games I played and dropped in September, but too much to really cover there.

# Stream Updates 
Not too much to say here. I haven't been streaming all that much but plans at present are continuing Trails streams as well as picking up more Retro PC streams. 

I'm thinking possibly doing full plays of <i>Wolfenstein 3D</i> and <i>Dragon Wars</i>.

That's about it for now though.

Till Next Time,

Rob



