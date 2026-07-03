list comprehension, basically u can do stuff to a list without needing to use a for loop to iterate over the whole loop

list = [expression for value in iterable (iterable can be dictionaries collections and strings) if condition]

expression is whatever u do to the values in the list and what gets returned

fruits = ["apple","orange","banana"]
fruits = [fruits.upper() for fruit in fruits]
print(fruits)
will print out all upper

numbers = [-1,-2,3,4]
numbers = [nums for nums in numbers if num >= 0] # will return all pos 
numbers = [nums for nums in numbers if num <= 0] # will return all negative

grades = [52,64.22.96]
grades = [grade for grade in grades if grade >= 60]

match variable
	case 1 (or whatever case u need it to be):
		return smth
	 case __:
		 case underscore is the default, u always put it last

instead of "or" u can use | 
if day = "mon" | (or) day = "tues"

def isweekend(day):
	match day:
			case "sunday" | "saturday"
				return True
			case "mon" | "tues" | "weds" | "thurs" | "fri"
					return False
print(isweekend())

start chapter 39