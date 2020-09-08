# PythonLab2
Working with Strings & For Loops

# An overview of Strings in Python
Source: [invent with Python](https://inventwithPython.com)

What can we do with Strings in Python?? 

- String Concatenation with +
- String Replication with *
- Getting Characters from Indexes
- Negative Indexes
- Slicing Strings
- String Length
- Other String Methods (Functions)

### String Concatenation & Replication
Strings can be concatenated using "+" as long as both are the same data type.  (Both strings = concacentation and both ints/floats = addition).  An integer or float can be converted by using `str(value)`.  

Strings can also be replicated using the * symbol.  

```
>>>'Omaha'* 4 
'OmahaOmahaOmahaOmaha'

>>> mascot = 'Eagles'
>>> mascot = mascot * 3
'EaglesEaglesEagles'
```

### String Indexing
Strings used 0-based indexing (same as Java and JavaScript).  Any character in a string can be accessed by using [] and specify which the index of the desired character.  

```
>>> course_name = Cybersecurity
>>> course_name[0]
'C'
>>> course_name[3]
'e'
>>> 'Central'[2]
'n'
```

### Negative Indexes
Negative indexes start at the end of the string and go backwards.  
```
>>>'Central'[-1]
'l'
>>>'Central'[-2]
'a'
>>>'Central'[-3]
'r'
>>>'Central'[-7]
'C'
```
This could be used rather than needed to use the length - 1 to obtain the last value or other values near the end of the string.  

### Slicing Strings
String slicing uses the syntax [a:b].  'a' being the first index, inclusive and 'b' being the last index, exclusive. 

[:a] would show the characters from the beginning of the string up to, but not including a. 
[a:] would show the character at index a to the end of the String

Negative Indexing can also be used in conjuction with slicing.  

```
>>> full_name = 'Stephen Curry'
>>> full_name[0:5]
'Steph'
>>> full_name[8:]
' Curry'
>>> full_name[:5]
'Steph'
>>> full_name[-5:]
'Curry'
```

### String Length
Similar to `.length` in JavaScript and `.length()` in Java, Python uses `len(string)` to return the length of the string.  

```
>>>name = 'Bill'
>>>print(len(name))
4
```

### Other String Methods
String Methods use the '.' operator with a string or variable pointing to the string.  

name.replace()
name.split(",")

- `strip()` removes any whitespace from the beginning or end.  
- `replace()` replaces a string with another string
- `split()` splits the string into substrings if it finds instances of the seperator

You can explore more about string with Python by going to the following:
[W3Schools](https://www.w3schools.com/python/python_strings.asp)
[geeksforgeeks.org](https://www.geeksforgeeks.org/python-strings/)

---

# For Loops
Remember that a for loop is really a while loop.  In java/javascript the for loop has a special syntax to make the initialization, condition, change more concise.  

Python is a bit different.  A for loop in Python is more designed to iterate over lists, arrays and strings rather than being used to repeat a process a given number of times. Basically anything index-based. 

```
for letter in 'Central':
  print('the letter is',letter)

'the letter is C'
'the letter is e'
'the letter is n'
'the letter is t'
'the letter is r'
'the letter is a'
'the letter is l'
```
Remember the equivalent while loop would be:
```
i = 0
while i < len('Central'):
  letter = 'Central'[i]
  print('the letter is', letter)
  i = i + l

```
It's important to note that 'letter' can be anything we want. I could use any name, but it is best practice to name it something within the context of what you are iterator over.  

```
playlist = ['Let it Be', 'Something', 'Octopus's Garden', 'The Long and Winding Road', 'Because', 'Golden Slumbers'] 

for songs in playlist:
  print(songs[:4])
```

There is the function range() that exists to creates a specific number of times for a loop to run.  

```
for num in range(6):
  print(num)

0
1
2
3
4
5
```
Again 'num' could be whatever we wanted.  
Range can also be `range(a,b)` that would specify a starting value (inclusive) and ending value (exclusive).  
Range also can have `range(a,b,c)` which c represents a step to count by (default step is 1)

```
for x in range(2, 12, 3):
  print(x)

2
5
8
11
```
---
## Python Scripting Practice
- Write a function `flip_it()` that reverses and prints whatever the user inputs.  

- Write a function `email_validate()` that takes an email address and determines if it is a valid address. ex: __ @ ___.___ or something similar.  

- 


