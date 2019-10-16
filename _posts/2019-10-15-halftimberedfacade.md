---
layout: post
title: "Half Timbered Facade - Break-Down"
date: 2019-10-16
---

Modular Half-Timbered-House Break-down
===============

After 5 weeks I completed the first assignment of Vince Joyal's Advanced Seminar environment art class<br/>
The goal of the assignment was to recreate a picture with as much modularity as possible. Everything in the left picture is homemade. <br/>
![colombage1](https://i.imgur.com/t4lATKD.png)
![colombageRef](https://i.imgur.com/68jCq9E.jpg)<br/>

A large part of modularity is tiling textures, and maintaining a consistent texel-density, both of which I knew very little about at the start<br/>
of the assignment, especially within 3DS Max which was a brand new, and an incredibly daunting program.<br/>
As you can imagine, missteps were bound to happen. Because of this, I will post my process, as well as ways I'll improve my workflow going forwards. <br/>
<br/>

# Breaking down the picture modularly <br/>
My method of breaking down the image into modular chunks meant I'd focus 95% of my time working on 3 tiles. I spent 100% of my time working on them for the first 3 weeks.<br/>
*The door section, the ground-level window section and the top window section that tiles infinitely upwards.*<br/>
I attribute this working out to sheer luck. If this were a larger project, *(i.e. what Vince has me working on now)* it would have been a major set-back.<br/>
Still, noticing I still had 3 tiles left to make at week 3 scarred me. This will be the last time I make modules without planning ahead.<br/>
**Moral of the story:** Break down all modular pieces into segments before you start modeling. By all, I mean every last piece. <br/>
![colombageModularityBreakdown](https://i.imgur.com/8CSyv1M.jpg)<br/>
*This can even be done with Microsoft Paint*<br/>
)<br/>

# Choosing a modularity pyramid <br/>
During our second class, Vince Joyal introduced us to the modularity pyramids, which fundamentally dictate the scale translation from our images to UE4.<br/>
There are 2 types of pyramid, **base-1**, or **base-2**. The base-1 pyramid means that tiles must be created at a size of 1x1 meter, 2x2 meters, or 4x4 meters. <br/>
The base-2 pyramid (the one that I followed) means that tiles must be either 2x2 meters, 4x4 meters or 8x8 meters.<br/>
I chose base-1 because I knew my main 3 modules fit best within a 2x2 space, which was determined by the size of the door.<br/>
The current standard for door height is 6', 8", or roughly 2 meters, but these buildings pre-date modern standards, so I figured 2x2m would be a perfect fit.<br/>
This gave me the freedom to use half-walls for both 1x2 or 2x4 and stay within a usable ratio. <br/>
Although I ended up with some scale issues around the door in correlation to the ref. image, that was an overseight rather than technical issue.<br/>
**Take-away:** Base your scale around things in your scene that have a standardized real-world scale, such as doors, table height, steps, etc. <br/>
Remember not to alter the scale of the object you based your project scale around. This was easily my most costly mistake.<br/> 
<br/>

# Using multiple elements to make 1 object <br/>
This is as simple as it sounds, there's no major negative to using multiple elements within a single mesh, so long as hidden faces are deleted. <br/>
Knowing this at the start would greatly have improved my workflow, as each of the windows and support beams were modeled off of cubes and welded into place.<br/>
If I hadn't welded them and left them separated, I could have UV'd one, then duplicated it and offset the UV on my material.<br/>
This would have saved hours in the UVing process, and relieved a lot of frustration.<br/>
<br/>

# Using master materials and instancing within UE4 <br/>
Master materials are essentially just standard materials (with maps like roughness, normal, AO, etc.) only more efficient on performance and design.<br/>
Master materials use packed maps and exposed variables to make changing material info in real-time quick and painless. <br/>
I was able to reuse one master material for 3 of the 4 materials in my scene.<br/>
*Thanks to [Leanna Russell](https://www.artstation.com/leannarussell) for helping me set that up.* <br/>
<br/>

# Making curtains using 3DS Max and UE4 within 5 minutes <br/>
I made my glass sub-material translucent, as to allow for more interesting interiors which break up the monotonous modularity in the image.<br/>
My greatest discovery during this process was when I made a curtain using the WorldPosOffset material input.<br/>
I took a 2x2 subdivided plane in Max, UVW plannar mapped it, imported it into UE4, and applied a material with SimpleGrassWind plugged into WorldPosOffset. <br/>
The material itself was made in Photoshop by taking a gradient, leveling it, rotating it 180 degrees and multiplying the layer. <br/>
**Take-away:** UE4 has hundreds of blueprint nodes for a reason. Sometimes getting creative with them could save tremendous amounts of time.<br/>
<br/>

# Conclusion <br/>
This project was a major learning experience for me, and now that I have the software and workflow experience,<br/>
I'll be able to tackle some significantly larger scale projects in the future with much more confidence. <br/>
Big thanks to everyone who provided critique and helped me get to this level of comfort.<br/>
Check back within the coming weeks for updates on my next big assignment!<br/>
  


