<<<<<<< HEAD
This is an open-world 3D block-based exploration game similar to Minecraft. You can freely explore, build, and destroy within the procedurally generated pixel world.
=======
# Voxel Block World

A Minecraft-inspired 3D voxel exploration game built with Three.js. Runs entirely in the browser - no installation required.

## Play Now

**[Click here to play](https://applezh-11.github.io/my-space/)**

Open the link on any device (desktop or mobile) and start exploring!

## Controls

### Desktop
| Action | Control |
|--------|---------|
| Move | W / A / S / D |
| Look Around | Mouse |
| Jump | Space |
| Place Block | Left Click |
| Break Block | Right Click |
| Select Block | 1-6 Keys / Scroll Wheel |
| Pause | ESC |

### Mobile
| Action | Control |
|--------|---------|
| Move | Virtual Joystick (bottom-left) |
| Look Around | Swipe right side of screen |
| Jump | Jump Button |
| Place Block | Place Button |
| Break Block | Break Button |
| Select Block | Tap block in hotbar |

## Features

- **Procedural Terrain Generation** - Infinite world with Simplex noise-based heightmaps
- **6 Block Types** - Grass, Dirt, Stone, Sand, Wood, Leaves
- **Tree Generation** - Automatically generated trees with trunks and leaf canopies
- **Chunk System** - 16x64x16 block chunks with dynamic loading/unloading
- **Face Culling** - Only visible faces are rendered for optimal performance
- **Physics** - Gravity, collision detection, and jumping
- **Block Interaction** - Place and break blocks with raycasting
- **Mobile Support** - Touch controls with virtual joystick and action buttons
- **Pixel Art Textures** - Procedurally generated 16x16 textures

## Tech Stack

- **Three.js r160** - 3D rendering engine
- **Vanilla JavaScript** - ES Modules, no build step required
- **Simplex Noise** - Procedural terrain generation
- **WebGL** - Hardware-accelerated rendering

## Local Development

To run this project locally:

```bash
# Clone the repository
git clone https://github.com/applezh-11/my-space.git
cd my-space

# Start a local server (any of these work)
python -m http.server 5000
# or
npx serve .
# or
php -S localhost:5000
```

Then open http://localhost:5000 in your browser.

## Project Structure

```
├── index.html          # Game entry point
├── styles/
│   └── main.css        # UI styles (HUD, menus, responsive)
├── js/
│   ├── noise.js        # Simplex 2D noise generator
│   ├── voxel.js        # Core engine: blocks, textures, chunks, world
│   ├── animals.js      # Robot entity system
│   └── game.js         # Player controls, physics, game loop
└── README.md
```

## Performance

- **Render Distance**: 4 chunks (desktop & mobile)
- **Chunk Size**: 16 x 64 x 16 blocks
- **Pixel Ratio**: Capped at 2x desktop / 1.2x mobile
- **Incremental Loading**: Max 2 chunks generated per frame

## License

MIT
>>>>>>> c675444 (docs: add English README with play instructions)
