# 🪙 Coin Flip Puzzle

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

**A mesmerizing brain-teasing puzzle game where strategy meets logic!**

*Turn chaos into order, one flip at a time* ✨

[🎮 Play Now](#getting-started) • [🧠 Strategy Guide](#strategy-tips) • [🔧 Customize](#features)

---

</div>

## 🌟 What Makes This Special

Transform a chaotic grid of mixed coins into perfect golden harmony! This isn't just another puzzle game – it's a mathematical masterpiece that challenges your strategic thinking and pattern recognition skills.

### ✨ Game Highlights

- **🎯 Perfect Solvability**: Every puzzle is mathematically guaranteed to be solvable
- **🎨 Stunning Visuals**: Glassmorphism design with smooth animations and particle effects
- **📱 Responsive Design**: Plays beautifully on desktop, tablet, and mobile
- **🧩 Multiple Difficulties**: Choose from 3×3 to 6×6 grids for varying challenge levels
- **🏆 Move Optimization**: Track your efficiency and aim for the perfect solution

## 🎮 How to Play

### The Rules are Simple
1. **🎯 Goal**: Turn all coins to show heads (H) - that beautiful golden state!
2. **🔄 Action**: Click any coin to flip it AND all adjacent coins (up, down, left, right)
3. **🧠 Challenge**: Achieve your goal in the fewest moves possible

### Visual Guide
```
Initial State:          After Clicking Center:
H T H T                 T H T T
T H T H        →        H T H T
H T H T                 T H T T
T H T H                 T H T H
```

## 🚀 Getting Started

### Quick Play
1. Save the HTML file to your computer
2. Open it in any modern web browser
3. Start puzzling immediately - no installation needed!

### For Developers
```bash
# Clone or download the repository
git clone https://github.com/gnurtuv/spectral-lines-course.git

# Open the game
open index.html
# or
python -m http.server 8000  # For local development
```

## 🎯 Features

### 🎨 Visual Excellence
- **Gradient Backgrounds**: Eye-catching color schemes that adapt to your actions
- **Smooth Animations**: Coins flip with realistic 3D effects
- **Particle Effects**: Celebration animations when you win
- **Modern UI**: Clean, accessible interface with hover effects

### 🧩 Gameplay Features
- **Smart Generation**: Puzzles are created by scrambling a solved state, ensuring solvability
- **Multiple Grid Sizes**: From beginner-friendly 3×3 to challenging 6×6
- **Move Counter**: Track your efficiency and compete with yourself
- **Reset Function**: Return to the initial state if you want to try a different approach
- **Hint System**: Strategic guidance when you're stuck

### 📱 Technical Features
- **Zero Dependencies**: Pure HTML, CSS, and JavaScript
- **Responsive Design**: Adapts to any screen size
- **Fast Loading**: Optimized for instant gameplay
- **Browser Compatible**: Works on all modern browsers

## 🧠 Strategy Tips

### For Beginners
- **Start with corners**: Corner coins have fewer neighbors, making effects more predictable
- **Think in patterns**: Look for symmetries and recurring configurations
- **Work backwards**: Sometimes it's easier to visualize the solution and work towards it

### Advanced Strategies
- **Learn common patterns**: Certain configurations appear frequently and have known solutions
- **Use parity**: The total number of tails changes predictably with each move
- **Master edge cases**: Edge and corner strategies are fundamental to efficient solving

### Mathematical Insight
This puzzle is based on linear algebra over finite fields (GF(2)). Each coin state can be represented as 0 (tails) or 1 (heads), and flipping is addition modulo 2. The game state space forms a vector space, and solvability depends on whether the target state lies in the span of possible moves.

## 🎨 Customization

### Easy Modifications
- **Colors**: Modify the CSS gradients to change the visual theme
- **Grid Size**: Add new options in the dropdown (requires minor JavaScript changes)
- **Animation Speed**: Adjust transition durations in CSS
- **Difficulty**: Modify the number of scrambling moves in `createGrid()`

### Advanced Customization
```javascript
// Change flip pattern (add diagonals)
const positions = [
    [row, col], [row-1, col], [row+1, col], [row, col-1], [row, col+1],
    [row-1, col-1], [row-1, col+1], [row+1, col-1], [row+1, col+1] // diagonals
];

// Modify win condition (all tails instead)
const allTails = grid.every(row => row.every(cell => cell === 'T'));
```

## 🔬 The Mathematics Behind the Magic

This game implements a variant of the famous "Lights Out" puzzle, which has fascinating mathematical properties:

- **Group Theory**: The game states form a group under the flip operation
- **Linear Algebra**: Solvability can be determined using Gaussian elimination
- **Graph Theory**: The grid represents a graph where edges determine flip relationships
- **Computational Complexity**: Finding optimal solutions is NP-complete for general graphs

## 🏆 Challenge Yourself

### Difficulty Levels
- **🟢 Beginner (3×3)**: Perfect for learning the mechanics
- **🟡 Intermediate (4×4)**: The sweet spot of challenge and fun  
- **🟠 Advanced (5×5)**: Requires serious strategic thinking
- **🔴 Expert (6×6)**: For puzzle masters only

### Personal Goals
- Solve a 4×4 grid in under 10 moves
- Complete a 5×5 puzzle in under 15 moves
- Master the 6×6 grid challenge

## 🤝 Contributing

Found a bug? Have an idea for improvement? Contributions are welcome!

### Ways to Contribute
- 🐛 Report bugs or suggest features
- 🎨 Improve the visual design
- 🧮 Add new mathematical features
- 📚 Enhance documentation
- 🎵 Add sound effects

## 📜 License

This project is open source and available under the MIT License. Feel free to use, modify, and distribute as you see fit!

## 🎉 Acknowledgments

- Inspired by the classic "Lights Out" electronic game
- Mathematical foundations based on linear algebra over finite fields
- Design influenced by modern glassmorphism trends
- Built with love for puzzle enthusiasts everywhere

---

<div align="center">

**Ready to flip your way to victory?** 🏆

*Every master was once a beginner. Every pro was once an amateur.*

**[🎮 Start Playing Now!](#getting-started)**

</div>
