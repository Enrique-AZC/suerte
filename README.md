# Interactive 3D Candle Visualization

## Abstract
This project implements an **interactive 3D candle** rendered in the browser using the **Three.js API** (a high-level WebGL framework).  
The candle is accompanied by a flame animation that flickers dynamically. When the flame is clicked (or tapped), a hidden **“easter egg” interaction** is revealed: a random affectionate phrase appears on screen, together with a “Good Luck Activated” message.

The project explores the use of **computer graphics for artistic expression**, blending simple geometry with interaction design to deliver a playful and emotional user experience.

## Objectives
1. To create a **3D candle visualization** with real-time flame animation using Three.js.
2. To implement **interactive raycasting** for detecting user input on the flame geometry.
3. To integrate **narrative overlays** that enhance the personal and artistic character of the visualization.
4. To experiment with the combination of **minimalist 3D graphics** and **user-driven storytelling**.

## Features
- **3D Candle geometry**:
  - Cylinder-shaped candle with pure white material.
  - Cone-shaped flame in yellow/orange tones.
- **Flame animation**:
  - Subtle scale and position oscillations simulate natural flickering.
- **Interactive easter egg**:
  - Clicking or tapping the flame reveals a random phrase (e.g., *“Estrellita”*, *“Ángel”*).
  - A message appears at the bottom of the screen: *“Buena suerte activada”*.
- **Responsive design**:
  - Works on both desktop and mobile devices.
  - Resizes dynamically with the browser window.

## Implementation Details
- **HTML/CSS**:
  - Minimalist layout with a black background to emphasize the candle.
  - Overlays for displaying messages and easter egg phrases.
- **JavaScript**:
  - Handles random phrase selection and DOM manipulation.
  - Manages user input events (clicks and touch).
  - Animates the flame with sine-based transformations.
- **Three.js API**:
  - Provides the rendering pipeline (scene, camera, renderer).
  - Supports geometric primitives (`CylinderGeometry`, `ConeGeometry`) and materials.
  - Uses **Raycaster** API to detect intersections with the flame object.

## Requirements
- A modern web browser supporting WebGL.
- Three.js loaded from CDN:
  ```html
  <script src="https://cdn.jsdelivr.net/npm/three@0.161.0/build/three.min.js"></script>
