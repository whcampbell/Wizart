# Wizart Gaem

### We're back at it again
Work has started on a third game, and it's not just mine this time. May I introduce...

## The Team, POGLAW
Pascal King - the art / the brains <br>
Owen Wolman - well versed in the trade <br>
George Khankeldian - he's george <br>
Laura Garling - the cool one <br>
Andrew Castelino - wants to do the music(?) <br>
Will Campbell - had the idea (and will provide moral support)

I'll be working with these wonderful folks to make a much bigger project than the ones before! We're still early on in development, so no builds 
to show yet. This will only be a log for now. Keep on coming back to see what we can do!

[Back to the Castle](https://whcampbell.github.io/Ivys-Castle/)

### Meeting 1 - 9/17/20
For the first part of the meeting, Pascal, Owen and I built up the design doc, discussing possible creative and gameplay ideas. Our plan is a top-down 
magical survival game. The player will have to use various spells and manage their mana in order to fight back the approaching enemy horde 
while navigating an expanding map.

Once everybody got to the office we began with the housekeeping and setup work. First we decided upon VSCode as our IDE. After that there was 
much sharing and inviting, including a github repo, trello board, and the design doc. Owen also got us rolling on GitKraken. Since some of us
hadn't used any of this stuff before (me included, I'd never used trello or kraken), Pascal and Owen stepped in to give some lessons. Pascal
gave us a quick explanation for trello and Owen did the same for Kraken. Pascal then started on the setup for the repo, building up the vital 
structures for engine, rendering, etc. My important contribution was the decision of the trello board's background. 

A successful first day. 

oh yeah I also drew this

<img src="./Load_Screen.png"/>

### Meeting 2 - 9/24/20

We were trying a while to get things to compile, but it was difficult to do across multiple platforms. Andrew and Pascal were doing most of the heavy
lifting on that, researching CMake to get a makefile going. Pascal also set up the code to have a game window pop up, but it couldn't be compiled
for the aforementioned reasons. The people using mac had to do some research on gcc (g++ really) that we could use. It wasn't going all too well,
the download for clang took about five million years and there was nothing else we could do but sit around. We're all excited for when we get out
of these woods here so that we can get to some normal programming and not twiddling our thumbs waiting on new software. 

### Meeting 3 - 10/1/20

Very brief meeting today, still working on compilation. The mac people all got cmake downloaded, but xcode was being iffy. We needed Owen to lead
us in our journey through the downloads and updates. Laura and I had yet to get xcode, but I needed an OS update and Laura was just having
issues with the download on that bad boy. Therefore both of our computers were out of commission. Andrew was working on the makefile once again, 
but he needed to get his combinatorics done so he couldn't work long. Pascal set up a metafile generator for importing sound effects and sprites, 
he's MVP today.

<img src="./Waiting.png"/>

### Meeting 4 - 10/8/20

Finally got C++ to compile on mac. This took way too long. Owen was correct that what we needed to do was download xcode so as to get all the 
necessary libraries. After that it was just installing the c++ extension on vscode and the hello world was off to the races. Pascal, Owen, George 
and I then made some creative decisions. Pascal had drawn up some concept art for the main character and we all decided on which option we liked,
and then we decided that we wanted random rogue-esque room generation. We had to go through some issues of this though, mostly scalability.
This map could grow real big, and in order to save it we had to do something about efficiency. Our decision was to select rooms randomly from a 
pool. The map will be made of tiles, however, so when a room is added it is no longer a room, it is just a bunch of tiles. Then, when the map is
saved, it just needs to be compressed down. We decided that rooms could be created without a GUI, and then they can be loaded with a set-size 
chunk system. I wanted to look up alternatives, but google failed me. Turns out not many people are trying to be indie game developers. Ope. 

<img src="./characters.png"/>

Owen also got a new role. He is now the creative writing lead! He wanted some story, and I thought that putting some lore collectibles in the 
game would flesh it out a bit so I agreed. Andrew was dealing with cmake still, he concluded that no intelligent person has ever used cmake. 

