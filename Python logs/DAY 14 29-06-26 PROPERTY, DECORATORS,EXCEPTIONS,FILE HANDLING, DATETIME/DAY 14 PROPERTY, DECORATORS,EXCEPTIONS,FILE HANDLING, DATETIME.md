==**PROPERTY:**==
@property = decorator used to define a method as a property (basically turns a method into an attribute)
adds additional logic when read, write or del an attribute
![[Property decorator.png]]

**==DECORATORS:==**
function that extends behaviour of another function without modifying base function
pass base function as argument into decorator

u need another function inside the decorator function, otherwise if u call the decorator, the decorator and applied function will run even if u dont run the function that the decorator is being applied on

basically allows u to reuse code without having to rewrite it out every time, instead u just call the decorator. ![[decorator functions.png]]

**==EXCEPTIONS:==**
an event that interrupts flow of program, usually an error
(zerodivision, type error, valueerror,etc.)
use try except

try:
try some code
execept Exception:
handle exception
finally
do some cleanup

finally always runs if called as a function
![[exceptions python.png]]

**==FILE HANDLING==**

opening a file with the "with" function means that u dont needa close it.

uname file u wanna open and what mode to open as, w is write, only overwrite if u open multiple times.

x will create a new file and write in that new file,otherwise throw error r is for read, a is for append

as file assigns the file that is being opened to a variable called "file", can name anything
![[file handling python.png|697]]
TXT FILE WRITING
![[txt file writing.png]]
JSON FILE WRITING
![[json file writing.png]]
CSV FILE WRITING:
![[csv file writing.png]]
TXT FILE READING:
![[TXT FILE READING.png]]
JSON FILE READING:
![[JSON FILE READING.png]]
CSV FILE READING:
![[CSV FILE READING.png]]
**==DATE TIME:==**
Date time formatting:
![[Date time formatting.png]]
![[datetime learning python.png]]
ALARM CLOCK
![[ALARM CLOCK.png]]