# simple-number-guessing-game
a simple number guessing game made with python


###### I wanted to try writing code in github

```
# -*- coding: utf-8 -*-
"""
Created on Mon Mar 20 11:24:36 2023

@author: sbalam2007
"""

import random
def numGuessGame():
    num = random.randrange(1,101)
    numGuess = 7
    print("you have ", numGuess, " guesses")
    guess = int(input("enter a number from 1 to 100: "))
    while numGuess > 1:
        if guess > num:
            print("enter a smaller number")
        elif guess < num:
            print("enter a larger number")
        else:
            break
        numGuess -= 1
        print("you have ", numGuess, " guesses left")
        guess = int(input("enter a number from 1 to 100: "))
        



    if guess == num:
        print("Congrats! You guessed the correct answer!")
    else:
        print("Sorry, you were not able to guess the correct answer, the number was ", num)
```

use this to call the function:
`numGuessGame()`

