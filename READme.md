# Daven - The Hedgehog

## Overview
Hopeful Hedgehog is a 2D side-scrolling arcade game developed in Godot Engine 4. Inspired by classic vertical-navigation mechanics and high-speed action platformers, players guide a hedgehog through an alpine wilderness. The objective is to navigate between suspended icicles and snow-covered pine trees while collecting berries and utilizing a high-speed spin dash ability. Reaching the target berry count concludes the game with an encouraging message focused on resilience, mental well-being, and optimism.

## Genre and Classification
* Primary Genre: 2D Arcade Action
* Sub-Genre: Side-Scrolling Flyer and Runner
* Theme: Wholesome and Inspirational

## Key Features
* Dynamic Character States: The protagonist transitions between a standard posture and a curled, brown-spined ball when jumping or dashing.
* Shooting Star Superpower: Traveling a set horizontal distance charges a power meter. At maximum capacity, the hedgehog transforms into an invincible, high-speed projectile capable of destroying obstacles upon contact, accompanied by a particle trail and speed afterimages.
* Three-Life Respawn System: Players begin with three hearts displayed on the heads-up display. Colliding with an obstacle deducts one heart and triggers a brief invincibility window upon respawn.
* Dual Ending Conditions: Depleting all three lives displays a supportive summary screen, while collecting 50 berries triggers the primary victory screen containing a motivational life lesson.
* Custom Audio and Visuals: Includes transparent 2D sprites, a seamlessly scrolling alpine background, snowfall particle effects, and synthesized retro sound effects.

## Controls
* Spacebar or Left Mouse Click: Jump upward and curl into a rolling ball.

## Project Structure
* `project.godot`: Main configuration file containing display settings and input mappings.
* `Main.tscn` and `Main.gd`: Primary game scene managing the scrolling background, obstacle and berry spawners, user interface, life tracking, and ending states.
* `Player.tscn` and `Player.gd`: Character physics implementation, jump mechanics, sprite state switching, and superpower dash logic.
* `Obstacle.tscn` and `Obstacle.gd`: Hazard logic pairing top icicles and bottom pine trees, including collision detection and destruction behavior during superpower states.
* `Berry.tscn` and `Berry.gd`: Collectible item logic with vertical sine-wave oscillation and score incrementation.
* Audio Assets: `jump.wav`, `berry.wav`, `dash.wav`, and `hit.wav`.
* Visual Assets: `hedgehog.png`, `hedgehog_ball.png`, `tree.png`, `icicle.png`, `berry.png`, `heart.png`, `star.png`, and `background.png`.

## Installation and Setup
1. Download and extract the project archive to a local directory on your computer.
2. Download and launch Godot Engine 4.2 or a newer version.
3. In the Godot Project Manager window, select the Import button.
4. Browse to the extracted project directory, select the `project.godot` file, and click Import and Edit.
5. Once the editor loads, press F5 or click the Play button in the top-right corner of the interface to run the game.

## Configuration and Customization
Game balance parameters can be modified directly within the script files:
* Target Berry Goal: Open `Main.gd` and modify the `TARGET_BERRIES` constant on line 7 (default is set to 50).
* Superpower Charge Distance: Open `Main.gd` and adjust the `DISTANCE_FOR_SUPERPOWER` constant on line 8 (default is set to 1200.0).
* Gravity and Jump Physics: Open `Player.gd` and adjust the `GRAVITY` and `JUMP_FORCE` constants on lines 3 and 4 to alter movement responsiveness.

## Licensing and Credits
* Game Engine: Developed using Godot Engine, licensed under the MIT License.
* Visual and Audio Assets: All included background artwork, sprites, and synthesized audio files are original or licensed under Creative Commons Zero (CC0) public domain terms for unrestricted use.
