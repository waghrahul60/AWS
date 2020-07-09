```python
print("Hello BestOfBest.in")
```

    Hello BestOfBest.in
    


```python
print('Hello  hfjsdsdfgfgjhfgsdhgfsdhgghfsdhgggggggg',end=' ')
print('This is a python training')
print('This is a new line')
```

    Hello  hfjsdsdfgfgjhfgsdhgfsdhgghfsdhgggggggg This is a python training
    This is a new line
    


```python
help(len)
```

    Help on built-in function len in module builtins:
    
    len(obj, /)
        Return the number of items in a container.
    
    


```python
# This is a comment
```


```python
''' This is a multiline
comment we are testing with
multiple line '''

print("Multiline comment above")
```

    Multiline comment above
    


```python
import keyword
keyword.iskeyword('and')
```


```python
print('new cell')
```

    new cell
    

## Intgers
## There is effectively no limit to how long an integer value can be


```python
print(123456789101010101010101001010101010101001010101010101010111111111111111111111111111111111111111111111)
```

    123456789101010101010101001010101010101001010101010101010111111111111111111111111111111111111111111111
    


```python
print(10)
```

    10
    


```python
a=10
print('a is equal to ', a)
print(a, 'is assigned to to variable a')
```

    a is equal to  10
    10 is assigned to to variable a
    


```python
type(a)
```




    int




```python

```

## Floating-Point Numbers

## float values are specified with a decimal point
## Optionally, the character e or E followed by a positive or negative integer


```python
4.2
```




    4.2




```python
b = 5.244
```


```python
type(b)
```




    float



## Almost all platforms represent Python float values as 64-bit “double-precision” values, according to the IEEE 754 standard. In that case, the maximum value a floating-point number can have is approximately 1.8 ⨉ 10308. Python will indicate a number greater than that by the string inf


```python
1.79e308
```




    1.79e+308




```python
1.8e308
```




    inf



## The closest nonzero number can be to zero, is approximately 5.0 ⨉ 10-324. Anything closer to zero than that is effectively zero


```python
5e-324
```




    5e-324




```python
1e-325
```




    0.0



## Complex Numbers


```python
2+3j
```




    (2+3j)




```python
a = 2+3j
```


```python
type(a)
```




    complex



## Strings


```python
print("Welcome CDAC batch to String Introduction ")
```

    Welcome CDAC batch to String Introduction 
    


```python
type("Welcome")
```




    str




```python
...
```




    Ellipsis




