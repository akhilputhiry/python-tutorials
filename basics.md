## Syntax ##
* Python uses indentation to to mark block of code like class/function definition, flow control etc
* No braces
* No semicolons
* 4 space indentation is the standard followed by the python community

```
>>> if True:
...     print 'It Worked!'
... else:
...     print 'This will never work'
... 
It Worked!
>>>
```

## Reserved words ##
* Every language has a set of reserved words which you cannot use as constant or variable or identifier name
* Following are the list of reserved words in python

```
and, exec, not, assert, finally, or, break, for, pass, class, from, print
continue, global, raise, def, if, return, del, import, try, elif, in, while
else, is, with, except, lambda, yield
```

## Data types ##
* Python has five standard data types
* Numbers, String, List, Tuple, Dictionary
* We will see the possible operations on these data types later
* This is just an overview, there are different versions of numbers saying int, float, long, complex
* Similarly string has unicode strings etc
* We will see all of them in the later part, for now just understand there are 5 basic datatypes

```
>>> a = 3
>>> type(a)
<type 'int'>
>>> 
>>> b = 'Maria'
>>> type(b)
<type 'str'>
>>> 
>>> c = [1, 2, 3, 4, 5]
>>> type(c)
<type 'list'>
>>> 
>>> d = (1, 2, 3, 4, 5)
>>> type(d)
<type 'tuple'>
>>> 
>>> e = {1: "one", 2: "two", 3: "three"}
>>> type(e)
<type 'dict'>
>>>
```

## Operators ##
* This is again common for almost all languages
* The list of operators supported in python are
  * Arithmetic operators (+, -, *, /, %, //, **)  
  * Comparison operators (==, !=, >, <, >=, <=)
  * Assignment operators (=, +=, -=, /=, %=, **=, //=)
  * Logical operators (and, or,  not)
  * Bitwise operators (&, |, ~, ^, <<, >>)
  * Membership operators (in, not in)
  * Identitiy operators (is, is not)

```
>>> # Arithmetic Operators
>>>
>>> a = 2
>>> b = 1
>>> 
>>> a + b
3
>>> a - b
1
>>> a / b
2
>>> a % b
0
>>> a // b
2
>>> a ** b
2
>>> a * b
2
>>> 
>>> # Comparison Operators
>>> 
>>> a = 1
>>> b = 3
>>> 
>>> a == b
False
>>> a > b
False
>>> a < b
True
>>> a >= b
False
>>> a <= b
True
>>> a != b
True
>>>
>>>
>>> # Logical Operators
>>>
>>> a = True
>>> b = False
>>> 
>>> a and b
False
>>> a or b
True
>>> not a
False
>>> not b
True
>>>
>>> # Membership Operators
>>> 
>>> a = [1, 2, 3, 4, 5]
>>> 1 in a
True
>>> 10 not in a
True
>>> 10 in a
False
>>>
>>> # Identity Operators
>>>
>>> a = 1
>>> 
>>> a is int
False
>>> a is 1
True
>>> a is not 2
True
>>>
>>> # Assignment Operators
>>> 
>>> a = 1
>>> a
1
>>> a += 1
>>> a
2
>>> a -= 1
>>> a
1
>>> a /= 2
>>> a
0
>>> a = 10
>>> a
10
>>> a **= 2
>>> a
100
>>>
```
