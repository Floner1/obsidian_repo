pass function:
	basically a placeholder, doesnt do anything

continue function
	if u place it in an if and the if runs, it will go back up to the top of the while loop

def spin_row(): 
	symbols = ['🍒', '🍉', '🍋', '🔔', '⭐'] 
	results = [random.choice(symbols) for _ in range(3)] 
	return results

string module:
contains a bunch of digits, punctuation and letters
string.punctuation = all ascii punctuation
string.digits = 0-9
string.ascii_letters = all ascii letters

put `_` as variable if u never going to use variable, u just need one there so that syntax is correct

to put a string in a list, just do:
variable = list(variable)

.copy(), allocates new memory block. if u just do variable1 = variable 2 without doing .copy on variable 2 then variable 1 just pointing at same place as variable 2. 

when printing backslash\, u have to do double backslash because python treats 1 backslash as source code

if u have to declare an empty set, use set() function

.join(): list function, concatenates elements of a list tgt 

banking:
def display_balance(balance):

    print("********************")

    print(f"Your balance is: ${balance:,}")

    print("********************")

  

def deposit(balance, amount):

    print("********************")

    print(f"You have deposited: ${amount}")

    print(f"Old balance: ${balance:,}")

    balance += amount

    print(f"New balance: ${balance:,}")

    print("********************")

    return balance

  

def withdraw(balance, amount):

    print("********************")

    print(f"Withdrawing: ${amount}")

    print(f"Old balance: ${balance:,}")

    balance -= amount

    print(f"New balance: ${balance:,}")

    return balance

  

def menu():

    print("********************")

    print("Welcome to the banking app")

    print("1. Display balance")

    print("2. Deposit")

    print("3. Withdraw")

    print("4. Exit")

    print("********************")

  

stop = False

balance = 0

  

while not stop:

    valid_input = False

    menu()

  

    while not valid_input:

        try:

            choice = int(input("Enter your choice: "))

            valid_input = True

            print(f"Valid input, you chose: {choice}")

        except ValueError:

            print("Invalid input, try again")

  

    valid_input = False

  

    match choice:

        case 1:

            display_balance(balance)

  

        case 2:

            while not valid_input:

                try:

                    amount = float(input("Enter the amount you want to deposit: "))

                    if amount <= 0:

                        print("Enter a positive amount")

                    else:

                        valid_input = True

                        print(f"Valid input, you are depositing: ${amount:,}")

                except ValueError:

                    print("Invalid input, try again")

  

            balance = deposit(balance, amount)

  

        case 3:

            while not valid_input:

                try:

                    amount = float(input("Enter the amount you want to withdraw: "))

                    if amount <= 0:

                        print("Enter a positive amount")

                    elif amount > balance:

                        print("You are withdrawing more than you have!")

                        print(f"Your current balance: ${balance:,}")

                    else:

                        print(f"Valid input, you are withdrawing: ${amount:,}")

                        valid_input = True

                except ValueError:

                    print("Invalid input, try again")

  

            balance = withdraw(balance, amount)

  

        case 4:

            print("Good bye")

            stop = True

  

        case _:

            print("Invalid input, input must be between 1-4")

word guesser:

import random

  

fruits = ("apple","oranges","coconut","pineapple","banana")

  

hangman_stages = {

                    1: (" o ",

                        "   ",

                        "   "),

                    2: (" o ",

                        " | ",

                        "   "),

                    3: (" o ",

                        "/| ",

                        "   "),

                    4: (" o ",

                        "/|\\",

                        "   "),

                    5: (" o ",

                        "/|\\",

                        "/  "),

                    6: (" o ",

                        "/|\\",

                        "/ \\"),

                }

  

def display_man(wrong_guesses):

    for line in hangman_stages[wrong_guesses]:

        print(line)

  

def display_hint(hint):

    print(" ".join(hint))

  
  

word_chosen = random.choice(fruits)

hint = ["_"] * len(word_chosen)

wrong_guesses = 0

guessed_letters = set()

stop = False

  

while not stop:

    display_hint(hint)

    user_guess = input("Enter your guess: ").lower()

  

    if len(user_guess) != 1:

        print("Your guess should only be 1 character")

        continue

    if user_guess.isalpha() == False:

        print("You can only enter letters!")

        continue

  

    if user_guess in guessed_letters:

        print("You've already guessed this letter!")

        continue

  

    if user_guess in word_chosen:

        for i in range(len(word_chosen)):

            if word_chosen[i] == user_guess:

                hint[i] = user_guess

        guessed_letters.add(user_guess)

    else:

        print("Wrong guess")

  

        wrong_guesses += 1

  

        print("*"* 20)

        display_man(wrong_guesses)

        print("*"* 20)

  

        guessed_letters.add(user_guess)

    if wrong_guesses == 6:

        print("Game lost")

        print(f"The correct word is: {word_chosen}")

        stop = True

    if "_"  not in hint and wrong_guesses < 6:

        print("You won!")

        print("".join(hint))

        stop = True