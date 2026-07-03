day 2

ternary operator/conditional expression:
x if condition else y
eg:
num = 5
print("Positive" if num > 0 else "negative")

string methods:
len(): length of str, include spaces

all below will be variable.smth()

.find(): find first occurrence of specific char
.rfind(): find last occurrence of specific char
no found = return -1
.capitalize(): uppercase first char of string, everything else lower
found confusing at first bc thought it was everything upper, then learn later it only first char
.upper(): everything upper
.lower(): everything lower
.isdigit(): bool, str only contain digits
.isalpha(): bool, str only contain chars
.count(): count no. occurrence smth in str
.replace(1,2): replace all occurrences of 1 with 2.

print(help(str)): output all available string methods

string index:
string[start (inclusive) : end (exclusive) : step]
string[:6] means start of string up to 6th char
string[5:] means 5th char in string up to end
string[-1] would start from end of string, instead of start of string. eg if string = "hello", then would be olleh
string[-1] would be o

