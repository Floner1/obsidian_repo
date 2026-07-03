object: a bundle of related attributes (variables) and methods (functions)
lets say an object is a book

attributes example:
title = "The hobbit"
pages = 310
both related to the object book

methods example:
def openbook()
def readbook()
def closebook()

to create many objects, u need a class

class: (blueprint) used to design the structure and layout of an object

==u need: def dunder init dunder (self): to create an object in a class (constructor)==
class car:
	def dunder init dunder (self, model, year, colour, forsale):
			self.model = model
			self.year = year
			self.colour = colour
			self.forsale = forsale

code inside the constructor will always be executed once an object is created
car 1 and car 2 are instances of the object in class

car1 = car("R8",2023,"Green", False)
car1.model would print R8
car1.year would print 2023, so on and so on

u can make a new object in class as car 2
car2 = car("Gumpurt Apollo GT", 2007, "Purple", False)
and car2.model would do the same thing as abv



self = the object itself, from the inside. It's just the name of the first parameter in every method, and Python automatically fills it with whichever object called that method.

Objects don't have built-in names. Variables like my_car just point to an object. self is the placeholder name for that same object before it has an outside name.

self.model = model

Right side: model is the local value passed in, like "Tesla".  
Left side: self.model saves that value onto the object permanently, as an attribute.

Without self.model =, the value disappears once the method finishes. With it, you can call my_car.model later and still get "Tesla" back.

Quick mental model: class = blueprint or form letter. self = the blank that gets filled in with whichever object is using it right now.

to import class from another file, do from filename import classname

class variable

class car:
	wheels = 4 
	# this is the class variable, outside of constructor, can be used for any objects inside the class 

	numcars = 0

	def dunder init dunder (self, model, year, colour, forsale):
			self.model = model
			self.year = year
			self.colour = colour
			self.forsale = forsale
			car.numcars += 1 # points to the variable numb cars and adds 1

car1 = car("R8",2023,"Green", False)
car2 = car("Gumpert Apollo GT", 2007, "Purple", False)

so if u do print(car1.wheels) it will be 4
and if u print(car2.wheels) it will be 4

usually u would access class variable using name of class
so print(car.wheels) instead of print(car1.wheels) or whatever

access class directly and not any instances from class

car1 and car2 constructs 2 cars, therefore print(car.numcar) would be 2

**==Inheritance==**
allows a class to inherit attributes and methods of another class

class animals:

    def __init__(self, name):

        self.name = name

        self.is_alive = True

  

        def eat(self):

            print(f"{self.name} is eating")

  

        def sleep(self):

            print(f"{self.name} is sleep")

class Dog(animals): # the (classname) will inherit the stuff from that class

    def speak(self):

        print("Woof")

  

    #pass #when u inherit stuff u usually just put pass, or u can put specific stuff inside of the class that is inheriting stuff

  

dog = Dog("scooby") #create object dog using the class Dog

print(dog.name)

dog.speak()


