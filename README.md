# Hangman

This Hangman game project is a simple command-line game written in Python. The game is based on the popular word-guessing game, where players have to guess a hidden word by suggesting letters, one at a time. The user starts with 6 guesses. For each incorrect guess, user lose a guess. The player loses if the hangman is completed before they can guess the word, and wins if they are able to guess the word correctly.

## Getting Started

### Prerequisites
To run this game, you will need to have Python 3 installed on your computer. 

### Installation
To install and run the game, you can follow these steps:

1. Clone this repository or download the code as a zip file and extract it to a folder on your computer.
2. Open a terminal or command prompt and navigate to the folder containing the game code.
3. Run the following command to start the game:

```python
hangman.py
```
4. The game will start, and you can begin playing by following the instructions on the screen.

## Game Architecture and Rules:  

1. The computer selects a word at random from the list of available words that was provided in words.txt. The functions for loading the word list and selecting a random word have already been provided in hangman.py.
2. The user starts with 6 guesses.
3. At the start of the game, the computer informs the user how many letters the computer's word contains and how many guesses the user starts with.
4. The computer keeps track of all the letters the user has not guessed so far and before each turn shows the user the available letters and number of guesses left
5. The computer then asks the user to supply one guess at a time. The user can input a letter by typing it on the keyboard and pressing the Enter key.
6. Immediately after each guess, the computer tells the user whether the letter is in the computer's word or not.
7. After each guess, the computer also displays to the user the computer's word, with guessed letters displayed and unguessed letters replaced with an underscore and space (_ ).
8. At the end of the guess, the computer prints some dashes () to help separate individual guesses from each other.
9. The game continues until either the user guesses the word correctly, in which case the computer congratulates the user and displays the word, or the user runs out of guesses, in which case the computer reveals the word and informs the user that they have lost the game.
10. If the user types anything other than an alphabet, such as symbols or numbers, the computer informs the user that only alphabets are allowed as input. To account for accidental mistakes, the user will receive three warnings at the beginning of the game. Each time they make an invalid input or repeat a letter they have already guessed, they will lose a warning. If the user exhausts all their warnings and makes another invalid input, they will lose a guess instead.
11. **How to get hints**: user can guess an asterisk (*), in which case the computer will print out all the words that match that guess.

## Contributing
The implementation of game is complete. However, I have made an attempt to convert it to a Flask app and deploy it to Heroku, but it's kinda buggy. If you would like to contribute to this project for the web implementation, you can fork the repository, make your changes, and submit a pull request. Any contributions are welcome, including bug fixes, new features, or improvements to the existing code.

## License
This project is licensed under the MIT License - see the LICENSE



