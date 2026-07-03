day 4:
lists:
{element} in {list name} return true or false whether that element in list or not

list[index] = "", anything in "" will replace the current thing in that index of list
all below will be nameofcollection.
LISTS:
.insert(index, what to add)
.sort(sort ascending)
.reverse(): print out list back to front based on index
to sort desc, sort first then do reverse
.clear() to clear all elements in collection
.index(element in list) return index of element in list, otherwise error
.count(element) count how many times smth is in a collection
.pop(element) removes either 

SETS:
.sort(sort ascending)
.reverse(): print out list back to front based on index
to sort desc, sort first then do reverse
.clear() to clear all elements in collection

TUPLES
.sort(sort ascending)
.reverse(): print out list back to front based on index
to sort desc, sort first then do reverse
.clear() to clear all elements in collection

if u print a set{}, different order every time printed
eg if fruits was {}, then print(fruits{}) would be elements in random order every time print
SETS:
.add(element) will add element to set
.remove(element) 
.pop() randomly remove element

 dictionaries:
collection of {key:value} pairs
capitals = {"USA": "Washington D.C.", "India": "New Delhi", "China": "Beijing", "Russia": "Moscow"}
print(dir(capitals)) will show all methods of dictionaries
print(help(capitals)): in depth of all methods

to get value. do this:
.get(key)
if no found then return none

to append or change key/value, do this:
dictionary.update({"new/current key","new value"})
to remove:
dictionary.pop(key)
.popitem(): remove latest key/value in dictionary
.clear()
.keys(): gets all keys, but no values
.values(): return all values, no keys
.items(): return both keys and values
for key, value in capitals.items():
	print(f"{key}: {value}")
display the key and its value, eg USA : Washington D.C.

start chapter 27

cinema snacks:

menu = {

    "pizza": 3.00,

    "nachos": 4.50,

    "popcorn": 6.00,

    "fries": 2.50,

    "chips": 1.00,

    "pretzel": 3.50,

    "soda": 3.00,

    "lemonade": 4.25

}

  

cart = []

total = 0

stop = False

  

while not stop:

    exists = False

    print("------------MENU-------------")

    for items,price in menu.items():

        print(f"{items:10}: ${price:.2f}")

    print("-----------------------------")

    item = input("Enter what you want (q to quit): ")

    item = item.lower()

    if item == "q":

        print("Good bye")

        stop = True

    else:

        while not exists:

            if menu.get(item) is not None:

                print("\nGreat choice\n")

                cart.append(item)

                for i in range(len(cart)):

                    print(f"-----Your current cart-----")

                    print(f"Item {i+1}: {cart[i].capitalize()}\n")

                print("-------------------")

                exists = True

            else:

                print("Invalid input, try again.")

                item = input("Enter what you want (q to quit): ")

  

print("-----Your Final Cart-----")

for i in range(len(cart)):

    print(f"Item {i+1}: {cart[i]}")

    total = total + menu.get(cart[i])

  

print(f"\nYour total is: ${total:.2f}")

answering questions:

questions = ("q1","q2","q3","q4","q5")

options = (("A. 1", "B. 2","C. 3", "D. 4"),

           ("A. 1", "B. 2","C. 3", "D. 4"),

           ("A. 1", "B. 2","C. 3", "D. 4"),

           ("A. 1", "B. 2","C. 3", "D. 4"),

           ("A. 1", "B. 2","C. 3", "D. 4"))

answers = ("a","b","c","d","a")

guesses = []

score = 0

question_numb = 0

  

for question in questions:

    guess_numb = 0

    correct = False

    ans = ""

    print("----------------")

    print(question)

    for option in options[question_numb]:

        print(option)

    while not correct:

        ans = input("Enter your answer: ")

        ans = ans.lower()

        if ans == answers[question_numb]:

            print("Correct")

            correct = True

            guess_numb += 1

            guesses.append(guess_numb)

            question_numb +=1

        else:  

            print("Wrong, try again: ")

            guess_numb += 1

for i,guess in enumerate(guesses):

    print(f"Your number of guesses for question {i+1}: {guess}")

  

    #why tf would u use like question in questions for the loop

    #just use a damn counter