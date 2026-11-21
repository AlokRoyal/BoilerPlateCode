# p5.js Game Starter

![JavaScript](https://img.shields.io/badge/JavaScript-p5.js-FB7D24?logo=p5dotjs&logoColor=white)
![Status](https://img.shields.io/badge/project-starter%20template-lightgrey)

A minimal browser sketch scaffold using p5.js and p5.play. It initializes a 600 × 600 canvas and provides an empty frame loop for building a game or interactive sketch.

## What it demonstrates

- The p5.js lifecycle: preload, setup, and draw
- Loading browser libraries from local script files
- A simple project structure for canvas sketches

## Current behavior

index.html loads p5.js, p5.dom, p5.sound, and p5.play from lib/, loads CSS/style.css, and then runs sketch.js. setup() creates the canvas; draw() currently paints a black background. No game mechanics or controls have been implemented yet.

## Architecture

Browser → index.html → local p5 libraries + sketch.js → canvas

## Start locally

Open index.html in a modern browser. Keep lib/ and CSS/ at their existing paths. If local script loading is blocked by the browser, serve the directory with a local static web server.

## Project layout

- index.html — script and stylesheet entry point
- sketch.js — p5.js sketch lifecycle
- CSS/style.css — page styling
- lib/ — bundled p5.js and p5.play browser libraries

## Extend the sketch

Add asset loading to preload(), one-time initialization to setup(), and per-frame drawing or updates to draw(). Use the bundled p5.play library if you add sprites and collisions.

## Limitations

The repository has no package.json, build tool, automated tests, or application-specific dependencies. Libraries are loaded from the checked-in lib/ directory.