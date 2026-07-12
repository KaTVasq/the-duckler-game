# The Duckler

Fast-paced top-down action RPG developed with **Phaser 3**, **JavaScript**, **Vite** and **Electron**.

The game follows an angry duck who becomes the last survivor of its park after an invasion of predators. The player explores different areas, defeats enemies, collects weapons and consumables, improves character statistics and progresses towards the final boss.

## Project overview

The Duckler is a pixel-art hack-and-slash game built as a university team project.

The main gameplay loop combines:

- Exploration
- Real-time combat
- Weapon collection
- Character progression
- Item management
- Enemy encounters
- Boss fights
- Checkpoints and upgrades

The game can be played with keyboard and mouse or with an Xbox controller.

## Main features

- Top-down movement and combat
- Multiple weapons with different behaviours
- Weapon durability and replacement system
- Enemy AI and combat states
- Consumable items
- Shop and in-game currency
- Character upgrades
- Checkpoints based on puddles
- Dash with temporary invulnerability
- Player death and respawn system
- Multiple scenes and areas
- Final boss encounter
- Sound effects and background music
- Keyboard, mouse and Xbox controller support
- Desktop builds with Electron

## Technologies

- JavaScript
- Phaser 3
- Vite
- Electron
- HTML
- CSS
- Node.js
- GitHub Actions

## Gameplay

The objective is to progress through the different zones of the park and defeat the final boss.

During the game, the player can:

- Move using `WASD` or the arrow keys
- Attack with the equipped weapon
- Dash to avoid damage
- Pick up and exchange weapons
- Use consumable items
- Collect feathers
- Spend feathers on upgrades
- Collect bread currency
- Purchase items from the shop
- Activate enemies with the duck's quack ability

## Controls

### Keyboard and mouse

| Action | Control |
|---|---|
| Move | `WASD` or arrow keys |
| Attack | Left mouse button |
| Dash | Space |
| Quack | `C` |
| Interact / pick up | `E` |
| Previous item | `Q` |
| Next item | `R` |
| Quick item selection | `1–6` |

### Xbox controller

| Action | Control |
|---|---|
| Move | Left stick |
| Aim | Right stick |
| Attack | Right trigger or bumper |
| Dash | Left trigger or bumper |
| Quack | `B` |
| Interact | `A` |
| Use selected item | `X` |
| Navigate items | D-pad |

More detailed information is available in [`CONTROLES.md`](CONTROLES.md).

## Architecture

The project is organised around Phaser scenes, reusable game objects and input-management components.

```text
.
├── assets/
├── css/
├── documentacion/
│   ├── gdd_The_Duckler.pdf
│   ├── Informe_datos_playtest.pdf
│   └── informe_contribucion_The_Duckler.md
├── src/
│   ├── GameObjects/
│   │   ├── Consumables/
│   │   ├── Enemies/
│   │   ├── Projectiles/
│   │   ├── Puddles/
│   │   └── Weapons/
│   ├── managers/
│   ├── scenes/
│   └── game.js
├── CONTROLES.md
├── package.json
├── vite.config.js
├── electron.vite.config.js
├── electron-builder.yml
└── README.md
```

## Main components

- `duck.js`: player character behaviour
- `enemy.js`: common enemy logic
- `weapon.js`: shared weapon behaviour
- `store.js`: shop logic
- `InputManager.js`: keyboard and controller input
- `MenuScene.js`: main menu
- `MainScene.js`: main gameplay scene
- `AlcantarillasScene.js`: additional game area
- `SettingsScene.js`: settings interface
- `FinishScene.js`: final scene

## Installation

### Requirements

- Node.js
- npm

Clone the repository:

```bash
git clone https://github.com/KaTVasq/the-duckler-game.git
cd the-duckler-game
```

Install dependencies:

```bash
npm install
```

## Run in development mode

```bash
npm start
```

## Build the web version

```bash
npm run build
```

## Build the desktop version

Windows:

```bash
npm run build:win
```

macOS:

```bash
npm run build:mac
```

Linux:

```bash
npm run build:linux
```

## Documentation

The repository includes:

- Game Design Document
- Playtesting report
- Team contribution report
- Detailed controls
- Game assets
- Source code
- Desktop build configuration

## My contribution

My role in the project focused on **UI design, audio and gameplay programming**.

My main contributions included:

- Implementing sound effects and background music
- Designing and improving the game interface
- Developing the main menu
- Developing the settings menu
- Developing the death screen
- Developing the final screen
- Creating pop-up menus and the game guide
- Implementing the top HUD
- Creating the shop interface
- Improving the consumable-item system
- Developing and refining several game scenes
- Implementing player death logic
- Improving enemy behaviour and combat
- Contributing to the final boss
- Improving player progression and general gameplay balance

## What I learned

This project helped me strengthen my skills in:

- Game development with Phaser
- Scene management
- UI and HUD design
- Audio integration
- Input handling
- Gamepad support
- Object-oriented JavaScript
- Event-driven programming
- Gameplay balancing
- Collaborative development with Git
- Packaging applications with Electron
- Playtesting and iterative improvement

## Academic context

University team project developed for a video game design and development course.

The complete game was created collaboratively. My individual contribution focused on interface design, audio, gameplay systems, scene development and player progression.

## License

This project is distributed under the MIT License included in the repository.

## Author

**Katty Vasquez Peinado**

- [LinkedIn](https://linkedin.com/in/katty-vasquez)
- [GitHub](https://github.com/KaTVasq)
