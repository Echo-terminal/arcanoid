# Arkanoid Game

A modern remake of the classic Arkanoid/Breakout game built with pure JavaScript and HTML5 Canvas. Features stunning neon visuals, smooth gameplay, and colorful brick designs.

Play the game online: https://echo-terminal.github.io/arcanoid/

## Features

- **Modern Neon Aesthetics** - Beautiful glowing effects and smooth animations
- **Colorful Bricks** - Each brick color has different point values
- **Special Coin Mechanics** - Randomly spawned coins that change all remaining bricks to their color and double points
- **Progressive Difficulty** - Ball speed increases every 100 points
- **Responsive Canvas** - Dynamically scales to fit your screen while maintaining aspect ratio
- **High Score Tracking** - Your best score is saved locally
- **Sound Effects** - Background music and death sound effects
- **Keyboard Controls** - Simple A/D or Arrow key controls
- **Pause/Resume** - Game automatically pauses when window loses focus
- **Desktop Only** - Optimized experience for PC gaming

## Gameplay

Break all the bricks by bouncing the ball with your paddle. Different brick colors award different points:

| Color | Points |
|-------|---------|
| Orange | 10 |
| Blue | 20 |
| Green | 5 |
| Cyan | 15 |
| Yellow | 25 |

### Special Mechanics

- **Coin Bricks** (5% spawn rate): When hit, transforms all remaining bricks to the coin's color and doubles the points earned
- **Speed Increase**: Ball accelerates by 5% every time you score 100 points
- **Paddle Physics**: Ball angle changes based on where it hits the paddle for strategic gameplay

## Controls

- **A / Left Arrow** - Move paddle left
- **D / Right Arrow** - Move paddle right
- **Space** - Start/Restart game
- **Window Blur** - Automatically pauses game

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- Desktop computer (mobile devices are blocked)

### Installation

1. Clone the repository
2. Navigate to the project directory
3. Open `index.html` in your web browser

No build process or dependencies required - just open and play!

### Or play online

You can also play this game online: https://echo-terminal.github.io/arcanoid/

## Project Structure

```
arcanoid/
│
├── index.html          # Main HTML file
├── css/
│   └── style.css       # All styles and animations
├── js/
│   ├── game.js         # Core game logic and mechanics
│   └── app.js          # Application initialization
├── bit.mp3         # Background music
└── Dead.mp3        # Death sound effect
```

## Technical Highlights

### Canvas Rendering
- Custom rounded rectangle polyfill for older browsers
- Neon glow effects using canvas shadow properties
- Smooth 60 FPS gameplay using requestAnimationFrame

### Responsive Design
- Dynamic canvas scaling based on container size
- Maintains aspect ratio across different screen sizes
- Scales all game elements proportionally

### Physics Engine
- Realistic ball bouncing mechanics
- Paddle angle influence on ball trajectory
- Consistent ball speed with directional control

### State Management
- Lives system with game over handling
- Level progression with brick regeneration
- Pause/resume functionality
- High score persistence using localStorage

## Customization

### Changing Brick Colors/Points

Edit the Colors array in game.js to modify brick colors and their point values.

### Adjusting Game Difficulty

Modify the ball speed, brick row count, and brick column count values in the ArkanoidGame constructor.

### Coin Spawn Rate

Change the probability in the createBricks() method to adjust how often coin bricks appear.

## Known Issues

- Mobile devices are intentionally blocked from playing
- Game requires modern browser with Canvas API support
- Audio autoplay may be blocked by some browsers

## Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## License

This project is open source and available under the MIT License.

## Acknowledgments

- Inspired by the classic Atari Breakout and Taito's Arkanoid
- Font: Press Start 2P for retro gaming feel

## Contact

Project Link: https://github.com/Echo-terminal/arcanoid

---

**Enjoy breaking some bricks!**