```python
print("This string contains a single quote (') character.")
```

    This string contains a single quote (') character.
    


```python
print('This string contains a double quote (") character.')
```

    This string contains a double quote (") character.
    


```python
print('This string contains a single quote (\') character.')
```

    This string contains a single quote (') character.
    


```python
print('a\
... b\
... c')
```

    abc
    


```python
print('c:\\home\\users')
```

    c:\home\users
    


```python
print('foo\tbar')
```

    foo	bar
    


```python
print('foo\nbar')
```

    foo
    bar
    

## Raw Strings


```python
 print(r'foo\nbar')
```

    foo\nbar
    


```python
a=10
print(f'a is equal to',a)
```

    a is equal to 10
    


```python
print('''This string has 
a single (') and 
a double (") quote.''')
```

    This string has 
    a single (') and 
    a double (") quote.
    

## Boolean


```python
type(True)
```




    bool




```python
type(False)
```




    bool




```python
type(1==2)
```




    bool



# Built-In Functions
# Math
## Function	Description
## abs()	Returns absolute value of a number
## divmod()	Returns quotient and remainder of integer division
## max()	Returns the largest of the given arguments or items in an iterable
## min()	Returns the smallest of the given arguments or items in an iterable
## pow()	Raises a number to a power
## round()	Rounds a floating-point value
## sum()	Sums the items of an iterable


```python
a=5
b=7
abs(a)
```




    5




```python
help(abs)
```

    Help on built-in function abs in module builtins:
    
    abs(x, /)
        Return the absolute value of the argument.
    
    


```python
help(sum)
```

    Help on built-in function sum in module builtins:
    
    sum(iterable, start=0, /)
        Return the sum of a 'start' value (default: 0) plus an iterable of numbers
        
        When the iterable is empty, return the start value.
        This function is intended specifically for use with numeric values and may
        reject non-numeric types.
    
    


```python
a=[1,2,3,4]
sum(a)
```




    10



# Type Conversion
# Function	Description
## ascii()	Returns a string containing a printable representation of an object
## bin()	Converts an integer to a binary string
## bool()	Converts an argument to a Boolean value
## chr()	Returns string representation of character given by integer argument
## complex()	Returns a complex number constructed from arguments
## float()	Returns a floating-point object constructed from a number or string
## hex()	Converts an integer to a hexadecimal string
## int()	Returns an integer object constructed from a number or string
## oct()	Converts an integer to an octal string
## ord()	Returns integer representation of a character
## repr()	Returns a string containing a printable representation of an object
## str()	Returns a string version of an object
## type()	Returns the type of an object or creates a new type object


```python
a = 2000
print(type(a))
b=str(a)
```

    <class 'int'>
    


```python
print(b)
type(b)
```

    2000
    




    str



# Iterables and Iterators
# Function	Description
## all()	Returns True if all elements of an iterable are true
## any()	Returns True if any elements of an iterable are true
## enumerate()	Returns a list of tuples containing indices and values from an iterable
## filter()	Filters elements from an iterable
## iter()	Returns an iterator object
## len()	Returns the length of an object
## map()	Applies a function to every item of an iterable
## next()	Retrieves the next item from an iterator
## range()	Generates a range of integer values
## reversed()	Returns a reverse iterator
## slice()	Returns a slice object
## sorted()	Returns a sorted list from an iterable
## zip()	Creates an iterator that aggregates elements from iterables


```python
help(all)
```

    Help on built-in function all in module builtins:
    
    all(iterable, /)
        Return True if bool(x) is True for all values x in the iterable.
        
        If the iterable is empty, return True.
    
    


```python
help(any)
```


```python
l = [0, False,5]
print(any(l))
```


```python
start = 2
stop = -14
step = -2

print(list(range(start, stop, step)))

# value constraint not met
print(list(range(start, 14, 2)))
```

# Composite Data Type
# Function	Description
## bytearray()	Creates and returns an object of the bytearray class
## bytes()	Creates and returns a bytes object (similar to bytearray, but immutable)
## dict()	Creates a dict object
## frozenset()	Creates a frozenset object
## list()	Creates a list object
## object()	Creates a new featureless object
## set()	Creates a set object
## tuple()	Creates a tuple object


```python
dir(52.75)
```

# Input/Output
# Function	Description
## format()	Converts a value to a formatted representation
## input()	Reads input from the console
## open()	Opens a file and returns a file object
## print()	Prints to a text stream or the console


```python
def myFun(**kwargs):  
    for key, value in kwargs.items(): 
        print ("%s == %s" %(key, value)) 
```


```python
myFun(first ='Geeks', mid ='for', last='Geeks')
```


```python
for i in range(0,10):
    myFun(i=i+1)
```

## Operators
## https://www.w3schools.com/python/python_operators.asp


```python
2+3
```




    5



## Python Placeholders


```python
txt = "For only {price:.2f} dollars!"
print(txt.format(price = 49))
```

    For only 49.00 dollars!
    

## https://www.w3schools.com/python/ref_string_format.asp


```python
a = 3.4536
print ("{0:.2f}".format(a)) 
```


```python
print ("The value of number till 2 decimal place(using %) is : ",end="") 
print ('%.2f'%a) 
```


```python
print ("The value of number till 2 decimal place(using round()) is : ",end="") 
print (round(a,2)) 
```

## Decision Making

## if


```python
var = 100
if ( var == 100 ) : print ("Value of expression is 100")
```

    Value of expression is 100
    


```python
var=200
if(var == 200):
  print("first if")
```

    first if
    

## if else


```python
var1 = 100
if var1:
   print ("1 - Got a true expression value")
   print (var1)
else:
   print ("1 - Got a false expression value")
   print (var1)
print("else will never be executed")
```

    1 - Got a true expression value
    100
    else will never be executed
    


```python
## neseted if
```


```python
if (1==2) :
    pass
```


```python
var = 100
if var == 200:
   print ("1 - Got a true expression value")
   prin(var)
elif var == 150:
    pass
elif var == 100:
   print ("3 - Got a true expression value")
   print (var)
else:
   print ("4 - Got a false expression value")
   print (var)
```

    3 - Got a true expression value
    100
    

## While


```python
var = 1
while var == 1 :  # This constructs an infinite loop
    num = input("Enter a number  :")
    print ("You entered: ", num)
    var+= 1
```

    Enter a number  : 50
    

    You entered:  50
    


```python
count = 0
while count < 5:
   print (count, " is  less than 5")
   count = count + 1
else:
   print (count, " is not less than 5")
```

    0  is  less than 5
    1  is  less than 5
    2  is  less than 5
    3  is  less than 5
    4  is  less than 5
    5  is not less than 5
    

## For with Pass and elypses


```python
for letter in 'Python':     
    print ('Current Letter :', letter)
```

    Current Letter : P
    Current Letter : y
    Current Letter : t
    Current Letter : h
    Current Letter : o
    Current Letter : n
    


```python
fruits = ['banana', 'apple',  'mango']
for fruit in fruits: 
   print ('Current fruit :', fruit)
```

    Current fruit : banana
    Current fruit : apple
    Current fruit : mango
    


```python
fruits = ['banana', 'apple',  'mango']
for fruit in fruits: 
   pass
```


```python
fruits = ['banana', 'apple',  'mango']
for fruit in fruits: 
   ...
```


```python
fruits = ['banana', 'apple',  'mango']
for index in range(len(fruits)):
    print ('Current fruit :', fruits[index])
```

    Current fruit : banana
    Current fruit : apple
    Current fruit : mango
    

## Nested for and break


```python
for num in range(10,20):     #to iterate between 10 to 20
    for i in range(2,num):    #to iterate on the factors of the number
        if num%i == 0:         #to determine the first factor
            j=num/i             #to calculate the second factor
            print ('%d equals %d * %d' % (num,i,j))
            break #to move to the next number, the #first FOR
        else:                  # else part of the loop
            print (num, 'is a prime number')
            break
```

    10 equals 2 * 5
    11 is a prime number
    12 equals 2 * 6
    13 is a prime number
    14 equals 2 * 7
    15 is a prime number
    16 equals 2 * 8
    17 is a prime number
    18 equals 2 * 9
    19 is a prime number
    

## Continue


```python
for letter in 'Python':     # First Example
    if letter == 'h':
        continue
    print ('Current Letter :', letter)
```

    Current Letter : P
    Current Letter : y
    Current Letter : t
    Current Letter : o
    Current Letter : n
    


```python
for letter in 'Python':     # First Example
    if letter == 'h':
        pass
    print ('Current Letter :', letter)
    
```


```python

```
