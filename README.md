# Cosmic Parkour

Cosmic Parkour is a fast-paced JavaScript parkour game built with Three.js. Move through a neon sci-fi world, chain jumps, wall-runs, and sprints, and collect score-boosting coins while avoiding obstacles.

## Features

- First-person parkour movement (run, sprint, jump, wall-run)
- Procedurally generated cosmic platform world
- Score, coin, platform, timer, and stamina HUD
- Pause/resume and restart flow
- Optional wallet connection via MetaMask
- In-game map designer mode for creating custom layouts

## Technologies Used

- JavaScript (ES Modules)
- Three.js
- HTML5 + CSS3
- Ethers.js (wallet/blockchain integration)
- Node.js + `http-server` (local development server)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/cssaditya/cosmic-parkour.git
   cd cosmic-parkour
   ```
2. Install dependencies:
   ```bash
   npm install
   ```

## How to Run the Project

Start the local server:

```bash
npm start
```

Then open the URL printed by `http-server` (typically `http://127.0.0.1:8080`).

## Project Structure

```text
cosmic-parkour/
├── index.html              # Main game page and UI containers
├── main.js                 # Game bootstrap and loop
├── player.js               # Player movement, controls, physics
├── world.js                # Platform generation, collectibles, obstacles
├── ui.js                   # Start/pause/end screens and HUD updates
├── effects.js              # Post-processing visual effects
├── mapDesigner.js          # In-game map editing logic
├── mapDesignerUI.js        # Map designer panel and controls
├── sound.js                # Game audio manager
├── style.css               # Game/UI styles
├── sounds/                 # Audio assets
└── blockchain/             # Hardhat contracts and frontend integration snippets
```

## Gameplay Instructions

1. Launch the game, click **BEGIN RUN**, then click once inside the 3D view to lock the mouse pointer.
2. Use controls:
   - `W/A/S/D` → Move
   - `Mouse` → Look around
   - `Space` → Jump
   - `Shift` → Sprint (uses stamina)
   - `V` → Toggle character visibility
   - `Esc` → Pause/Resume
3. Collect coins and keep landing on new platforms to increase your score.

### Map Designer (Optional)

- `E` → Toggle design mode
- `1-5` → Select prefab types
- `R` → Rotate selected object
- `S` → Scale selected object
- `Delete` → Remove selected object

## Contributing Guidelines

Contributions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Make clear, focused changes with descriptive commit messages.
4. Open a pull request describing what you changed and why.

## License

This project is licensed under the **ISC License** (see the `license` field in [`package.json`](package.json)).
