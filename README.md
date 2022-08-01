
# Higher-lower game in python

The higher-lower game is the name of some Instagram 
accounts will be displayed, you have to guess which has a higher 
number of followers by typing in the name of that account. Make sure 
you type the name exactly as shown. If the answer is correct, one of 
the accounts will stay, and some other account will be displayed to 
compare to. We will develop the game using basic concepts of Python.
The link for the actual game: http://www.higherlowergame.com.


## Requirement:
We have created the ASCII module which contains ASCII art with 
the name "higherlower_art". To import that module in the 
main.py we used:

- from higherlower_art import log
- from higherlower_art import vs
Similarly, we have created another module called "game_data" which contains the dictionary of the data which we're going to use in our code. 
To import that module in the main.py we used:
- from game_data import data
- import random

## How code works:
- Generating a random account from the game data. Used the random.choice function that returns the random entries from the dictionary named "data". We need two random accounts because we have to compare A to B.
- Formatting the account data into a printable format. We have created the function named "def format_data()" and take the input in the function as "account".
- Ask the user for a guess by using the 'input' function. We also used the lower() function because the user can enter either the upper or lower case input.
- Get a followers count for each account. There is a function for this called " def check_answer()" with the inputs guess, a_followers, b_followers. is_correct is the variable that checks answers for guess, a_followers and b_followers. is_correct.
- Give user feedback on their guess. Using the if condition with the is_correct variable.
- Keep the record of the Score. Created the variable named Score = 0, each time the user play it added the score and showed the  current score if they get it right and final score if they get it wrong.
- Making an account at position B becomes the next account at position A. For that, we have created the variable "account_b = random.choice(data)" outside the while loop. Inside the while loop like:

##### account_a = account_b

account_b = random.choice(data)


## Screenshots

![App Screenshot](https://github.com/Saad-data/higherlower_game-in-python/blob/main/Screen%20Shot%202022-08-02%20at%2002.59.07.png)


## Authors

- [@saad-data](https://www.github.com/octokatherine)


## Feedback

If you have any feedback, please reach out to us at syedsaad047@gmail.com

