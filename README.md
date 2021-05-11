# CS2-Final-Project


4/19/21: Day 1
Goal(s): Deciding on my Challenge project
Result: Video Game using Scratch. Two-Player, Battle game. Started Creating some of my Sprites

4/21/21: Day 3
Goals(s): Determine Sprites, Start Programming
Result: I was able to determine the the focus of my video game along with choosing the 4 main sprites that will be used. Focusing on animals, I had designed a snake, bat, penguin, and bear to "battle" against each other in a 2 player game. I was able to program the character selection process that would be used in the beginning of each game along with some basic character movement features. More modifications will be required on movement for later. 
Notes: I spent Day 2 getting more comfortable with the software, as I hadn't used scratch that much. During the programming process, I did run into a small issue. I had difficulty making my sprites appear after the character selection process. It was a small programming error which just required a small amount of debugging to fix. 
Important Lesson: Order of code MATTERS.

4/23/21: Day 5
Goal(s): Further refining of program
Result: I had difficulty implementing a gravity system that worked without the game looking weird with obsure movement issues so I decided to remove the gravity in my game completely. The game originally was going to have movement where player controlled sprites could move up, down, left, and right but both the movement and pvp I had originally planned seemed a little weird in a 480x360 grid so I decided to settle with just up/down movement.
Notes: I wasted a lot of my time debugging certain issues during this process. These issues weren't very major, but enough to annoy me so that I spent the time to debug. This told me that I should definitely be debugging AS I program not AFTER I program. The major issue was trying to configure the bat sprite's flapping animation. I wanted it to flap only during certain moments making it a little more difficult as I can't just add a forever loop. 
-> I also implemented a pretty nice/useful variable today called "curEvent", which keeps track on what phase the game is in. This should make situational codes easier to implement.

4/25/21: Day 7 
Goal(s): Research
Result: I spent the day researching different ways to present a proper health bar in scratch. Obviously the simplest way would be using a variable to represent the health but that method doesn't look visually pleasing. So, I spend a few hours poking around other people's projects, forumns, and looking at code for inspiration. In the end, I decided to take inspiration from another user named, TheLogFather, and his project, "Health bar with pen"(https://scratch.mit.edu/projects/18482376/editor/). I decided I would use the same idea to draw my health bars. I wouldn't copy his code, but just the idea.
Notes: I probably won't be programming the Health Bar feature until much later into the project when the main feature have already been finished, however this experience opened my eyes to the many ways one can solve the same problem.

4/27/21: Day 9
Goal(s): Basic Projectile
Result: This time I added what would be the most important part of my project, an attack system. Today's code was relatively simple, just a simple projectile that could be sent from both players with the keys, "d" and "left-arrow". The attacks work by creating a clone of the sprite and moving straight forward. Once the projectile touches the edge, or another sprite, the clone deletes itself. It's like apoptosis, but for a series of 1s and 0s. If it were to touch another sprite, that sprite would take damage. If the projectile touches another projectile, they would both be deleted. A buffer was also added in order to prevent attack spamming.
Notes: A few small bugs popped up as I was programming. The first being the collision of projectiles. What happened was that when the projectiles collide, only one gets deleted, so what I did was make the projectiles stop of 0.05 seconds to ensure that they BOTH collide and delete themselves. The other was the buffer feature, in the end I had to create a delay/timer variable to accurately implement the buffer

4/29/21: Day 11
Goal(s): Special Attacks pt.1
Result: Today I decided each of the avatars would need something to make them stand out. This would be... Special Attacks!!! I spent the day brainstorming Ideas for special attacks and decided what they should be. Bat: Weaken Effect (Less Damage Per Hit), Bear: Massive Damage (Does lots of damage), Snake: Poison (Opponent can't use other attacks for certain period of time), Penguin: Slow Effect (movement speed slow). And with this, I would need to introduce a few special variables (p1_dmg, p1_speed, p1_status, p2_dmg, p2_speed, p2_status) along with a timer(cooldown) variable to prevent spam (p1_sp_timer, p2_sp_timer). So I spent the day designing sprites/costumes and adding new variables and replacing certain integers with these variables (ex. change p2_hp by -5 : -> change p2_hp by p1_dmg).

5/1/21: Day 13
Goal(s): Special Attacks pt.2
Result: I programmed the entire special attack section today. Took a while but I was able to complete it. I basically used most of the code from the Basic Projectiles but modified it so that the special attacks are quite a bit different (inflict status effects). In order to do this(inflict status effects), I had to create a few methods in order to make this work(run_sp_attack, inf_slow, inf_poison, inf_weak). The only annoyance about this is that the methods are exclusive to each sprite so I had to copy and paste the methods in order for them to be "global", even so, a few small modifications were still needed. No major issues, however, I did learn that debugging AS I go along is a good idea. Debuggin large strings of code after finishing a section is very time consuming and inefficient after all.

5/3/21: Day 15
Goal(s): Ultimate Attack pt.1
Result: Special attacks have been implemented, now it is time for ultimate attack. These are the game-changing attacks which will turn the tides of battle if they connect. In order for this to be successfully implemented, these attacks must be visually appealing and apply powerful, thoughtful effects. Bat: Weaken + Poison, Bear: Instant Win, Snake: Reset Charge for Opponent Ultimate, Penguin: Extremely long Slow. Some of these abilities may seem overpowered, but the attacks are avoidable and quite balanced if you think about it. I tried giving each sprite it's own niche (Snake does an especially nice job at preventing the opponent from attacking...etc.) along with making the effects bland in nicely with the game. Similar to day 11, I didn't actually do any programming, just some sprite/costume design andthe addition of new variables. This time, my idea for the ultimate is no longer cooldown based, but it is damaged based. Once you have successfully damaged the opponent by 4 times with your basic attack, your Ultimate will be charged and ready for use.

5/5/21: Day 17
Goal(s): Ultimate Attack pt.2
Result: Much like day 13, I was able to finish the entire Ultimate attack section. This was actually relatively simple as I was able to use the methods created on Day 13 with a little bit of "Globalization" (Copy/Paste into each sprite's code + a few modifications). No issues, the entire process went smoothly without me having to grind my teeth in annoyance at every little issue. 

5/7/21: Day 19:
Goal(s): Health Bar + Ultimate Charge
Result: Today I decided to actually implement the health bar into my game. I did this first by creating another project in scratch(https://scratch.mit.edu/projects/521962307/) to test the health bar. Once I was satisfied, I copied the code(manually so as to not have any issues) into my project for implementation. For the charging of the ultimate, instead of using the "draw" tool, I decided to use a sprite that would switch between costumes depending on the stage the ultimate is charged in. This wasn't much of an issue but the health bar was a HUGE pain. I had quite a difficult time understanding what each block did. I'm unfamiliar with the code afterall.

5/9/21: Day COMPLETE!!!
Goal(s): FINISH THE PROJECT!!!!
Result: I Finished!!! There wasn't much to be added today, just a few finishing touches and an end-game screen. It was pretty easy compared to everything else. I'm just happy this project is finished. 



