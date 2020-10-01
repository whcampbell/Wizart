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
