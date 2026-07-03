use def init for attributes, and def function_name for methods
the self.variable = variable is what value of the variable is received from the user

**==Multiple inheritance==**
inherit from more than 1 parent class
c(a,b)

==**Multilevel inheritance**==
inheriting from a parent that has inherited from another parent

![[multiple + multilevel inheritance.png.png|697]]

**==Super():==**
function used in child class to call methods from parent class (superclass)

You only need to use `super()` if the child class overrides (redefines) a method or constructor from the parent class but still wants to execute the parent's logic. 

If you do not override anything, you **can** just inherit the parent and move on without writing `super()`. Furthermore, this design absolutely allows child classes to have their own unique attributes alongside parent attributes without declaring them in the parent class. 

basically if child class has it own def init then u needa use super, bc if child has same method as parent, the child method will override parent. 
![[super inheritance.png]]

**==Polymorphism==**
Done either through inheritance or duck typing

**==Duck Typing:==**
another way of polymorphism, but must meet a minimum number of necessary attributes/methods
"If it looks like a duck, quacks like a duck, it must be a duck. "
as long as an object resembles another, it can be treated the same
![[Duck typing.png]]

**==Static Method:==**
method that belongs to class rather than certain object
instance method: operations on objects
static method: utility functions that dont need access to class data\
![[static methods.png]]

**==Class Methods:==**
uses cls instead of self, allows operations to the class itself
![[Pasted image 20260627144455.png]]

==**Magic Methods:**==
dunder methods int str eq
allow dev to define or customize behaviour of objects
auto called when creating new objects

