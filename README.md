# 2048 Game

## Introduction

Welcome to the 2048 Game project, a browser-based implementation of the classic 2048 puzzle game built with JavaScript.

The goal of the game is to combine tiles with equal values on a 4 × 4 board until the player creates a tile with the value 2048. The project focuses on implementing game logic, keyboard controls, score calculation, game-state management, and DOM updates.

This project demonstrates practical knowledge of object-oriented programming, JavaScript classes, array manipulation, event handling, and interaction with the browser DOM.

## Key Features

- Classic 4 × 4 Board: The game uses the standard 2048 grid layout.
- Keyboard Controls: Players can move tiles using the arrow keys.
- Tile Merging: Tiles with equal values merge into a single tile with a doubled value.
- Random Tile Generation: A new tile with the value 2 or 4 appears after each valid move.
- Score Tracking: The score increases based on the values of merged tiles.
- Win Condition: A victory message appears when the player creates the 2048 tile.
- Game-Over Detection: The game detects when no valid moves remain.
- Start and Restart Controls: Players can start a new game and reset the board at any time.
- Responsive Interface: The layout adapts to different screen sizes.
- Game-State Management: The current board, score, and status are managed through a dedicated Game class.

## Challenges

Developing the 2048 game involved several important technical challenges, especially in implementing the movement and merging rules correctly.

### Key Challenges

- Tile Movement Logic: Moving all tiles in the selected direction required careful handling of empty cells and array transformations.

- Correct Tile Merging: Equal tiles must merge only once during a single move. Preventing a newly merged tile from merging again required precise control of the algorithm.

- Directional Movement: The same game rules had to work consistently for left, right, up, and down movements. This required adapting rows and columns without duplicating unnecessary logic.

- Valid Move Detection: A new tile should appear only when the board actually changes. Detecting whether a move was valid was an important part of the implementation.

- Score Calculation: The score needed to increase by the sum of all newly created merged tiles.

- Win and Lose Conditions: The game had to detect both the creation of the 2048 tile and situations where no moves remained.

- DOM Synchronization: The visual board, score, button state, and game messages needed to stay synchronized with the internal game state.

Solving these challenges improved my understanding of JavaScript classes, algorithms, immutable data handling, event-driven programming, and browser-based user interfaces.

## Technical Requirements

To run this project locally, you need:

- A modern web browser
- Node.js
- NPM

## Installation and Setup

Follow these steps to install and run the project locally.

### 1. Clone the repository

```bash
git clone https://github.com/aholubko/2048-game.git
``` 

### 2. Navigate to the project directory

```bash
cd 2048-game 
```

### 3. Install dependencies

```bash
npm install 
```

### 4. Start the local development server

```bash
npm start 
```

After starting the project, open the local address displayed in the terminal.

## Usage

1. Click the Start button.
2. Use the keyboard arrow keys to move the tiles:
   - Arrow Up
   - Arrow Down
   - Arrow Left
   - Arrow Right
3. Combine tiles with equal values.
4. Continue playing until you create the 2048 tile.
5. Use the Restart button to reset the game.

## Live Preview

[Play the game](https://aholubko.github.io/2048-game/)

## Technologies Used

This project was built using the following technologies:

- HTML5: Used to structure the game interface.
- SCSS: Used to style the board, tiles, controls, and responsive layout.
- JavaScript (ES6): Used to implement the game logic and user interaction.
- Object-Oriented Programming: Used to organize the game logic in the Game class.
- DOM API: Used to update the board, score, messages, and controls.
- Keyboard Events: Used to process player movement through arrow keys.
- Node.js: Used as the project runtime environment.
- NPM: Used to install and manage dependencies.
- Git: Used for version control.
- GitHub: Used to host and manage the repository.
- GitHub Pages: Used to deploy the live game.

## Design Specifications

### Game Board

- Grid size: 4 × 4
- Supported tile values: 2, 4, 8, 16, and higher powers of two
- Winning tile: 2048

### Responsive Sizes

- Desktop: 1024px and wider
- Tablet: 576px and wider
- Mobile: 320px and wider

## Available Scripts

Run the project locally:

```bash
npm start
```

Run the tests:

```bash
npm test 
```

Deploy the project to GitHub Pages:

```bash
npm run deploy
```
