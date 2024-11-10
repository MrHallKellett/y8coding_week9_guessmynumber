# Y8 Coding Project 3: Guess My Number

## Intro

The final project for our first Python unit will be for you to create your very own **GUESS MY NUMBER** game that runs in your terminal.

## STAGE 1:

Follow the class demo to recreate the basic functionality of the game:

```
	Welcome to GUESS MY NUMBER!
	...generating my number... 
	Number generated!
	
	Guess my number:
	23
	HIGHER!
	Guess my number:	
	73
	LOWER!
	Guess my number:	
	51
	HIGHER!
	Guess my number:
	60
	LOWER!
	YOU ARE CLOSE - within 5 away!
	Guess my number:
	55
	HIGHER!
	Guess my number:
	57
	LOWER!
	Guess my number:
	56
	YOU GOT IT!!!
```

## STAGE 2:

Implement difficulty levels.

Beginner mode = 10 guesses maximum + extra feedback when within 7 away from the target number.
 
Explorer mode = 8 guesses maximum + extra feedback when within 5 away from the target number

Adventurer mode = 6 guesses maximum + extra feedback when within 3 away from the target answer

```
	WELCOME TO GUESS MY NUMBER!
	...generating my number...
	Number generated.
	Choose difficulty:
		1. Beginner
		2. Explorer
		3. Adventurer
	3
	You chose ADVENTURER mode!

	Guess my number:
	50
	LOWER!
	Guess my number:
	25
	LOWER!
	Guess my number:
	20
	LOWER!
	Guess my number:
	15
	LOWER!
	Guess my number:
	14
	LOWER!
	YOU ARE CLOSE - within 3 away!
	Guess my number:
	13
	You ran out of lives.
```

## STAGE 3:

Have your program record statistics about the user, and display these once the game has ended.

```
	Username      : bob1253
	Game number   : 6
	Difficulty    : Explorer
	Guesses made  : 6/8
	Time taken    : 45 seconds
	Best possible
	guess accuracy: 98%
```

To calculate the _best possible guess accuracy_, the program should work out the best possible guess according to the _binary search algorithm_ we talked about in the first lesson on this project (always pick the number in the middle). If the user picks the exact number, their guess accuracy is set to 100%. Otherwise, calculate a percentage based on user's guess / actual guess. Tally up each guess accuracy and calculate the average.

To help with recording the time taken, make use of the following function:

```
	from datetime import datetime
	start = datetime.now()
```
