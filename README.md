♟️ Chess Game

A complete chess game with a full-featured chess engine, interactive drag-and-drop support, and a polished UI. Play against yourself with all standard chess rules implemented!

<img width="569" height="639" alt="Screenshot 2026-06-18 201954" src="https://github.com/user-attachments/assets/084ef29b-5f13-4d4f-a8f0-752dbfc7401e" />


🌐 Live Demo



🎮 Features

### Complete Chess Engine
- **All Standard Rules**: Legal move validation, check, checkmate, stalemate detection
- **Special Moves**: Castling, en passant, pawn promotion with piece selection dialog
- **Turn Management**: Automatic turn switching with visual indicators

### Interactive Gameplay
- **Click-to-Move**: Select pieces and click valid squares to move
- **Drag Support**: Drag pieces on desktop for intuitive control
- **Highlight System**: Green circles show valid moves, blue highlights selected pieces

### Game Controls
- **Restart**: Reset the game at any time
- **Undo**: Step back through moves with move history
- **Flip Board**: Play from black's perspective
- **Auto-Save**: Game state persists in localStorage

### Visual Design
- **Classic Chess Board**: Wood-themed design with piece emojis
- **Move History**: Algebraic notation with numbered moves
- **Captured Pieces**: Separate displays for captured pieces
- **Game Over Detection**: Clear messages for checkmate and stalemate


🚀 How to Play

1. **Start**: Game begins with standard position. White moves first.
2. **Select**: Click a piece to select it (valid moves highlighted)
3. **Move**: Click a highlighted square or opponent's piece
4. **Special Moves**:
   - **Castling**: Drag king two squares toward rook
   - **En Passant**: Capture pawn as if it moved one square
   - **Promotion**: Choose piece when pawn reaches the end
5. **Controls**: Use buttons to restart, undo, or flip board

🛠️ Technologies Used

- **HTML5** - Game structure and layout
- **CSS3** - Responsive design, animations, theming
- **JavaScript (ES6)** - Complete chess engine and game logic
 📁 File Structure


📦 chess-game

├── 📄 index.html          # Main game interface



🧠 Chess Engine Architecture

### Core Classes

```javascript
class ChessGame {
  board: 8x8 array of piece objects
  currentTurn: 'white' | 'black'
  moveHistory: Array of move objects
  capturedPieces: { white: [], black: [] }
  
  getLegalMoves(row, col)  // Calculate all legal moves for a piece
  isInCheck(color)         // Check if king is in check
  makeMove(move)           // Execute a move with validation
  undoMove()               // Revert to previous game state
}
```


### Game States

| State | Description | Visual Indicator |
|-------|-------------|------------------|
| Playing | Game in progress | Highlighted valid moves |
| Check | King is in check | Red highlight on king |
| Checkmate | Game over - winner declared | "Checkmate! [Color] wins!" |
| Stalemate | Game over - draw | "Stalemate! It's a draw!" |

## 🔧 Installation

 **No dependencies!** Pure HTML/CSS/JavaScript - just run and play.

## 📝 Requirements

- Modern web browser (Chrome, Firefox, Safari, Edge)
- JavaScript enabled
- No internet connection required after loading

## 🎯 Future Enhancements

- [ ] AI opponent with difficulty levels (Minimax algorithm)
- [ ] Chess clock with time controls
- [ ] PGN import/export for game analysis
- [ ] Sound effects for moves and captures
- [ ] Online multiplayer via WebSocket
- [ ] Responsive design for mobile devices

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Development Tips

- **Chess Engine**: Focus on `script.js` for game logic
- **UI/UX**: Modify `style.css` and DOM manipulation in `script.js`
- **Testing**: Use the console to debug move generation and game states

## 📄 License

This project is open source and available under the **MIT License**.

## 🙏 Acknowledgments

- Chess piece design inspired by [Chess.com](https://www.chess.com)
- Testing feedback from the open-source community
- Special thanks to all contributors

---

**Made with ♟️ by [HAMZA RASHID]**

---

*Enjoy the royal game! ♚♛♜♝♞♟*