p.s. Owen is also the programming director. He also has the right to hand that role off like a hot potato. Will remains creative director. 

In fact, lets assign the roles. 

Pascal - Art Director, Game Dev Expert, Engine Lead <br>
Owen - Writing Director, Programming Director <br>
George - Associate Developer <br>
Laura - Associate Developer <br>
Andrew - Music Director, Compilation Expert, Associate Developer <br>
Will - Creative Director, Associate Developer <br>

p.p.s. ONION MAN

### Meeting 5 - 10/15/20

Pascal continued to be the boss of linking and engine setup over the past week. He did the grunt work on getting things to build on mac. A round of 
applause was given to Pascal for his worthy efforts. We also decided to set down some story stuff. Owen raised a few ideas and Pascal put one up as 
well. All this is just to give context to the world: who are we, who are the enemies we're fighting, why are you in the place where you are, et 
cetera. We thought that we could have a narrator trying to kill the player. This way we could spice things up by changing the setting, since the 
world is at the narrator's fingertips. Pascal and I also had some discussion about mechanics, such as what environmental effects we want, spell
interaction, and the mechanics which would force the player to explore. 

New issue came up that things would build on my mac, but not on Owen's. Just needs to update xcode for a better clang version, but needs to 
update his OS first (like what happened with me). Laura is also getting things set up. Update: her build worked just fine. Owen (being the programming
director) and Pascal (being the game design expert) are gonna divide the design into programming tasks for all of us to start working on. From that
point, we'll be able to really get down to the brass tacks. 

### Meeting 6 - 10/22/20

Going through standup, nobody did much once again since the base/engine of the game hadn't been built up yet. Pascal, being the engine master man,
DID go pretty hard this week on knocking out the initial work. There are a few bugs with building the project but things are going pretty well.
Pascal worked out drawing to the screen, playing music, and keyboard inputs. Pascal also educated us on how to work his engine and went through
a test entity. Aside from that, not much. Splitting up the tasks on trello should happen very soon, and work shall be done. 

### Meeting 7 - 10/29/20

The green light has been given! Pascal has told us that everything we need to start coding is set down. We just need to get familiar with the 
documentation and get warmed up with how to use his engine. For the first part of the meeting we figured out the first set of tasks we need to
start on. We went through the design doc to get a bunch of trello tickets going. We worked on how we wanted the UI to look, such as the 
health, mana, and XP bars and the spells as well. After that we split up the tasks. I'm going to build up the class structure for spells, Pascal is 
going to take item drops, I believe Laura is going to take the enemies, Owen is going to work on procedurally generating rooms, and I'm not sure
what George and Andrew are doing. They're probably just gonna take whatever they like off the trello pile. I'm excited to finally get things going!
Just gotta warm up my C++...

### Meeting 8 - 11/5/20

I kinda dropped the ball this week by not getting around to doing much. Turns out everyone had a pretty busy Halloweekend, and Owen couldn't get 
Xcode working. Owen did do some research on integrated databases though, he's going to be messing with SQL (good for C and C++) to get things 
saved real nice. Pascal, being the expert, was hard at work as usual. He drew up some sprites for mana, an enemy, and other item drops, and he 
also did some more engine setup. As project leader, I need to stop Pascal from working. I have banished him to the art realm. He has given me no 
guarantees. Andrew also has an idea for what he wants the sound of the game to be musically, and I'm excited to see what he's got.

Now that we're splitting up to search for clues, Owen gave us the info on branching so we don't destroy the world. We then did a little more 
messing with build on mac (turns out pascal yote the whole engine, thanks version control for getting it back), and now it works like a charm. 
Since Laura and I were kinda daunted by the project the group decided that we should work together on something to figure out how this
whole programming thing works. Laura and I will be coming back to the office on sunday to get some knowledge on coding and project structure 
and we'll get started on a couple of the item drops to help us learn. 

