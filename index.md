---
permalink: //
title: "Home"
---

## Overview

![](/assets/images/startscreen.png)

### Synopsis
Society has crumbled. The World as we knew it is rotting. Strange behavior in the weather finds odd particles of dust set in the very air we breath. Set during the aftermath of a zombie outbreak in the United States, the game pits a survivor and their infected little sister against hordes of the infected. Setting out to do what our primal insticts as humans urge us to do. Survive. However, due to a lapse in judgement, his little sister manages to get infected. Now must he set out to find a cure and save his sister. Hoping to somehow against all odds find an answer for the dust.

![](/assets/images/instructions.png)

### Game Description
Get ready to blast your way through hordes of undead in this pulse-pounding top-down shooter! You'll need to use all your wits and skill to survive seven long days of endless zombie waves, armed only with a variety of fun and interesting items and weapons. But there's more at stake than just your own survival - your sister is counting on you to keep her safe from the zombie horde! It won't be easy - this game is tough as nails - but if you can make it through each day, you'll emerge a true survivor!

![](/assets/images/sample-gameplay.mp4)

### Our Vision
With An Answer to the Dust, our vision is to create an immersive and thrilling gaming experience that transports players into a dark and dangerous world filled with all types of zombies. We aim to deliver a game that not only challenges players with strategic combat and resource management, but also draws them in with rich storytelling and character development. Our goal is to create a game that keeps players on the edge of their seats as they navigate through treacherous environments, and confront formidable enemies. We believe that the combination of intense gameplay, atmospheric world-building, and engaging narrative will create an unforgettable experience for players that they'll want to return to again and again.

## Development

### Projectiles and Shooting

![](/assets/images/shooting-and-projectiles.png)

Shooting in games is done in one of two ways. They either use raycasts or spawn game objects bullets from a designated firing point. Our game we decided to use the spawning method. One hurdle I had to figure out was how to spawn multiple bullets in a fixed pattern. When the player upgrades their weapon to increase their projectile count, bullets need to be spawned in a fan-like pattern. My first attempt to deal with this problem was to create new firing points for each bullet. This would prove to be problematic when the projectile count increased and the firing pattern changed. There would be way too many firing points that would need to be managed. Instead I manipulated the single firing point and rotated it to create the fan-shaped pattern. I was able to do this by creating a switch statement and assigning each case according to the number of projectiles. I would spawn bullets in each of the desired directions then use a helper script to give each bullet the correct values and force. This of course still had its downsides, the pattern was hard coded into the script and if it were to be changed, one would need to open the script and change them manually. This reduced the amount of firing points to just one and removed the need to create more than a dozen different firing points for the different patterns. In addition, if I wanted to create a new pattern with an additional projectile I would have to code that pattern manually into the script.
- Justin Y.
