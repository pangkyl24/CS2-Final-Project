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
Goals(s): 

4/29/21: Day 11
