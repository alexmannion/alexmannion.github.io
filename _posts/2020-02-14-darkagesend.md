---
layout: post
title: "The Dark Ages - What's Up?"
date: 2020-02-14
---

Dark Ages, concept by [Vladimir Manyukhin](https://www.artstation.com/artwork/5yKeO)
===============

This environment was developed for Vince Joyal's Advanced Seminar in Game Environments class.<br/>
My goal was to work off of concept art, but maintain an enthesis on modularity and tiling textures.<br/>
## My finished image
<img src="https://cdna.artstation.com/p/assets/images/images/022/621/526/large/alex-mannion-screenshot1.jpg?1576097848" width="546" height="300" /><br/>

## Why follow up 2 months after completion?
After finishing this piece in mid-December, I had a month-long break in my formal schooling. After spending over 200 hours working on The Dark Ages, 
I called the project done. That is until I was approached by EXP, an environment art publication dedicated to writing articles for growing environment artists. 
They asked me if I'd like to write an article and break down the construction of my environment, and I very excitedly said yes. They provided a list of questions to answer, 
and I started writing. I submitted the article a week or 2 later, and after having friends review it, and reviewing it myself, I felt for a first draft, it was pretty solid.<br/>
I spent my winter break very busy, both with life things and personal projects (I'll touch on this in a future post) and I quickly found myself in the second half of junior year. 
I'd heard very little in regards to the article, I'd checked up once and was assured it was being worked on, so I waited another month. I'm not sure of the future of its publication, 
but I think it addresses some things that would have helped me a lot, so I'll be posting it here, at least for the time being. <br/> <br/>
I appreciate all EXP does, and I look forward to reading their publications regardless of what happens, but I don't want the time I put into writing to be wasted.
If my statement of fact seems to promote misguided views on proper procedure, then I'd happily recieve your complaints, but regardless of what's currently the most effective and optimized means of creating environments, 
the following information portrays how I did it. I also give tips to avoid mistakes I made, and some resources that proved extremely effective, and these are simply things that I'd go back and give myself, 
were I presented with the opportunity. <br/>
Below is the unabridged article that I wrote for EXP, I hope you enjoy. <br/>

# The Dark Ages Breakdown
## With insights and advice for beginners

Tips for new 3D artists, and a breakdown of The Dark Ages. 

I’m Alex Mannion, a third-year Game Art & Animation major at Champlain College. 
I grew up in Oneonta, NY, a small town with not a lot going on. As a result, I spent a lot of time playing video games and messing around with computers growing up. 
Some of my favorite games as a kid were Roblox, Team Fortress 2, Minecraft and Chivalry: Medieval Warfare. 
In the midst of my college search, out of sheer desperation to find a major that seemed like something I could possibly do for 4 years, I decided that 3D modeling sounded cool, 
and was basically the only option for me. Although it wasn’t something I had a ton of experience in, it appeared to be a growing field with a lot of new and interesting applications. 
While the prospect of modeling architecture, and 3D printing things that I create sounded pretty great, what I was really interested in was game development. <br/>
Now a little more than 2 years after starting school at Champlain, I’ve become intimately familiar with 3D art, and recently [haha] created the piece *The Dark Ages*, 
which was based heavily on a concept entitled *Dark Ages* by Vladimir Manyukhin. <br/><br/>
My environment was created for the class Advanced Seminar in Game Environments, taught by the amazing Vince Joyal. I’ll be going in-depth on my workflow for the project; 
more specifically I’ll talk about finding modularity within medieval architecture, working from a concept, making master materials and using instancing within UE4, 
creating materials using substance designer, and entering the world of 3D art with no artistic experience.<br/>

## Composition and Modularity
### Composition

I will start by talking about how I composed this image. On the surface, it’s pretty simple. I saw a concept I thought looked awesome, could be expanded upon, and looked fun to reproduce. 
*Dark Ages* by Vladimir Manyukhin was perfect for me. As someone who is new to art in general, it felt satisfying having such a strong base to work off of, 
but also intimidating working from a concept as well received as his, with such a large reputation to live up to. <br/><br/>

For fellow beginners, I highly recommend finding one **pre-existing** piece of concept art to follow heavily. 
There’s a lot of great stuff out there, but the most beginner-friendly stuff to move into the third-dimension (in my opinion) are the images that can be broken up into sections, divided into modules, 
then pieced together to form something that would, at first glance, seem jaw-droppingly intricate and eye-catching. This not only demonstrates a strong understanding of modularity, 
but it cuts time in a major way, and will help you make more from less. <br/><br/>

As for what I added to the scene and why; I’ve included the paint-over below. Things that are highlighted are some of my favorite additions/changes I made from the original concept.<br/>
<img src="https://i.imgur.com/uDAuPeN.jpg" width="546" height="300" /><br/><br/>

**Crates and barrels!** - I made 1 type of crate, and 1 type of barrel, both using my wood material I created for the actual buildings. For more intricate props, you’d want to bring them into Substance Painter, but I was able to not only reuse 1 material and avoid Painter altogether, but I was able to reuse these 2 props all over my scene. Slightly adjusting scale and rotation of these objects was enough to keep the same exact objects from feeling overly repetitive.
<br/><br/>
**Overhang!** - Suggested by my instructor, the overhang was accomplished by taking an 8 meter tall post, moving a single edge out so that the overhanging side was angled by about 5 degrees. I assigned my stucco material, and moved the angled post beside my brick wall. I then put a cap segment (the thicker wooden plank) next to the angled post, and copied the front facing wall, rotated it, tilted it, and bam. Overhang. I also added a floor of course, which is the same mesh as the cap, just rotated 90 degrees. I also made supports for the overhang, but ended up using them all over the scene. The rock corners that are highlighted in blue were used to obscure the angled piece, but more importantly to break up silhouette, and repetivity.
<br/><br/>
**Scaffolds!** - While a massive scaffold was included in the original concept, I thought it’d be cool to put those pieces all over the place. Vince inspired me to copy the structure and move it around, which I did, but I then made some additional changes to give the individual scaffolds their own individuality (while still using the same pieces of course).
<br/><br/>
**Well!** - While the stone wall edges helped to break up the silhouette of the midground, I felt it needed something more. This was really the first big step I took outside of Manyukhin’s concept, and the one that got me to feel comfortable making changes. I slapped a noise filter on a hollowed out cylinder in 3DSMax, then applied my stone texture. The roof of the well is the same roof that’s on the building to the right of it, just scaled and with some added individual shingles to give it a more man-made feeling.
<br/><br/>
**Flags!** - At the start of the project, I used the cinematic camera in UE4 to divide the scene into a 3x3 grid. When I added the flags, I looked at the grid and felt that there was really nothing breaking up the middle ⅓ of the image. I’d learned that when in doubt, add rope/wires to break up space/lead eyes, so that’s exactly what I did. They ended up doing a really good job separating the front, middle and background. They also lead your eye from building to building, which was an added bonus! If you saw my progress screenshot, you’ll realize that for a while, the ropes didn’t have flags. That’s because I was of the impression that flags were kind of overused in medieval scenes, but when I tried them out, they just felt so right! 
<br/><br/>
**Background buildings!** - These buildings were added on a whim at around the same time I added the well, and it was made out of entirely pre-made pieces. I just stuck them together, applied different material instances (only in a few cases), and then made subtle adjustments over time. They were made more-so to demonstrate the modularity of my scene than anything else, but they ended up being a crucial part of the composition, and framed the background rather well. Another added bonus!
<br/><br/>
**Weather-vanes!** - Weather-vanes were some of the last things that I added. They’re a minor detail, but they helped breakup the skyline. 
<br/>

### Modularity

A pillar of game environments is modularity. You have to plan ahead, so that your assets can be reused in order to make big scenes with reusable pieces. 
I created *most* modular assets so that they fit within the dimensions of the planes shown below. <br/>

<img src="https://i.imgur.com/fzkVBmh.jpg" height="321" width="544.5" /><br/><br/>

This allowed me to create new buildings without having to make more assets. Not only does this save on production time, but it saves on performance. 
Instancing meshes is cheaper on performance than having to render new ones. If the mesh is already in the engine’s memory, rendering a copy of it would be quicker and less intensive on the player’s PC. 
This is an image from my Artstation post which shows a vast majority of the modular assets I used in my scene. 
In the background you can see entirely new buildings created quickly within engine, using only assets I created for my original scene. <br/><br/>

<img src="https://cdnb.artstation.com/p/assets/images/images/022/621/519/large/alex-mannion-pieces1.jpg?1576097842" width="545" height="400" /><br/>

### Procedural Materials & VFX

Thankfully, at the same time as I was taking Advanced Seminar in Game Environments, I was taking a class involving the development of procedural materials in Substance Designer, with instructor Scott Johnston. 
I’d had about 3 hours of instruction in Substance Designer before-hand, and had a really loose grasp of it, but I knew I’d love it in time.
<br/>
During our first assignment in that class, I decided that for our final environment, I’d try to texture my scene entirely in Substance Designer, and with the exception of the red banner in the background, 
I accomplished this. I made an exception for the banner because I thought it needed some sort of symbol, which would have been a waste of time to make in designer, and Substance Painter had some good grunge generators. 
I just used a red base color, a leaf brush, and some dirt generators/masks.
<br/><br/>
I ended up using a total of 7 materials, all with some variants for vertex painting. These materials were; Mud/Grass (same graph), Stucco, Slate Roofing, Brick/Stone (same graph), Metal, Glass, and Wood. 
These materials were all set up as master materials, vertex painting was also kept in mind, and used pretty frequently. I used instancing on objects that were further in the background, 
or ones that just didn’t require vertex painting. A specific example of instancing was reusing my main wood material for the shutters. I used the Flatten Normal node to lower the normal intensity, 
and attached an overlay_blend node, with a ConstantVector4 exposed to the base color, coupled with an add node. It was pretty fun just being able to change so much about the material in-engine, and it was also a major time saver. 
<br/><br/>
A crucial part of my scene is the smoke VFX, which was an element suggested by my instructor Vince Joyal. Having less than 2 weeks remaining until submission at the time of the suggestion, 
I didn’t have time to learn how to create new VFX inside of UE4’s editor without guidance. So, I instead used the smoke VFX in UE4’s Starter Content as a base, 
and configured all of the emitter properties to create something more unique and interesting for my scene. This process took me an hour or 2, and involved loads of trial and error until I got the smoke looking decent. 
The most important things I needed to adjust were the Constant Acceleration and the Initial Velocity. This allowed me to get the smoke blowing really aggressively. <br/><br/>
<img src="https://i.imgur.com/1dXh6UE.jpg" height="440" width ="400" /><br/>

## Step By Step

The making of this scene took about 8 weeks, and around 200ish hours. Keep in mind, I was learning 3DS Max and Substance Designer throughout the project. 
I’ll briefly describe some of the larger strides I took throughout this project. <br/>

### Week 1: Blockout

Seeing as no one in my class had blocked out a UE4 scene before, and we started the assignment over a break, we were all really confused. 
I’m not sure if it was genuine confusion, or if we were really just intimidated by the scope of the project, but either way we didn’t want to start off on the wrong foot. 
I’m the type of person to do some research, but when I can’t find what I’m looking for, I just say *screw it, we’ll just try stuff and hope it works.*  <br/>
<img src="https://i.imgur.com/w0ZJuC4.jpg" width="546" height="300" /><br/><br/>

I made some really basic assets. I created panels that follow my modularity scale, which means that I had 1x1, 2x2, 4x4 planes and triangles at the start. 
I broke my reference image into a 3x3 grid, and then used a cinematic camera positioned at the same angle as my reference, so that I could compare the two as I work on my blockout. 
As you can see above, I started out with really simple shapes, and didn’t try to define any of the more complex shapes. This was so that I could replace my simple meshes with the new, more detailed ones I create. 
<br/><br/>
**Important** In order to avoid wonky perspective within my scene, I made some minor adjustments to the concept to keep my buildings together, and not floating off in the distance. 
I highly recommend this, as it gave my scene more individuality, helped me break free of the concept, and now I can walk around my scene free of wonky perspective.
<br/>
<iframe width="560" height="315" src="https://www.youtube.com/embed/zOakXEqiD5Y" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
<br/>

### Week 4: “Finishing” Modeling

The task I was given for the end of week 4 was to finish modeling, but accept that I might want to remodel/model more minor props later down the line. 
While I did eventually go back and model some more smaller modular props, and I remade the stone wall on the bottom left of the image, at the time, I had achieved my goal.<br/>

<img src="https://i.imgur.com/iEXrbQk.png" height="300" width ="546" /><br/><br/>

The largest change going forward was how the mood is achieved. In the original concept everything was gloomy and dark, and I wasn’t sure how to replicate that feeling in the same way within UE4. 
Many areas were obscured in shadow, and while there was suggestion, the viewer was still left to wonder what’s going on in the shadows. I decided to take the liberty to expose it, 
and make the scene feel lived in, even without characters.
<br/><br/>
As you can likely tell, in week 4 I had a post-processing volume, fog and not much in the way of lighting. I’d overcompensated, and this was the point when I realized I pushed the dark, 
blue and moody thing too far, and needed to completely reassess. I wanted to get the general vibe of the main concept, but in a different way, so I decided to take out the rain from the original concept, 
and imagine the scene after the rain. This gave me freedom to light the areas in the foreground, use creative freedom to fill them, and it gave me the willingness to experiment more. 
At this point I’d already deviated a fair bit from the concept, but there was more to come. 
<br/><br/>
I decided the foreground needed some more interesting elements, so I added some crates and planks just lying around. I’d already made barrels, so I just spread them around some more. 
In the coming weeks, the scene was finally starting to get broken in.<br/>

### Week 6: “Finishing” Texturing

By the end of week 6 I was supposed to have all of my textures created and assigned. While of course improvements were bound to happen, I decided I should have material IDs and materials sorted at this point. 
At this point I had all of my materials created except for my metal. Everything had UVs, lightmaps and material IDs, with the exception of the castle.<br/>
<img src="https://i.imgur.com/btWf6w2.jpg" height="300" width ="546" /><br/><br/>

I still hadn’t completely figured out lighting, although I had begun placing spotlights and point-lights around to light the scene with more control. Previously I’d only had a single directional light, 
so the addition of the row of spotlights down the main path, and point-lights from inside the houses are showing off a lot more detail than before, but it’s still not enough. 
In the coming weeks I got rid of the emissive window material (as seen on the right), and replaced it with small, not very detailed interiors that could be lit and display more light and detail than the emissive could.
<br/><br/>
By the end of the week, I’d leaned away from the blue lighting, and wanted everything to be desaturated, but still feel alive. 
I decided I needed some foliage to break up all of the yellow, blues and browns, but I also sensed that the lighting was still missing something. So that’s when I decided to up the gamma and exposure, and play around with fog.
<br/>

### Week 8: Wrapping it up

So in the final weeks, I really didn’t do that much that stuck. It was a lot of trial and error, looking at references, and revisiting old meshes and materials. 
A lot of this was due to the realization of things I mentioned prior, about capturing a dreary, gloomy feeling from an environment that still feels alive and lived in. 
It took a while to realize what feeling I was searching for from this image, but once I found it, everything else clicked.
<br/><br/>
<img src="https://cdna.artstation.com/p/assets/images/images/022/621/526/large/alex-mannion-screenshot1.jpg?1576097848" width="546" height="300" /><br/><br/>

I did 3 things of note in the final week that I believe are worth talking about in-depth. <br/>
**The first**, is adding fake volumetric fog planes. [Click here](https://forums.unrealengine.com/community/community-content-tools-and-tutorials/108372-fake-fog-volume-tutorial) for a link to the guide I followed to create this effect. 
I used the guide as a base, but went a step further and used masks so that I could blend fog more seamlessly. The graph for creating my masked version is below. 
The texture sample you see could be exposed to use different masks with instances, but I only relied on a very simple bell-shaped mask I exported as an alpha from Substance Designer. 
This helped me get a really nice depth fog effect that I wouldn’t have been able to achieve otherwise. I was also able to share this with some of my other classmates which was definitely an added bonus. <br/><br/>
<img src="https://i.imgur.com/rRb02Rm.jpg" width="500" height="330"> 
<br/><br/>
**The second**, is making decal generators. I used Substance Designer to create procedural puddles, cracks and grime, which helped me greatly in breaking up the repetition of using the same decals over and over again. 
I saved out 2 to 3 variations of each of these, and used them all over the place. Shown below is my puddle graph.
<br/>
<img src="https://i.imgur.com/jY9tgAg.jpg" width="500" height="164">
<br/>
All I had to do was adjust the random seed and it changed the disorder of the 2 noises I used, creating unique puddle variants. I also altered the starting shape for increased variation at times. 
I put these puddles all over, and paired with reflection captures, they helped tremendously with bringing new light and color into areas that were previously uninteresting.
<br/><br/>
**The third**, was adding foliage. I downloaded a free image of grass from [textures.com](https://www.textures.com), warped some planes with the UVs mapped over the texture, used the master material I made for my hay texture, 
and placed the prefab all over the scene. I was able to scale it, rotate it, and with the addition of a SimpleGrassWind node, sway it. <br/> 

## Conclusion

My final piece of advice might seem basic, but it’s important to address. When publishing art, or putting it in your portfolio, make 100% certain that it looks good to you. 
While I’ll look back at *The Dark Ages* for ages, always being able to find flaws in it, I posted it without any major aches and pains. 
If the piece doesn’t feel right to you, ask for critique, gain new perspective, try it out and see what sticks. The more you practice and the more perspectives you take into account, 
the more your artist mind will develop and grow with inspiration, creativity and self-assurance. It’s because of the people I sought out for help along the way, and the leaps of faith I took, 
that I was able to make something I’m satisfied to call finished (at least for now).
<br/><br/>
Thanks to all the people who helped me along the way, and contributed to my getting to this point, and a big thanks to Experience Points for giving me the honor of writing an article for them!<br/>
<br/>
Even if it may not get published, it was still a great learning experience. <br/><br/>

# What's next?

I'll be back to doing some more blog posts soon, regarding my current 3D environment project, what I worked on over winter break, and the game I'm working on for Production 2.


<br/> 

