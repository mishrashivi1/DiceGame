# 🎲 Dicee — Two Player Dice Game

A fun and simple two-player dice game built with HTML, CSS, and JavaScript. Refresh the page to roll the dice and find out who wins!

## 📸 Preview

<img width="1920" height="1032" alt="Screenshot (84)" src="https://github.com/user-attachments/assets/80edb1d7-59a4-4700-ad36-1029f53c2fc8" />

The app displays:
- A bold winner announcement (e.g., **"Player 2 Wins!"** or **"Draw!"**)
- Two large dice images side by side — one for each player
- Player 1 and Player 2 labels
- A flag icon next to the winner heading

## 🚀 Features

- Two-player dice roll on every page load
- Randomly generates a dice value (1–6) for each player
- Announces the winner or a draw
- Dice images update to match the rolled number
- Dark-themed, stylish UI with custom fonts

## 🛠️ Tech Stack

- **HTML** (`dicee.html`) — Page structure
- **CSS** (`styles.css`) — Dark theme, font styling, layout
- **JavaScript** (`index.js`) — Random dice logic and DOM manipulation
- **Images** (`images/`) — Dice face images (dice1.png to dice6.png)

## 🔧 Setup & Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/mishrashivi1/DiceGame
   cd dicee
   ```

2. **Open in browser:**

   ```bash
   open dicee.html
   ```

   Or rename `dicee.html` to `index.html` so it loads automatically on any server:

   ```bash
   mv dicee.html index.html
   ```

## 🖥️ How It Works

1. On every page load, JavaScript generates two random numbers between 1 and 6.
2. The dice image for each player is updated to match their rolled number.
3. The two numbers are compared:
   - If Player 1's number is higher → **"Player 1 Wins! 🚩"**
   - If Player 2's number is higher → **"Player 2 Wins! 🚩"**
   - If both are equal → **"Draw!"**

```javascript
let randomNumber1 = Math.floor(Math.random() * 6) + 1;
let randomNumber2 = Math.floor(Math.random() * 6) + 1;
```

## 📁 Project Structure

```
dicee/
├── images/
│   ├── dice1.png
│   ├── dice2.png
│   ├── dice3.png
│   ├── dice4.png
│   ├── dice5.png
│   └── dice6.png
├── dicee.html       # Main HTML file
├── styles.css       # Styling and dark theme
├── index.js         # Game logic
└── README.md        # Project documentation
```

## ⚠️ Notes

- Refresh the page to roll again — no button needed!
- Make sure the `images/` folder is in the same directory as `dicee.html`.
- Rename `dicee.html` → `index.html` to avoid directory listing issues on GitHub Codespaces.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
