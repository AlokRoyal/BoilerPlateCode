# p5.js Game Starter

A minimal starter for browser sketches using p5.js and p5.play. It creates a 600 × 600 canvas and leaves the drawing loop ready for your own scene, sprites, and interactions.

## How the starter is wired

index.html loads local p5.js libraries, the stylesheet, and sketch.js. The sketch uses setup() for one-time canvas initialization and draw() for the repeated frame loop. At present, draw() paints a black background.

## Stack

HTML5, JavaScript, p5.js, p5.dom, p5.sound, p5.play, and CSS. Libraries are bundled in lib/; the stylesheet is in CSS/.

## Run

Open index.html in a browser. Keep lib/ and CSS/ at their current paths because the page loads those files locally. If the browser blocks local assets, serve the folder with a local static server.

## Start building

Put initialization and asset loading in preload() or setup(). Add frame-by-frame drawing and updates to draw(). Use the bundled p5.play library for sprites and collisions. There is no npm package manifest or build script.