<img src="./Engine_Yeet.png"/>

### Mini-Meeting - 11/8/20

Pascal Laura and I hopped on discord this evening to get some stuff done. Pascal walked us through the structure of his quasi-Entity-Component 
system and we programmed up a couple items on our own. I was doing health, and I had it easy because I could just rip off the mana drop that 
Pascal had already made. Laura took a more difficult route with the Exp drop because we decided that all Exp is gonna be in a big shared pool, 
unlike health and mana which are gonna be separate for each player. Went quite well, I feel pretty good to have my first real code pushed up
to the project. 

### Meeting 9 - 11/12/20

Over the past week we started heating up. Laura and I did our item stuff, Owen made our shiny brand new integrated database, and Andrew brushed up
on mixing to make the music sound pretty. Pascal also did his normal ton of work over the week. He restructured the engine (again) to make sure 
that all the engine stuff we shouldn't see is behind an abstraction wall. He also made a particle system and it's currently showing numbers for
damage when we hit stuff. It's also crashing the game. That should change soon enough. 

Yeah, by the end of the meeting Pascal fixed the particle crashing issue. Apparently the multithreading was bonking itself because it would delete
the object before it got done rendering it (I think, I don't perfectly remember what he said it was). I also knocked out the speed boost drop. It
took a little more production than the health drop because I had to make a new component for buff timers and mess with the player files. I made 
a goof at one point and our little mans began to go at light speed. Ope. Anyways, Andrew started work on random room generation, and Owen and 
Laura were ironing out the experience drop some more. 

I guess George was busy this week. 

### Mini-Meeting 11/15/20

We were all able to get into the same room this time after a while of one or two of us having to discord in. We had a good head of steam going, so 
we all just broke out into our own little projects. Owen kept working on the integrated database with SQL, and Laura finished up the XP drop, 
getting her first commit up on the board. Andrew was working on the tiling of new rooms for procedural generation, and Pascal continued to be big 
brain guy and answered all our questions. What I want right now is to start burning through spells, because I found it was simple enough to kinda 
plug and chug for the item drops. I had to write in the skeleton enemy as a target though. I think my current mission is actually to add features 
to him like a hurtbox (which I should have done already, ope) and a physics driver for the knockback. 

### Meeting 10 - 11/19/20

Owen has a whole sector of the databases done. We decided that we only needed three, one each for mobs, spells, and items. He has the mob one all 
set up. After getting the other two done he's gonna write up helpers to allow the rest of us to easily interface. Andrew's been experimenting with
tiling and he has random generation of one room down. I believe he'll be working on stringing rooms together next. George was back with us this 
week, he's gonna get warmed up by doing item drops for the point system. Oh yeah, I guess we're gonna have a point system to see how well you did
after a run. Pascal is working away at some bugs and also being the font of knowledge that he usually is. Laura is following up on her XP drop and
worked on the display for XP, she's gonna make a nice bar. I coded up a physics component, mainly just for objects to slide around after they 
get hit by stuff. Took a little messing around with the bugs but I'm pretty happy with it. It's starting to look a bit like a game. Maybe I'll make
some recordings and put them up on youtube to give updates... Anyways, here's a good still.

<img src="./Week_10_Still.png"/>


### Meeting 11 - 12/3/20

We took the week of Thanksgiving off. Or at least most of us did. Pascal was hard at work as usual, he must really have a blast with all this. He
put in a log (now flog because ambiguity issues) function for output, added screenshake, and more art stuff like tiling and a couple animations for 
the player. The rest of us got warmed up pretty quickly as well, most of us picking up the same jobs we had been working on previously. I started 
fresh on a new spell for area of effect damage in a large box around the player. Queue lots of shenanigans with particles and a new lifetime 
component. That's pretty much all she wrote for this week. Highlights of the meeting were Andrew creating a "very scary bug" where the frame rate 
dropped to a big ol' zero and any movement of the player just caused the screen to smear, and my discord becoming wack and having "screenshake but 
for audio." These are the drawbacks of a socially distanced workplace. 

### Meeting 12 - 12/10/20

Today is just a short meeting due to finals coming around. Everybody has a mess of projects, early exams, and other assorted tomfoolery. We just met
for standup and to talk about plans for winter break. The mini coding sessions on sundays are gonna become a more consistent thing it seems. Good?
Okay, back to school nonsense. 

### no meeting during exam week. I also got sick. No it wasn't covid. 

### no meeting on Christmas Eve either. 

### Code Meeting - 12/27/20

I believe this is our second meeting over winter break to work on the game together. I haven't been treating these as official meetings because
not everyone is able to attend, but it's all we got right now so I guess I better document stuff. Laura has been working on UI for the XP bar and she
got it all finished up, I believe today she was working on some bugs elsewhere. Andrew had been working on tiling rooms together, I think he's
made good progress but I'm not sure because he couldn't make it today. Owen finished up the database for mobs and has been working on the skeleton
guy that I put in earlier. He's gonna do enemy routing as well, but he can't do much without walls in the map. Pascal has been doing his thing 
with rendering and engine stuff, he also did some animation work. He also fixed my bugs that I put into the AOE spell. Thanks Pascal. 
Speaking of the AOE spell, I finished it up and it's working pretty well with the animation that Pascal put in. I might tweak some constants for
knockback, but what I did today was add an onFire status effect to our component for buffs and debuffs. Works pretty good. I don't know what George
has been doing. Oh well. 

### Meeting 13 - 1/7/21

We were all able to get together this time around. None of us had done much, we were all relaxing with family or working on other projects. 
Everybody got back into the swing of things pretty easily though. George finished up the randomization and display for the score drop, and Laura
plied her expertise from the XP bar to the Evil bar. Have I explained that? Well, we're gonna have an evil bar that fills up if you stay in 
one spot for too long. That will encourage exploration, hopefully. Owen was working on pathfinding at first, but he decided to switch it up and
make some menus. I believe he started with a pause menu. Andrew was still generating rooms and maps, he might be switching to enemy pathing though.
It would work well with what he had been doing, because in order for A* to be effective there needs to be walls in the way. Pascal took my 
request to make a fire sprite so that the onFire effect would actually look like something, and I worked on broadening the elemental effects. I 
started by adding an element component that could be attached to spells, and then to make that work I had to give the player a spell slot system. I 
did the basic structure of that (with a lot of hard coded constants for now) and I plan on working it out further in the upcoming weekend. 

### Meeting 14 - 1/14/21

This meeting was only standup again. I get back from work pretty late these days (not because I work late, the commute is just long) so we had
an evening meeting and everybody had evening plans. I'm okay with that, I just wanted to make sure we had any kind of meeting. The last thing
I want to happen is for everybody to forget about the project and it eventually dies. Anyways I did some work as well, mostly just making the 
spell casting system less cringe. I just had to toss in some helper methods to avoid nested switch statements. The basic structure is all set
up, it just needs to be fleshed out with all the different types of stuff, which I'm excited to do. At work I do QA testing, so I'm not 
gonna be writing much, just looking at other people's stuff. This is kinda sad, because I like writing. Oh well. Money is money, and cash is
king. And I get to write for this project! It's all about the side hustle. 

<img src="./Boom.png"/>

### Meeting 15 - 2/5/21

Been a long time since our last meeting. Felt weird knocking the dust off of this project after what I've been doing at work. We managed to 
do actual stuff today though, more than just standup I mean. Everybody got back to what they'd been doing. Andrew with room generation, 
George with score UI, Pascal with particle effects, Owen with menus, Laura with spell juice, and I started putting another spell in. I'm 
currently satisfied with how the spell slot system is working so I moved on to putting more spells in. I'm happy that we can get back into
the swing of things (hopefully) after getting a bit shaky over break. Wish us luck!
