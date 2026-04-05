+++ 
draft = false
date = 2026-03-30T17:02:46-05:00
title = "Room Builer (Part 1)"
description = "About the room builder project, part 1"
slug = "2026_03_30_room_builder"
authors = ["Fredric Dorothy"]
tags = ["room_builder"]
externalLink = ""
series = []
+++

It was 1AM and I was tearing my hair out over the [Goblins the Walls](https://fredric.itch.io/goblins-in-the-walls) game. I had spent hours meticulously placing wall and floor pieces for the living room scene, arranging furniture, and debugging issues with the NavMesh in Unity. All of this for just a single room in a game with only a handful of different scenes. There had to be a better way.

![Goblins in the Wall](https://fdorothy-shared-content-938377608969-us-east-1-an.s3.us-east-1.amazonaws.com/posts/2026_03_30_room_builder/goblins_in_the_wall.png)

Fast forward a year and I finally rolled up my sleeves and began working on a better solution. Introducing: Room Builder.

![Room Builder 1](https://fdorothy-shared-content-938377608969-us-east-1-an.s3.us-east-1.amazonaws.com/posts/2026_03_30_room_builder/room_builder_1.png)

Room Builder is a web tool that lets you easily model the interior space of a house (or dungeon!) with just a few clicks. Instead of placing individual 3D models, I designed this tool to programatically generate all of the geometry from the floor to the walls to doors and windows. UV coordinates are automatically calculated, and the tool comes with a set of textures and materials that you can use to paint the floors and walls.

With Room Builder I can create the kinds of scenes that took me hours to make in Goblins in the Walls with just a few clicks. But that's not the only thing this is useful for. I see this as being kind of a swiss army knife for quickly prototyping an interior space, especially relevant for game jams.

During development I realized that this tool produces very blocky geometry. I guess that's OK, houses are blocky, but I wanted to create some geometry that was more interesting. I suddenly got the idea of adding a clipping height-map with additional Perlin noise to create 'ruin' effects of buildings.

![Ruins](https://fdorothy-shared-content-938377608969-us-east-1-an.s3.us-east-1.amazonaws.com/posts/2026_03_30_room_builder/ruins.png)

I am still in the process of developing this. I'm mostly focused on programatically generating a few different roof types. I'm hoping to wrap this up sometime in the next month and release the tool and source code for free to other hungry game devs.
