
# Hangman

# Table of Contents
1. [Introduction](#introduction)
2. [Section 1](#Setting up the environment)
3. [Section 2](#Creating the variables for the game)
4. [Section 3](#Checking if the guessed character is in the word)
5. [Section 4](#Creating the Game class)
6. [Section 5](#Putting it all together)
7. [Section 6](#Installation Instructions)
8. [Section 7](#Usage Instructions)
9. [Section 8](#License Information)
    
## Introduction

This project was built as my first introduction to AiCore. Creating the classic game Hangman required me to implement variables as well as Object Oriented programming.

## Setting up the environment

In this project, I use GitHub to track changes to my code and save them online in a GitHub repo. 

## Creating the variables for the game

I needed to use basic python commands, such as if-else statements and while loops. I first created a file named milestone_2.py which would contain the code. I created a list containing the names of my 5 favourite fruits and assigned the list to a variable called word_list. I then needed to choose a random word from the list. I did this using the 'random' module. Next, I asked the uer for an input using the input() function. I used this functio to ask the user to guess a single letter, and assigned the input to a variable called guess. I used if and else statements to check the input was a single charactr. 


## Checking if the guessed character is in the word

This code will continously ask the user for a letter and validate it. I created a script called milestone_3.py for this code. I created a while loop setting condition to true. I ask the user to guess a letter, assigning this a variable called guess. I check the guess is a single alphabetical character using the isalpha method. If the guess passes teh checks it breaks the loop, otherwise a message prints saying "Invalid letter. Please, enter a single alphabetical character."  Similarly I use if-else statements to check whether the guess is in the word.

## Creating the Game class

I created another script called milestone_py, and defined the __init method of the Hangman class. Inside the class I initialised different attributes: 

word: The word to be guessed, picked randomly from the word_list. 
word_guessed: list - A list of the letters of the word, with _ for each letter not yet guessed. For example, if the word is 'apple', the word_guessed list would be ['_', '_', '_', '_', '_']. If the player guesses 'a', the list would be ['a', '_', '_', '_', '_']
num_letters: int - The number of UNIQUE letters in the word that have not been guessed yet
num_lives: int - The number of lives the player has at the start of the game.
word_list: list - A list of words
list_of_guesses: list - A list of the guesses that have already been tried. 

 I would then create a method that will ask the user to guess a letter and another method that will check if the guess is in the word. The method was extended to define what happened if the letter was in the word, with a for-loop. An else statement as used if the letter was not in the word. The else block would reduce the number of lives by one and print a message saying "Sorry, {letter} is not in the word." and "You have {num_lives} lives left."

## Putting it all together

Here I could code the logic of the game. I made a new script called milestone_5.py and copied all of the code from milestone_4.py. I created a function called play_game that took word_list as a parameter. Inside the function, I wrote the code to:

-Create a variable called num_lives and assign it to 5
-Create an instance of the Hangman class. Do this by calling the Hangman class and assign it to a variable called game
-Pass word_list and num_lives as arguments to the game object
-Create a while loop and set the condition to True. In the body of the loop, do the following:
-Check if the num_lives is 0. If it is, that means the game has ended and the user lost. Print a message saying 'You lost!'
-Check if the num_letters is greater than 0. In this case, you would want to continue the game, so you need to call the ask_for_input method.
If the num_lives is not 0 and the num_letters is not greater than 0, that means the user has won the game. A message would print saying 'Congratulations. You won the game!'

Outside the function, I would call my play_game function to play my game.

## Installation instructions

To carry out section 2 of this project, you will need to have VSCode installed on your machine. 

## License information




