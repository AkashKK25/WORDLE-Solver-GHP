# Wordle Solver

A powerful web application that helps solve the daily [Wordle](https://www.nytimes.com/games/wordle/index.html) puzzle by suggesting possible words based on your current guesses.

![Wordle Solver Screenshot](static/screenshot.png)

## 📝 Description

Wordle Solver is an interactive tool that assists players in finding solutions for the [The New York Times](https://www.nytimes.com/)' popular word-guessing game, Wordle. The application takes your current game state (letter positions and feedback) and provides a list of possible words that match your constraints.

### Features

- Input up to 6 guesses (just like the official Wordle game)
- Color-coded feedback system (gray, yellow, green)
- Separate results for common and rare words
- Responsive design that works on desktop and mobile devices
- Intuitive UI that mimics the official Wordle game's appearance

## 🚀 Demo

Try out the live web app: [Wordle Solver](https://your-deployment-url.com)

## 💻 Technologies Used

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Python, Flask
- **Styling**: Bootstrap 5

---

## 🛠️ Installation and Setup

### Prerequisites

- Python 3.6 or higher
- pip (Python package installer)

### Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/akashkk25/wordle-solver.git
   cd wordle-solver
   ```

2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   
   # On Windows
   venv\Scripts\activate
   
   # On macOS/Linux
   source venv/bin/activate
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Run the application:
   ```bash
   python app.py
   ```

5. Open your browser and navigate to:
   ```
   http://127.0.0.1:5000/
   ```

## 📖 How to Use

1. **Start a Wordle Game**: Go to the official Wordle website and make your first guess.

2. **Input Your Guess**: Enter the same word into the Wordle Solver.

3. **Set Letter States**: Click on each letter to cycle through the states:
   - Gray (absent): Letter is not in the word
   - Yellow (present): Letter is in the word but in the wrong position
   - Green (correct): Letter is in the correct position

4. **Get Results**: Click the "Solve" button to see a list of possible words.

5. **Make Your Next Guess**: Choose a word from the suggestions for your next Wordle guess.

6. **Repeat**: Continue the process until you solve the puzzle.

## 🧩 How It Works

The Wordle Solver uses constraint-based filtering to narrow down possible words:

1. **Green Letters**: Filters for words that have the correct letter in the correct position.
2. **Yellow Letters**: Filters for words that contain these letters in any positions.
3. **Gray Letters**: Filters out words that contain these letters (unless they appear as green or yellow elsewhere).

The application uses two dictionaries:
- A common words dictionary containing frequently used 5-letter words
- A rare words dictionary for less common words


## 📞 Contact

Akash Kondaparthi - [akashkondaparthi@gmail.com](mailto:akashkondaparthi@gmail.com)

Project Link: [https://github.com/akashkk25/wordle-solver](https://github.com/akashkk25/wordle-solver)

---

### Acknowledgements

- [Wordle](https://www.nytimes.com/games/wordle/index.html) - The original game that inspired this project
- [Bootstrap](https://getbootstrap.com/) - The responsive CSS framework used
- [Font Awesome](https://fontawesome.com/) - For the beautiful icons

---

*Created with ❤️ as a portfolio project*
