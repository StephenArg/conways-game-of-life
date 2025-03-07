# Conway's Game of Life

This project implements **Conway's Game of Life**, a cellular automaton devised by mathematician John Conway. It simulates a grid of cells that evolve based on a set of simple rules, leading to complex and often unexpected patterns.

## Demo

The game runs in your browser using an HTML5 `<canvas>` element for visualization.

## How It Works

The game consists of:

- A grid of cells, each of which can be **alive** or **dead**.
- At each step (generation), cells evolve based on the following rules:
  1. A live cell with **fewer than 2** live neighbors dies (underpopulation).
  2. A live cell with **2 or 3** live neighbors survives.
  3. A live cell with **more than 3** live neighbors dies (overpopulation).
  4. A dead cell with **exactly 3** live neighbors becomes alive (reproduction).

## Project Structure

### `bitset.js`

This script provides a **bitwise representation** of the game grid to improve performance. Instead of storing each cell as a boolean, it packs multiple cells into a single integer, making operations faster.

### `index.js`

This is the core logic of the game, handling:

- **Grid updates** based on the Game of Life rules.
- **Canvas rendering** to display the evolving cells.
- **User interactions** (e.g., starting, pausing, or resetting the simulation).

## How to Run

1. Download all files into the same directory
2. Open `index.html` in a web browser.
3. The game starts automatically.
4. Modify `index.js` to adjust settings like grid size and speed.

## License

This project is open-source and available under the MIT License.
