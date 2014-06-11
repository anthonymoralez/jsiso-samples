HTML5 Canvas Tile Engine -- Samples
=========

![JSiso](http://jsiso.com/jsiso.png)


This repo contains an MIT Licensed samples of how to use the Isometric HTML5 tile engine 
Copyright © 2013 of Iain Hamilton and Edward Smyth.

The most current running dev build can be viewed here: http://better-beakable-isometric.herokuapp.com

For a list of examples and further details checkout: http://jsiso.com

Currently contained features are:
  - AMD structured using requireJS 
  - Easily create 2D or 2D.5 layouts
  - Unlimited layer stacking
  - Heightmaps
  - Auto scaling of image dimensions
  - Zooming (not 100% perfect yet)
  - Rotating (not 100% perfect yet - Rotates whole map but doesn't readjust view)
  - Simple Collision
  - AI Pathfinding using Web Workers
  - Custom built Particle Engine
  - Easy fake lighting
  - Player vision limiting
  - Simple player device interaction
  - Easy Node Multiplayer Integration

Setup Instructions:
-------------
0. Install yeoman `npm install -g yo`
1. `npm install`
2. `bower install`
3. `npm start`

Notes:
1. In each of the samples you'll see something like: ```<script data-main="../js/deps/jsiso.js" src="../js/deps/requirejs/require.js"></script>```. These two paths will need to be correct in order for JsIso to work.

2. Throughout the samples it makes use of an express.js app to read a image directory and output a XML list of image files``` XML.loadXML('../XMLFiles?folder=/ground/');```. This path will also need to be correct or you will need to pass an array of image paths manually through to the image loader ```imgLoader.loadImageArray(XML.getContent('files','file'), true);```. Note: The app adds /img/ itself for security, enforcing only reading of the img directory.

3. That should be everything.


Particles
![particles](https://f.cloud.github.com/assets/1159739/1322878/ca65cd72-3453-11e3-97f6-c6b0243787b0.png)


Pathfinding (All cuboids apart from blue are AI)
Pathfinding calculations are handled via webworkers.
![ai](https://f.cloud.github.com/assets/1159739/1286661/31621fbc-2fdb-11e3-9e7a-39436670d4ba.png)


Fog of view and lighting toggled on (blue cuboid represents player)
![lighting](https://f.cloud.github.com/assets/1159739/1278363/757498b4-2f0f-11e3-97af-5e5042679270.png)


Basic dynamic lighting
![with-lighting](https://f.cloud.github.com/assets/1159739/1277738/28d797b8-2edd-11e3-95f8-4e6177eb81bd.png)

Lighting toggled off
![no-lighting](https://f.cloud.github.com/assets/1159739/1277736/0fb64586-2edd-11e3-8a73-43645830401c.png)



Height Maps, Rotation, Auto Shadows, Zoom
![new-screen](https://f.cloud.github.com/assets/1159739/1273886/fd76d006-2d5c-11e3-8dde-f9d83eba639b.png)


Previous tile map zoomed out
![new-screen2](https://f.cloud.github.com/assets/1159739/1273894/d760ad64-2d5d-11e3-9bf2-77319cce1fc6.png)



Early Screenshot 1
![screen1](https://f.cloud.github.com/assets/1159739/1267397/a8c33f7a-2cb9-11e3-8d82-2b5ec4c5f2aa.png)

Early Screenshot 2 
![screen2](https://f.cloud.github.com/assets/1159739/1267395/94e0ea16-2cb9-11e3-9726-86f312bca9f9.png)




