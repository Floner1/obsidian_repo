 An interable is anything that can output its elements 1 at a time
all collections
dictionaries
strings

Membership operators:
in
not in

help find if an element is in collections, dictionaries or strings
word = "Apple"
guess = input("Guess a letter in the word: ")
if guess in word:
	print("Good job")
else:
	print("bad job")

grades = {"Sandy": "A",
          "Squidward": "B",
          "Spongebob": "C",
          "Patrick": "D"}

student = input("Enter the name of a student: ")

if student in grades:
    print(grades[student])
else:
    print("Student not found")

the in only finds keys