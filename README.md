# Tic-Tac-Toe Against Computer 🎮

A classic game with adaptive AI built using Python and Pygame. Features intelligent computer opponent, score tracking, and dynamic win animations.

<img width="172" alt="Screenshot 2025-03-31 at 6 04 21 PM" src="https://github.com/user-attachments/assets/d0638455-11ab-4a57-9b4d-c4ee66f5d77a" />

## Features ✨

- 📊 Persistent score tracking (Player vs Computer)
- 🔍 Win detection with dynamic line drawing
- 🖱️ Responsive mouse-click controls
- 🎯 Smart Computer prioritization: Wins > Blocks > Corners > Center > Edges
- 🎨 Clean Pygame UI with constant-driven layout

## Usage 🕹️

**Basic Gameplay**
1. Launch game: `python main.py`
2. Click empty cells to place X (Player)
3. AI automatically places O (Computer)
4. Match outcomes:
   - 🏆 Win: 3-in-a-row
   - 🤝 Tie: Full board
   - 🔄 Continue: Ongoing game

**Special Actions**
- 🆕 `Mouse Click`: Start new game after match conclusion
- 🚪 `Window Close`: Quit game

## Code Structure 🏗️

### Python Modules
| File          | Components                   | Responsibility          |
|---------------|------------------------------|-------------------------|
| `main.py`     | `Game` class                 | Core game loop & logic  |
| `sprites.py`  | `Board`, `Icon`, `UIElement` | Visual elements & state |
| `settings.py` | Constants & Colors           | Configuration values    |

### Key Functions 🔑
```python
def is_winner()       # Checks 8 win conditions
def smart_ai()        # Strategic move selection
def draw_icons()      # Renders X/O markers
def board_to_pixel()  # Converts grid to screen coordinates
