**Instructions:**

1. Fork this repository to your own Github account.
2. Clone the forked repository to your local machine.
3. After completing each exercise: git add, git commit and git push to your forked repository.

# Table of Contents

1. [Variables](#variables)
2. [Data Types](#data-types)
3. [Basic Operators](#basic-operators)
4. [Indentation](#indentation)

## Variables

**What are Variables?**

- Variables are named containers used for storing data in a program.
- They provide a way to label and reference data in memory.
- Variables can hold various types of data, including numbers(int), text(str), and more.
- Variables behave according to the rules of the data type they contain.
- The process of creating a variable is known as variable declaration.
- Variables should have a unique name within their scope.
- A variable's name typically follows specific naming conventions (e.g., no spaces, starts with a letter or underscore).
- The data stored in a variable can be changed, making them essential for working with dynamic data.

```python
# name in this case is the variable, and it stores the value "Zakumi"

name = "Zakumi"
```

 This is similar to how you used to solve for x in high school, :smile:, remember this?

 ```python
 let z = 1

 let y = 2

Solve for x if  z = 1, y = 2:

            x + y + z = 0

            x + (2) + (1) = 0

            x + 3 = 0

            x = -3 
 ```

 You can go ahead and print the name variable and see what you get :smile:

 ```python
 # The function 'print' is an in-built function in python. 
 print(name)
 ```

 You can start familiarising yourself with python documentation to see what other in-built function are there.

 https://docs.python.org/3/

https://realpython.com/documenting-python-code/

**Instructions:**

1. Use Python variables to store values of different types (integers, floats, strings, booleans).
2. Display messages using the print statement based on the variable values.

## Data Types

**What are data types?**

Data types are used to categorize and manage different types of data. In python you don't need to declare the data type of a variable explicitly.

Python has built-in data types. Here are some of the fundamental data types in Python:

```python
#Integer:
            int
#This represents whole numbers
#Example: 

num1 = 1

num2 = 20

num3 = -222
```

```python
#Floating-Point:
            float
#This represents numbers with decimals
#Example: 

num1 = 3.14

num2 = 2.0 

num3 = -0.23
```

```python
#String
            str
# This represents sequences of characters 
#Example: 

mascot = "Zakumi" 

wifi_password = "W3Th1nkC0dE"

greeting = "Hello world!"
```

```python
#Boolean
            bool
#This binary data with two values
#Examples:
            True

x = 1 

y = 1

#Question is, is x the same/equal to y? See what you get when you run the line below.

print(x=y)
            False
x = 1 

y = 3.14

#Question is, is x the same/equal to y? See what you get when you run the line below.

print(x=y)
```

```python
#List
                list
#This represents an ordered collection of elements
#Elements can be of different data types.
#Example: 
number_list = [1, 2, 3] 

fruit_list =  ['apple', 'banana', 'cherry']
```

```python
#Tuple
                tuple
#Similar to a list, but immutable (cannot be changed after creation).
#Example:

number_tuple = (1,2,3)

colour_tuple = ("red","green","blue")
```

```python
#Dictionary
                dict
#Represents key-value pairs.
#Keys are unique and used to access values.
#Example:

personal_details = {'name': 'Zakumi','age':30}
```     


```python
#Sets
                set
#Represents an unordered collection of unique elements.
#Useful for mathematical set operations.
#Example:

number_set = {1,2,3,4}

fruit_set = {'apple','banana','cherry'}
```

```python
#Nonetype
                None
#Represents the absence of a value
```

**Instructions:**

Let's attempt solving exercised inside the file `basic_syntax_exercise.py`

1. Explore Python's built-in data types.
2. Use the `type()` function to identify the data types of variables.

## Basic Operators
**What are Operators?**

Operators are a symbol or combination of symbols that allows you to perform a specific operation/process.

Let's explore the different kinds of operations:

*1. Arithmetic Operators:*

```python
                    #Addition(+)
#Adds numbers together
#Run the following to see what you get

x = 1 + 3 

print(x)
```


```python
                    #Subtraction(-)
#Subtract numbers together
#Run the following to see what you get

x = 5 - 3 

print(x)
```


```python
                    #Multiplication(*)
#Multiplies numbers together
#Run the following to see what you get

x = 5*3 

print(x)
```


```python
                    #Division(+)
#Divides the left operand by the right operand
#Run the following to see what you get

x = 100/3 

print(x)
```


```python
                    #Modulus(%)
#Returns the remainder of the division
#Run the following to see what you get

x = 10
y = 3

remainder = x % y

print(f"The remainder of {x} divided by {y} is {remainder}")
```

```python
                    #Exponentials(**)
#Raises the left operand to the power of the right operand
#The below means x raised to the power y  
#Run the following to see what you get

x = 5

y = 2

print(x**y)
```

*2. Comparison Operators*

```python
                    #Equal(==)
#Checks if two values are equal
#Run the following to see what you get
---------------------------------
x = 123

y = 123

print(x==y) #Should return True

---------------------------------

x = 123

y = '123'

print(x==y) #Should return False. We'll leave it to you to figure why :)
```

```python
                    #Not Equal(!=)
#Checks if two values are not equal
#Run the following to see what you get
---------------------------------
x = 'abc'

y = "ABC"

print(x!=y) #Should return True

---------------------------------

x = "WeThinkCode_"

y = 'WeThinkCode_'

print(x!=y) #Should return False. We'll leave it to you to figure why :)
```

```python
                    #Greater than(>)
#Checks if the left operand is greater than the right operand
#Run the following to see what you get
---------------------------------
x = 122

y = 123

print(x > y) #Should return False

---------------------------------

x = 123

y = 12

print(x > y) #Should return True. 
```     


```python
                    #Less than(<)
#Checks if the left operand is less than the right operand
#Run the following to see what you get
---------------------------------
x = 122

y = 123

print(x < y) #Should return True

---------------------------------

x = 123

y = 12

print(x < y) #Should return False. 
```     

```python
                    #Greater than or equal to(>=)
#Checks if the left operand is greater than or equal to the right operand.
#Run the following to see what you get
x = 5
y = 3

result1 = x >= y  # Is x greater than or equal to y?
result2 = y >= x  # Is y greater than or equal to x?

print(f"{x} >= {y} is {result1}")
print(f"{y} >= {x} is {result2}") 
``` 

```python
                    #Less than or equal to(<=)
#Checks if the left operand is less than or equal to the right operand.
#Run the following to see what you get
a = 10
b = 15

result1 = a <= b  # Is a less than or equal to b?
result2 = b <= a  # Is b less than or equal to a?

print(f"{a} <= {b} is {result1}")
print(f"{b} <= {a} is {result2}")
``` 


*3. Assignment Operators*

```python
                    #Assignment(=)
#Assigns a value to a variable

name = 'Zakumi'
```


```python
                    #Addition Assignment(+=)
#Adds the right operand to the left operand and assigns the result to the left operand
#Run the following to see what you get

------------------------------------------------
#How you'd normally write it:
x = 1

x = x + 5

print(x)

------------------------------------------------
#Using the addition assignement operator (equivalent to the above)

x = 1

x += 5

print(x)
 
```

```python
                    #Subtraction Assignment(-=)
#Subtracts the right operand from the left operand and assigns the result to the left operand
#Run the following to see what you get

------------------------------------------------
#How you'd normally write it:
x = 100

x = x - 35

print(x)

------------------------------------------------
#Using the subtraction assignement operator (equivalent to the above)

x = 100

x -= 35

print(x)
 ```

```python
                    #Multiplication Assignment(*=)
#Multiplies the left operand by the right operand and assigns the result to the left operand
#Run the following to see what you get

------------------------------------------------
#How you'd normally write it:
x = 2

x = x * 35

print(x)

------------------------------------------------
#Using the subtraction assignement operator (equivalent to the above)

x = 2

x *= 35

print(x)
 ```


```python
                    #Division Assignment(/=)
#MDivides the left operand by the right operand and assigns the result to the left operand
#Run the following to see what you get

------------------------------------------------
#How you'd normally write it: 

x = 7

x = x / 3.5

print(x)

------------------------------------------------
#Using the subtraction assignement operator (equivalent to the above)

x = 7

x /= 35

print(x)
 ```


*4. Logical Operators*

```python
#and logical operator
                        and
#Compares two operations and Returns True if both operands are True
#Run the following two see what you get

# Example 1: Logical AND with two True values
a = True
b = True

result1 = a and b

# Example 2: Logical AND with one True and one False value
x = True
y = False

result2 = x and y

print(f"Result 1: {result1}")
print(f"Result 2: {result2}")
``` 
 
 
```python
#or logical operator
                        or
#Returns True if AT LEAST ONE operand of the is True.
#Run the following two see what you get

# Example 1: Logical OR with two True values
m = True
n = True

result1 = m or n

# Example 2: Logical OR with one True and one False value
p = True
q = False

result2 = p or q

print(f"Result 1: {result1}")
print(f"Result 2: {result2}")
``` 


```python
#not logical operator
                        not
#Returns the opposite of the operand's value
#Run the following two see what you get

# Example 1: Logical NOT with a True value
value = True

result1 = not value

# Example 2: Logical NOT with a False value
status = False

result2 = not status

print(f"Result 1: {result1}")
print(f"Result 2: {result2}")
``` 
 
**Instructions:**

1. Practice using various arithmetic operators for addition, subtraction, multiplication, division, and modulus (remainder).

## Indentation

*What is indentation?*

Indentation is a fundamental part of the language's syntax and is used to define blocks of code. Proper indentation is crucial for the readability and correctness of Python programs

Indentation is used to define blocks of code within functions, loops, conditionals, and other control structures. Here's an example of a conditional statement:
```python
if condition:
    # This code is indented and part of the if block.
    do_something()
else:
    # This code is part of the else block.
    do_something_else()
```

Examples of loops:
```python
for condition:
    # This code is indented and part of the for loop.
    do_something()

    
while condition:
    # This code is part of the while loop.
    do_something_else()
```

**Instructions:**

1. Learn about the importance of indentation in Python.
2. You will complete a for loop to print numbers from 0 to 5.

By following this order, you will build a solid foundation in Python basic syntax. 
Make sure to commit your changes and push them to your forked repository after completing each exercise. Good luck!
