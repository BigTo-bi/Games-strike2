# Strike 2 — 2D Platformer (Work in Progress)

A 2D pixel-art platformer type game built with **Godot Engine 4.7** and **GDScript**. This is a personal learning project that I am developing to practise player movement, physics, collisions, tile mapping, object animations, and scene organisation.

> **Status:** Work in progress. The current version contains a playable level. More gameplay features, and levels would be included as soon as it's ready.

## Current Features

- **Player features:** `CharacterBody2D` with horizontal movement, jumping, gravity, and floor detection. Player attack movement would be icluded.
- **Tile-based scenes:** every level uses would contain a `TileMapLayer` node for its background and world layout.
- **Animated coin collectibles:** coins use `AnimatedSprite2D` and `Area2D` body detection. Collection currently prints a message and removes the coin; a visible score counter would be included.
- **Moving platforms:** `AnimatableBody2D` platforms use looping `AnimationPlayer` animations (horizontal, vertical).
- **Camera following:** a `Camera2D` is attached to the player, following the player all through the scenes.
- **Death zone:** an `Area2D` starts a timer when the player enters it, then reloads the current scene.

## Controls

The player script currently uses Godot's built-in UI input actions:

| Action | Input action | Default keyboard mapping |
| --- | --- | --- |
| Move left | `ui_left` | Left Arrow |
| Move right | `ui_right` | Right Arrow |
| Jump | `ui_accept` | Space / Enter (depending on the active default mapping) |


## Requirements

- Godot Engine **4.7** .

## Run the Project

1. Download or clone this repository.
2. Open Godot Engine.
3. Choose **Import** and select the `project.godot` file in the project folder.
4. Allow Godot to import the assets.
5. Run the project using **F5** to run the project/main scene.


## Project Structure

```text
strike-2-platformer/
├── Assets/
│   └── brackeys_platformer_assets/
│       ├── fonts/
│       ├── music/
│       ├── sounds/
│       ├── sprites/
│       └── LICENSE & CREDITS.txt
├── scene/
│   ├── game.tscn
│   ├── player.tscn
│   ├── coins.tscn
│   ├── platforms.tscn
│   └── deathzone.tscn
├── script/
│   ├── player.gd
│   ├── coins.gd
│   └── deathzone.gd
├── icon.svg
├── project.godot
└── README.md
```

## Planned Improvements

The following are development goals and are **not yet implemented** in the current project version:

- Improve movement feel with configurable acceleration and deceleration.
- Add a HUD and a score counter for collected coins.
- Add enemies and player damage/interaction mechanics.
- Add a game-over/restart screen and checkpoints.
- Expand the level and include more platforming challenges.
- Add a start menu, pause function, sound effects, and background music.
- Test the game and improve overall polish.
- An actual name for the game as well.

## Assets and Credits

The project includes the **Brackeys Platformer Assets** pack.


## About

This project is being developed as part of my learning journey in 2D game development with Godot and GDScript. I plan to update this repository as I add features, refine the code, and expand the game as a whole.
