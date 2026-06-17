# Blackjack Game in Python

A simple command-line Blackjack game built using Python. This project simulates the classic casino card game where the player competes against the computer (dealer) to get as close to **21** as possible without going over.

## Features

* Random card dealing using Python's `random` module
* Blackjack detection (Ace + 10-value card)
* Automatic Ace value adjustment (11 → 1 when needed)
* Dealer follows Blackjack rules (draws until score reaches 17)
* Win, lose, and draw result handling
* Clean and beginner-friendly code structure

## Project Structure

```text
blackjack-game/
│
├── main.py
├── art.py
└── README.md
```

## Requirements

* Python 3.x

## Installation

1. Clone the repository:

```bash
git clone https://github.com/echoesofnil/blackjack-game.git
```

2. Navigate to the project folder:

```bash
cd blackjack-game
```

3. Run the game:

```bash
python main.py
```

## How to Play

1. Start the game.
2. You and the computer are dealt two cards each.
3. Only the computer's first card is shown.
4. Choose:

   * **y** → Draw another card.
   * **n** → Pass your turn.
5. The dealer draws cards until its score reaches at least 17.
6. The winner is decided according to standard Blackjack rules.

## Card Values

| Card  | Value      |
| ----- | ---------- |
| Ace   | 11 or 1    |
| 2-10  | Face Value |
| Jack  | 10         |
| Queen | 10         |
| King  | 10         |

## Blackjack Rules Used

* Blackjack = Ace + 10-value card (score 21 with only 2 cards)
* If an Ace causes the score to exceed 21, its value changes from 11 to 1
* Dealer must keep drawing until reaching a score of 17 or higher
* Going over 21 results in a bust (automatic loss)

## Example Gameplay

```text
Your cards: [10, 7], current score: 17
Computer's first card: 9

Type 'y' to get another card, type 'n' to pass: y

Your cards: [10, 7, 3], current score: 20
Computer's first card: 9

Type 'y' to get another card, type 'n' to pass: n

Your final hand: [10, 7, 3], final score: 20
Computer's final hand: [9, 8], final score: 17

You win
```

## Concepts Practiced

* Functions
* Lists
* Loops (`while`, `for`)
* Conditional Statements
* Random Module
* Code Reusability
* Game Logic Implementation

## Future Improvements

* Multiple decks
* Betting system
* Graphical User Interface (GUI)
* Card graphics
* Multiplayer support

## License

This project is open-source and available under the MIT License.
