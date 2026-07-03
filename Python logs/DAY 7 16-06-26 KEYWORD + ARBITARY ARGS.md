keyword arguments:
def hello(greeting,title,first,last):
	print(f"{gretting} {title} {first} {last})

hello(title = "Mr.", greeting = "bonjour"...)
basically u just assign the value to the variable as u call the function, the argument dont needa be in the same pos as in the original function def, idk why and when u would needa use this im ngl

print(x, end = " ") end is a keyword argument of print(), usually end would just be \n 
print("1","2","3","4","5", sep = "-"), would print 1-2-3-4-5


arbitary arguments:
args = arguments
put either:
"star *args" for non keyword arugments
or "2 stars**for keyword arguments"

eg
def add(*args)
	print(type(args))
add(1,2,3)

will return print as a tuple, basically arguments are stored in a tuple. 
def add(*args):

    total = 0

    for arg in args:

        total += arg

    return total

  

print(add(1,2,3,4))
will return 10.

same thing btw can be written like this: 
def add(*args):
    return sum(args)
print(add(1,2,3,4))

actually pretty useful

**kwargs will return dictionary as type bc u asign a value to a key
def print_addy(**kwargs):

    for key,value in kwargs.items():

        print(f"{key}: {value}")

  

print_addy(street = "12353 fake", city = "hcm", zip = "67")

basically allow u to pass in varying number of arguments. 