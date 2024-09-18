# Space Invaders

Space Invaders is one of the earliest shooting games. The objective is to defeat waves of aliens using a laser cannon to earn as many points as possible.

## Developer

**Isaac Tapia**  
**Email:** itaps1@unm.edu

## Game Play

### Download & Run the Game

To play the game, [download the JAR file here](your-link-here).  
Once downloaded, open a terminal or command prompt and run the following command to start the game:

```bash
java -jar SpaceInvaders.jar
```
### Key Controls

- **Left Arrow** – Move the ship to the left.  
- **Right Arrow** – Move the ship to the right.  
- **Space Bar** – Fire a laser from the ship.

### Scoring

- **Hit an alien** – Earn 10 points.  
- **Ship hit by a laser** – Lose a life.  
- **Lose all lives** – Game over.

### Lasers

This game only allows one laser to be on the screen at any given time, adding a layer of strategy to timing your shots.

## Program Internals

### Classes Overview

#### `SpaceInvaders`

This is the main class where the program is initiated. The `main` method is located here to start the game.

#### `GamePanel`

This class handles most of the game logic, such as:

- Drawing game objects (ship, aliens, lasers).  
- Moving game objects across the screen.  
- Checking for collisions between objects.  
- Managing the game state (pause, over, new wave of enemies).

#### `StartPanel`

This class manages the start and pause buttons. When the game is paused, object movement is suspended.

#### `StatsPanel`

This class tracks game statistics:

- Updates the score when aliens are hit.  
- Decreases lives when the ship is hit.  
- Ends the game when lives reach zero.

## Assets

### Alien

The alien sprite was sourced from [Comp3 Interactive's Invaders from Outer Space Asset Pack](https://comp3interactive.itch.io/invaders-from-outerspace-full-project-asset-pack).

### Ship

The ship sprite was sourced from [SeekPNG](https://www.seekpng.com/ipng/u2r5q8w7y3t4y3t4_nave-space-invaders-png/).

## Known Bugs & Feature Requests

- **Game Over Condition:** The game only ends when an alien reaches the bottom-right corner of the screen, instead of anywhere along the bottom edge. This can be improved in future updates.

## Extras

No additional features were implemented beyond the core gameplay.

