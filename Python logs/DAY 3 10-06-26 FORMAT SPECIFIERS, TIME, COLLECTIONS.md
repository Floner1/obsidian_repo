day 3

string format specifiers:
used with an f string
formula: print(f"{variable:specifier)")

decimal: :.2f = 2dp, :.3f = 3dp
spaces: :10 means 10 spaces to display output, eg print(f"hello {name:10}") = hellopeter , use 10 spaces to display output
print(f"hello {name:015}") will zero pad spaces = 00000hellopeter
print(f"hello {name:<15}"), left justify, leave spaces after output will zero pad spaces = hellopeter12345 spaces
vice versa for right justify
center align is ^
:+ will display number preceded with their sign, eg print(f"Hello {num}) will display num = +52134 if num > 0, and -52134 if num < 0
or :space will do the same as :+ for pos numbers
:, will separate thousands in numbers

can combine specifiers, eg :,.2f will separate thousands and do 2dp

for loops
for variable in range(inclusive numb, exclusive numb):
reversed(range()) to count backwards, or range(x,y, negative numb)
continue with skip over a specific iteration in the for loop

eg:
for x in range (1, 21):
	if x == 13:
		continue 
		#skips over 13
	else:
		print(x)

time library, bunch of functions to do with time
time.sleep(x) is pause for x number of s before do 

more print stuff
for x in range(1,10):
	print(x, end = "") 
will make output be this: 123456789 instead of each number being on separate line
default of print is print(x,\n), end = "" stops this, u can make end = "-" and it will be 1-2-3...

collections:
lists[] : ordered + changable, ok duplicates
sets{}: unordered + immutable, no duplicates, add/remove ok
tuple():ordered  + unchangable, duplicates ok

COLLECTIONS STUFF:
eg. fruits = ["apple","banana","mango","dragon fruit]
fruits[0:2] would give all values from index 0 to index 2
fruits[::2] will give you every second element, "apple" and "mango"
fruits[::-1] will output all stuff in list backwards

for fruit in fruits:
	print(fruit) 
#prints all elements in fruits

for i,fruit in enumerate(fruits)
	print(f"Item {i+1}: ,fruit)
output will be: 
Item 1: apple
Item 2: banana
...
#prints out the current position in list and the element in list

print(dir(fruits)) will give all functions available for the collection
print(help(fruits)) will give description of all functions available for collection

