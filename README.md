# Tetris in HTML5 Canvas

A sleek, fully functional clone of the classic Tetris game built entirely with HTML, CSS, and vanilla JavaScript in a single file. This project uses the HTML5 `<canvas>` element for rendering and features a modern, responsive user interface with glassmorphism styling.

## Features

* **Classic Gameplay Mechanics:** Includes piece rotation, collision detection, line clearing, and scoring.
* **Progressive Difficulty:** The game speed automatically increases as you clear lines and level up.
* **Modern UI:** A beautiful dark theme with a semi-transparent sidebar and smooth gradients.
* **Responsive Design:** The layout automatically adjusts for smaller screens and mobile devices.
* **Pause Functionality:** Press 'P' to pause or unpause the game at any time.
* **Hard Drop:** Quickly snap pieces to the bottom using the Spacebar.

## How to Run

Because this game is entirely client-side and contained within a single file, there are no dependencies or build steps required.

1. Save the provided code as an `.html` file (e.g., `tetris.html`).
2. Double-click the file to open it in any modern web browser (Chrome, Firefox, Safari, Edge).
3. Click "Restart Game" to reset the board if you ever get a Game Over.

## Controls

* **Left Arrow (⬅️):** Move piece left
* **Right Arrow (➡️):** Move piece right
* **Down Arrow (⬇️):** Soft drop (move down faster)
* **Up Arrow (⬆️):** Rotate piece
* **Spacebar:** Hard drop (instantly drop to the bottom)
* **P:** Pause / Resume game

## Scoring System

Points are awarded based on the number of lines cleared simultaneously, multiplied by your current level:

* **1 Line:** 100 points × Level
* **2 Lines:** 300 points × Level
* **3 Lines:** 500 points × Level
* **4 Lines (Tetris):** 800 points × Level

*Note: Your level increases automatically for every 10 lines cleared.*

## Technical Details

* **Canvas Rendering:** The game board is a 10x20 grid, scaled to 30 pixels per block on a `300x600` canvas.
* **Game Loop:** Powered by `requestAnimationFrame` for smooth rendering and consistent speed calculations based on the `time` delta.
* **Matrix Operations:** Piece rotation is handled by transposing and reversing 2D arrays.
