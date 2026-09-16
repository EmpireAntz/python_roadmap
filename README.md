# Python Roadmap

## Table of Contents

- [1. Variables](#1-variables-️)
- [2. Type Casting](#2-type-casting-️)
- [3. User Input](#3-user-input-️)
- [4. Math and Arithmetic](#4-math-and-arithmetic-️)
- [5. If Statements](#5-if-statements-️)
- [6. Logical Operators](#6-logical-operators)
- [7. Conditional Expressions](#7-conditional-expressions-️)
- [8. String Methods](#8-string-methods-️)
- [9. String Indexing](#9-string-indexing-️)
- [10. Format Specifiers](#10-format-specifiers-️)
- [11. While Loops](#11-while-loops-️)
- [12. For Loops](#12-for-loops-️)
- [13. Nested Loops](#13-nested-loops-️)
- [14. Lists Sets and Tuples](#14-lists-sets-and-tuples-️)
- [15. 2D collections](#15-2d-collections-️)
- [16. Dictionaries](#16-dictionaries-️)
- [17. Random Numbers](#17-random-numbers-️)
- [18. Functions](#18-functions-️)
- [19. Default Arguments](#19-default-arguments-)
- [20. Keyword Arguments](#20-keyword-arguments-)
- [21. \*args and \*\*kwargs](#21-args-and-kwargs-)
- [22. Iterables](#22-iterables-️)
- [23. Memebership Operators](#23-memebership-operators-️)
- [24. List Comprehensions](#24-list-comprehensions-)
- [25. Match-Case Statements](#25-match-case-statements-️)
- [26. Modules](#26-modules-️)
- [27. Scope Resolution](#27-scope-resolution-️)
- [28. if **name** =="**main**"](#28-if-name--main-️)
- [29. Python Object Oriented Programming](#29-python-object-oriented-programming-️)
- [30. Class Variables](#30-class-variables-️)
- [31. Inheritance](#31-inheritance-️)
- [32. Multiple Inheritance](#32-multiple-inheritance-️)
- [33. super()](#33-super-️)
- [34. Polymorphism](#34-polymorphism-)
- [35. "Duck" Typing](#35-duck-typing-)
- [36. Static Methods](#36-static-methods-)
- [37. Class Methods](#37-class-methods-)
- [38. Magic Methods](#38-magic-methods-)
- [39. @Property](#39-property-)
- [40. Decorators](#40-decorators-)
- [41. Exception Handling](#41-exception-handling)
- [42. File Detection](#42-file-detection)
- [43. Writing Files](#43-writing-files)
- [44. Reading Files](#44-reading-files)
- [45. Dates & Times](#45-dates--times)
- [46. Multithreading](#46-multithreading)
- [47. Request API Data](#47-request-api-data)
- [48. Virtual Environments (venv)](#48-virtual-envirnoments-venv)
- [49. PyQt5](#48-pyqt5)

## 1. Variables ✔️

Variables are how values are stored, think of it as a container that holds something. In this example, animal_1 is the variable and "cat" is the value stored in that variable while the variable animal_2 stores the value of "dog".
We put text values in quotes to identify them as a string(more on that next chapter).

```python
animal_1 = "cat"
animal_2 = "dog"
print(animal_1)
print(animal_2)
```

We use the print() function to print things to the terminal window. In this case we want to print our animal_1 and animal_2 to see the values they are holding. We pass in the values we want to print between the (). When we run the program we will see this as the output in the terminal.

#### Output:

```
cat
dog
```

## 2. Type Casting ✔️

There are several different data types we can work with in python. Some of the most commonly used are strings, integers, floating point numbers and booleans.

### Strings:

Text values are what we call 'strings' and can be stored in double or single quotes

```python
number_1 = "1"
```

### Ints and Floats:

Number values can be whole numbers ('Integers' or 'int'), or Decimals ('Floating point' or 'float')

```python
number_1 = 1
number_2 = 2.1
```

### Bools:

There are also 'boolean' values or 'bool' which are a true or false statement

```python
working_hard = True
hardly_working = False
```

We can cast values to become another value type with type casting.

```python
int()
float()
str()
```

By casting the values as a differnt type, we can do things like change numbers to strings or strings to numbers

```python
number_1 = "1"
number_2 = "2"
print(int(number_1)) #will convert to whole number as 'int' for integer
print(int(number_2))
print(float(number_1)) #will convert to floating point number as 'float'
print(float(number_2))
print(str(number_1)) #will convert to text value as 'str' for string
print(str(number_2))
```

note that while the 1 and 2 printed first look the same as the 1 and 2 printed at the end but the difference is the first are of type 'int' while the last are of type 'str' and strings cannot be inerpreted as numbers

#### Output:

```
1
2
1.0
2.0
1
2
```

We will see in this example that not everything is treated equally when type casting

```python
animal_1 = "cat"
animal_2 = "dog"
print(int(animal_1))
print(int(animal_2))
print(float(animal_2))
print(float(animal_2))
print(str(animal_1))
print(str(animal_2))
```

#### Output:

```
Traceback (most recent call last):
  File "c:\Users\Owner\dev\python\python_roadmap\test.py", line 3, in <module>
    print(int(animal_1))
          ~~~^^^^^^^^^^
ValueError: invalid literal for int() with base 10: 'cat'
```

here we will see that the string cannot be converted to an integer because cat is not a number, whereas in the previous example, even tho we had a string of "1" we still are able to cast it as an integer because 1 is a castable number.

## 3. User Input ✔️

```python
user_name = input("What is your name?: ")
print(f"Hello {user_name}!")
```

#### Output:

![alt text](/img/image.png)

![alt text](/img/image-1.png)

![alt text](/img/image-2.png)

## 4. Math and Arithmetic ✔️

```python
number_1 = 1
number_2 = 2
print(number_1 + number_2)
print(number_1 - number_2)
print(number_1 * number_2)
print(number_1 / number_2)
print(number_1 % number_2)
```

#### Output:

```
3
-1
2
0.5
1
```

## 5. If Statements ✔️

```python
number_1 = 1
number_2 = 2
if number_1 == 1 :
    print("This is number 1")
```

#### Output:

```
This is number 1
```

## 6. Logical Operators ✔️

```python
number_1 = 1
number_2 = -1
if number_1 > 0 :
    print("This Number is Greater than 0")
if number_2 < 0 :
    print("This Number is Less than 0")
if number_1 < 10:
    print("This number is less than 10")
if number_2 >= 1:
    print("This number is greater than or equal to 1")
```

#### Output:

```
This Number is Greater than 0
This Number is Less than 0
This number is less than 10
```

## 7. Conditional Expressions ✔️

```python
number_1 = 1
number_2 = 2
if number_1 == 1 and number_2 == 2:
    print("All numbers are correct")
elif not number_1 == 1 or not number_2 == 2:
    print("Somethings not right here")
```

#### Output:

```
All numbers are correct
```

## 8. String Methods ✔️

```python
animal_1 = "cat"
animal_2 = "dog"
print(animal_1.upper())
print(animal_2.upper())
print(animal_1.lower())
print(animal_2.lower())
print(animal_1.capitalize())
print(animal_2.capitalize())
```

#### Output:

```
CAT
DOG
cat
dog
Cat
Dog
```

## 9. String Indexing ✔️

```python
animal_1 = "cat"
animal_2 = "dog"
print(animal_1[0])
print(animal_1[1])
print(animal_1[2])
print(animal_2[0])
print(animal_2[1])
print(animal_2[2])
```

#### Output:

```
c
a
t
d
o
g
```

## 10. Format Specifiers ✔️

```python
item_1 = "milk"
item_2 = "eggs"
item_1_price = 5
item_2_price = 7.6

print(f"The first item is {item_1} and it costs ${item_1_price:.2f}")
print(f"The second item is {item_2} and it costs ${item_2_price:.2f}")
```

#### Output:

```
The first item is milk and it costs $5.00
The second item is eggs and it costs $7.60
```

## 11. While Loops ✔️

```python
import time

game_running = True
countdown = 3

while game_running:
    print(f"Continue? {countdown}")
    time.sleep(1)
    countdown -= 1
    print(f"Continue? {countdown}")
    time.sleep(1)
    countdown -= 1
    print(f"Continue? {countdown}")
    time.sleep(1)
    countdown -= 1
    print(f"Continue? {countdown}")
    time.sleep(1)
    if countdown <= 0:
        print("GAME OVER")
        game_running = False
        break
```

#### Output:

```
Continue? 3
Continue? 2
Continue? 1
Continue? 0
GAME OVER
```

## 12. For Loops ✔️

```python
for i in range(5):
    print("hello")
```

#### Output:

```
hello
hello
hello
hello
hello
```

## 13. Nested Loops ✔️

```python
suits = ("♥️","♦️","♣️","♠️")
ranks = ("2", "3", "4", "5", "6", "7", "8", "9", "10", "J", "Q", "K", "A")
for rank in ranks:
    for suit in  suits:
        print(f"{rank}{suit}", end = " ")
```

#### Output:

```
2♥️ 2♦️ 2♣️ 2♠️ 3♥️ 3♦️ 3♣️ 3♠️ 4♥️ 4♦️ 4♣️ 4♠️ 5♥️ 5♦️ 5♣️ 5♠️ 6♥️ 6♦️ 6♣️ 6♠️ 7♥️ 7♦️ 7♣️ 7♠️ 8♥️ 8♦️ 8♣️ 8♠️ 9♥️ 9♦️ 9♣️ 9♠️ 10♥️ 10♦️ 10♣️ 10♠️ J♥️ J♦️ J♣️ J♠️ Q♥️ Q♦️ Q♣️ Q♠️ K♥️ K♦️ K♣️ K♠️ A♥️ A♦️ A♣️ A♠️
```

## 14. Lists, Sets, and Tuples ✔️

```python
my_list = []
my_set = {}
my_tuple = ()
```

## 15. 2D Collections ✔️

## 16. Dictionaries ✔️

## 17. Random Numbers ✔️
Pythons random module has several useful methods for creating "psuedo-randomness." These are some of the most useful ones.

```python
random.choice(sequence) # returns a random element from a sequence
random.shuffle(sequence) # returns a shuffled sequence from a given sequence
random.randint(a, b) # returns an integer between a specified range where both ints are inclusive
random.randrange(start, stop, step) # returns integer between start and stop where stop is exclusive and can be stepped
random.random() # returns a random number between 1 and 0 and does not take an argument
random.uniform(a, b) # returns a random float between 2 numbers where both are inclusive
random.sample(sequence, k) # returns a list with a specified number of random items from a sequence where k = number of items returned
```
Here is an example of something fun you can do with ranomness. Here were just randomizing a float between 1 and 100 and creating a percentage chance for each tier. 
```python
import random
t1 = 0
t2 = 0
t3 = 0
t4 = 0
for i in range(10):
    rng = random.uniform(1, 100)
    if rng <= 60:
        tier = "Tier 1 ⬜ | 60% Chance"
        t1 += 1
    elif rng > 60 and rng <= 90:
        tier = "Tier 2 🟩 | 30% Chance"
        t2 += 1
    elif rng >= 90 and rng <= 99.8:
        tier = "Tier 3 🟪 | 9.8% Chance"
        t3 += 1
    else:
        tier = "Tier 4 🟨 | 0.2% Chance"
        t4 += 1
    print(tier)
print("===FINAL COUNT===")
print(f"Tier 1 ⬜ : {t1}")
print(f"Tier 2 🟩 : {t2}")
print(f"Tier 3 🟪 : {t3}")
print(f"Tier 4 🟨 : {t4}")
```

#### Output:

```
Tier 3 🟪 | 9.8% Chance
Tier 1 ⬜ | 60% Chance
Tier 1 ⬜ | 60% Chance
Tier 2 🟩 | 30% Chance
Tier 2 🟩 | 30% Chance
Tier 1 ⬜ | 60% Chance
Tier 1 ⬜ | 60% Chance
Tier 1 ⬜ | 60% Chance
Tier 1 ⬜ | 60% Chance
Tier 1 ⬜ | 60% Chance
===FINAL COUNT===
Tier 1 ⬜ : 7
Tier 2 🟩 : 2
Tier 3 🟪 : 1
Tier 4 🟨 : 0
```
if you run this several times you wil get a different outcome everytime and a very low chance at getting a tier 4 but eventually if you run it enough you will get a tier 4. You could also cheese it and just put like 1000 in the for loop range and see how many you get. (I ran this 1000 times and this was the outcome)

```
===FINAL COUNT===
Tier 1 ⬜ : 602
Tier 2 🟩 : 293
Tier 3 🟪 : 102
Tier 4 🟨 : 3
```

## 18. Functions ✔️
```python
def do_this():
    print("doing this")

def do_that():
    print("doing that")

do_this()
do_that()
```

#### Output:

```
doing this
doing that
```

```python
def do_this(task):
    print(f"doing this {task}")

def do_that(task):
    print(f"doing that {task}")

do_this("sweeping")
do_that("laundry")
```

#### Output:

```
doing this sweeping
doing that laundry
```

## 19. Default Arguments 🟥

## 20. Keyword Arguments 🟥

## 21. \*args and \*\*kwargs 🟥

## 22. Iterables ✔️

## 23. Memebership Operators ✔️

## 24. List Comprehensions ✔️

## 25. match-case Statements ✔️

## 26. Modules ✔️

## 27. Scope Resolution ✔️

## 28. if **name** == '**main**' ✔️

## 29. Python Object Oriented Programming ✔️

## 30. Class Variables ✔️

## 31. Inheritance ✔️

## 32. Multiple Inheritance ✔️

## 33. super() ✔️

## 34. Polymorphism 🟥

## 35. Duck Typing 🟥

## 36. Static Methods 🟥

## 37. Class Methods 🟥

## 38. Magic Methods 🟥

## 39. @property 🟥

## 40. Decorators 🟥

## 41. Exception Handling

## 42. File Detection

## 43. Writing Files

## 44. Reading Files

## 45. Dates & Times

## 46. Multithreading

## 47. Request API data

## 48. Virtual Envirnoments (venv)

To create Virtual Environment for Windows
```
python -m venv env
```
To active the Virtual Environment
```
env/Scripts/activate
```
To create a requirements.txt file
```
pip freeze > requirements.txt
```
To install requirements from requirments.txt file
```
pip install -r requirements.txt
```

## 49. PyQt5
