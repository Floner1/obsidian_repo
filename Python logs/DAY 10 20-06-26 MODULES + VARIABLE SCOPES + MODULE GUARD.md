modules are a file that contains specific functions that can be used in your program
called by: import (module name)
or if u wanna import only certain functions u can do:
from (module name) import (function name in that module)

scope = where accessible and visible
scope resolutions: LEGB local enclosed global built in
the program will always use local first, then enclosed then global then built in

variables in functions are local
eg:
def func1():
	a = 1
	print(a)
variable a is local to func1

enclosed variable scope is when a variable is inside a function, and that function is inside another function
def func1():
	x = 1
		def func2()
			x = 2
			print(x)
	func2()
	 print(x)
	the first instance of x is in func 2, which then prints x = 2, and then afterwards the next instance of x is 1, so it prints x = 1

global = outside of functions, the normal variables u declare basically

built in is like the stuff that u find in modules
eg e in maths or pi in maths

module guard:
if dunder name dunder  == 'dunder main dunder':
	main()
for example, if u import a module, and that module has loose code that are not functions, then this guard prevents that loose code from running. 

loose code has to be placed inside the guard (main())