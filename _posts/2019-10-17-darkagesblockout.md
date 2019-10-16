---
layout: post
title: "Dark Ages - Week 1: Blockout"
date: 2019-10-17
---

Dark Ages, concept by [Vladimir Manyukhin](https://www.artstation.com/artwork/5yKeO)
===============

This environment is being developed for Vince Joyal's Advanced Seminar in Game Environments class.<br/>
The purpose is to recreate a picture or concept art as closely as possible, with an enthesis on modularity and tiling textures.<br/>
<img src="https://cdnb.artstation.com/p/assets/images/images/011/268/535/large/vladimir-manyukhin-dark-ages.jpg?1528716831" width="546" height="300" /><br/>
Time to get started!<br/>
<br/>

## Setting up my camera
![CameraPlacement](https://i.imgur.com/YDLKYX7.png)<br/>
For this assignment, I decided to place the camera at 0,0,0 and base the world around it.<br/>
I decided to use a CineCam in UE4 so that I could configure the Filmback settings to the exact resolution ratio of the image I'm recreating.<br/>

## Setting up my master material
<img src="https://i.imgur.com/9oMryIk.png" width="527" height="297" /><br/>
You might think this is unnecessary, but I like using a custom grid, so that I can more easily differentiate between foreground, midground and background.<br/>
The node entitled Brightness is exposed, and simply allows me to brighten/darken the base color map. I have 3 instanced materials using this brightness node.<br/>
This will help me visualize the shapes of the buildings, and break up the image into modules.<br/>

## Blocking out
I started off the blockout by bringing my image into Photoshop and drawing lines over it, dividing it into 2x2 sections.<br/>