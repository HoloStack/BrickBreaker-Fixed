# BrickBreaker Game (Java 17 Compatible)

A classic Brick Breaker game implemented in Java with Swing, featuring updated compatibility for Java 17.

## 🎮 Features

- **Classic Gameplay**: Control a paddle to bounce a ball and break bricks
- **Power-ups**: Various power-ups including paddle size changes, extra balls, and speed modifications
- **Multiple Lives**: 3-life system with ball respawn
- **Score System**: Track your progress as you break bricks
- **Keyboard Controls**: Smooth paddle movement with arrow keys or WASD
- **Sound Effects**: Audio feedback for collisions (requires sound files)

## 🚀 Quick Start

### Prerequisites
- Java 17 or higher
- Maven (optional, for advanced building)

### Building and Running

#### Option 1: Using Java directly (Recommended)
```bash
# Clone the repository
git clone https://github.com/HoloStack/BrickBreaker-Fixed.git
cd BrickBreaker-Fixed

# Compile the game
mkdir -p build/classes
javac -d build/classes src/main/java/com/mycompany/brickbreaker/*.java

# Run the game
java -cp build/classes com.mycompany.brickbreaker.Brickbreaker
```

#### Option 2: Using Maven
```bash
# Clone the repository
git clone https://github.com/HoloStack/BrickBreaker-Fixed.git
cd BrickBreaker-Fixed

# Compile and run with Maven
mvn clean compile exec:java
```

## 🎯 Controls

- **Left Arrow** or **A**: Move paddle left
- **Right Arrow** or **D**: Move paddle right  
- **Enter**: Restart game when game over

## 🛠️ Technical Details

- **Language**: Java 17
- **GUI Framework**: Swing
- **Build System**: Maven
- **Architecture**: Object-oriented design with separate classes for game objects

### Project Structure
```
src/main/java/com/mycompany/brickbreaker/
├── Brickbreaker.java    # Main class and game window
├── Gameboard.java       # Game logic and rendering
├── Ball.java           # Ball physics and behavior
├── Paddle.java         # Paddle control and movement
├── Brick.java          # Individual brick properties
├── Grid.java           # Brick layout management
├── PowerUp.java        # Power-up system
├── Sounds.java         # Audio management
└── Object.java         # Base game object class
```

## 🔧 Recent Fixes

This version includes important compatibility fixes:
- ✅ Updated from Java 11 to Java 17 compatibility
- ✅ Fixed `ArrayList.getFirst()` method calls for broader Java version support
- ✅ Verified compilation and runtime functionality
- ✅ Maintained all original game features and mechanics

## 🎵 Audio Setup (Optional)

Place sound files in the `sounds/` directory:
- `Hit.mp3` - Brick collision sound
- Add other sound effects as needed

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

## 🎯 Game Rules

1. Use the paddle to keep the ball in play
2. Break all bricks to advance
3. Collect power-ups for special abilities:
   - **Type 1**: Increase paddle size
   - **Type 2**: Decrease paddle size  
   - **Type 3**: Extra ball
   - **Type 4**: Increase ball speed
   - **Type 5**: Decrease ball speed
4. You have 3 lives - don't let the ball fall off the screen!
5. Press Enter to restart when the game ends

---

**Enjoy the game!** 🎮✨
