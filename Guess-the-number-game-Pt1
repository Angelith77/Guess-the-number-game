import random

number = random.randint(1, 100)
attempts = 0
level = input("What is the level you want? (easy, medium, hard): ").lower()

if level == "easy":
    max_attempts = 10
elif level == "medium":
    max_attempts = 6
elif level == "hard":
    max_attempts = 3
else:
    print("Invalid level, defaulting to medium.")
    max_attempts = 6

while True:
	try:
		player_input = int(input("Guess the number:(between 1 and 100) "))

	except ValueError:
		print("Sorry, that's not a number.")
		continue
	attempts += 1

	if player_input == number:
		print(f" Correct! You won in {attempts} tries!")
		break
	elif player_input < number:
		print("Too low!")

	else:
		print("Too high!")

	if attempts == max_attempts:
		print("Sorry, you lose. you ran out of tries.")
		break
