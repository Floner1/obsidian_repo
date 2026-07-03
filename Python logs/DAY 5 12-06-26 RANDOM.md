import random
help(random) for full list

all below will be random.
.randint(smallest,largest both inclusive)
.random(): give random float between 0 1
.choice(collection name): give random choice from collection
	.shuffle(collection name/sequence): shuffles the sequence randomly

number guessing game:

import random

random_number = random.randint(1,100)

  

guess_count = 0

stop = False

  

print("-----WELCOME TO THE RANDOM NUMBER GUESSER GAME-----")

print("You will have 5 guesses to guess a random number from 1 to 100")

while not stop:

    user_guess = int(input(("Enter your guess: ")))

    if user_guess == random_number:

        print(f"Correct, the random number is: {random_number}")

        guess_count += 1

        if guess_count == 1:

            print("You got it first try!")

        stop = True

    elif user_guess > random_number:

        print(f"Your guess is too high, try again")

        guess_count += 1

    else:

        print(f"Your guess is too low, try again")

        guess_count += 1

    if guess_count == 5:

        print("Game over")

        print(f"The correct number was {random_number}")

        stop = True



rock scissors paper game:

import random

stop = False

options = ("scissors", "rock", "paper")

print("-----ROCK SCISSORS PAPER GAME-----")

  

while not stop:

    pc_choice = random.choice(options)

    user_choice = input("Enter your choice (q to quit): ").strip().lower()

    print(f"The computer chose: {pc_choice}")

    match user_choice:

        case "scissors":

            if pc_choice == "scissors":

                print("Draw")

            elif pc_choice == "rock":

                print("You lost")

            else:

                print("You won!")

  

        case "paper":

            if pc_choice == "paper":        

                print("Draw")

            elif pc_choice == "scissors":

                print("You lost")

            else:

                print("You won!")

  

        case "rock":

            if pc_choice == "rock":

                print("Draw")

            elif pc_choice == "paper":

                print("You lost")

            else:

                print("You won!")

  

        case "q":

            print("Good bye")

            stop = True

  

        case _:

            print("invalid input")