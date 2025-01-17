Lab 2: Guess the number
Write a program that let's the user running it play a game where they have to guess a number between 1 and 25
The player gets 5 guesses to guess the number, and potentially 6 if they guess close to the chosen number.

Rules:
- Name your `.py` file according to the usual expected convention: `lastName_firstName_lab2.py`
- The player should be able to run the game within the terminal or command prompt with either:
       `python LastName_FirstName_lab2.py`  or `python3 LastName_FirstName_lab2.py`
- when the player is within 3 of the correct number, their max guess count increases by 1 
  (ex. correct number is 20, player guesses a number between 17-23, but doesn't guess 20, they get an extra guess)
- when the players gets an extra guess, they don't get any more extra guesses for the rest of the game.
  (ex. correct number is 20, players previously guessed 17, guesses 18, doesn't get any more bonus guesses, the `guess_count` 
  increments as it normally would )
- Every prompt to guess must show remaining guesses OR show what guess out of MAX GUESSES they are at (be mindful of the bonus guess)
- A guess doesn't count if it's not between 1 and 25, the `guess_count` doesn't change, the user must guess again. 
  ( `< 1` doesn't count, ` > 25` doesn't count)
- When the player guesses the correct number, they win and the program exits the game.
- When the player runs out of guesses, they lose and the program exits the game.

Add print statements to indicate when the following conditions are met:
- The player is prompted to guess a number in the given range
- The player guesses the number, and wins (the program should then finish)
- The player runs out of guesses and loses
- The player is within +/- 3 of the correct number, and gets an extra guess
- The player is within +/- 3 of the correct number, but doesn't get any more guesses
- The game scolds the user if a number is greater than 25 or less than 1, does not use a guess
