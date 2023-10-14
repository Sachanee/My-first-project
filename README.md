# **First Project**

This is my first project with git.

# _Let's play Hangman!!_


Following is a Python script of the classic game “Hangman”. A row of dashes represents the word to guess. If the player guesses a letter in the word, the script writes it in all its correct positions.  The player has 6 turns to guess the word. You can easily customize the game by changing the variables.

## Instructions

1. Open index.html in your browser to get an idea of Hangman game.

![hangman!](hangman.png)

* You can code your own hangman game to play with you friends.
1. 

* Download the dictionary file and open file for reading. 
---
```python
import random


def load_words_from_file(file_path):
    with open(file_path, "r") as file:
        words = [line.strip() for line in file]
    return words
```
* Generate random word from the dictionary
```python
def generate_random_word(word_list):
    return random.choice(word_list)


# Specify the path to your dictionary file
dictionary_file_path = "dictionary.txt"
# Load words from the dictionary file
word_list = load_words_from_file(dictionary_file_path)
random_word = generate_random_word(word_list)
```
