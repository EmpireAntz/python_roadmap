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
- [21. *args and **kwargs](#21-args-and-kwargs-)
- [22. Iterables](#22-iterables-️)
- [23. Memebership Operators](#23-memebership-operators-️)
- [24. List Comprehensions](#24-list-comprehensions-)
- [25. Match-Case Statements](#25-match-case-statements-️)
- [26. Modules](#26-modules-️)
- [27. Scope Resolution](#27-scope-resolution-️)
- [28. if __name__ =="__main__"](#28-if-name--main-️)
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
- [48. PyQt5](#48-pyqt5)



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

```python
number_1 = "1"
number_2 = "2"
print(int(number_1))
print(int(number_2))
print(str(number_1))
print(str(number_2))
```

#### Output:

```
1
2
1
2
```
## 3. User Input ✔️

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

## 6. Logical Operators

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

## 14. Lists, Sets, and Tuples ✔️

## 15. 2D Collections ✔️

## 16. Dictionaries ✔️

## 17. Random Numbers ✔️

```python
import random

class Gun :
    def __init__(self, name, tier, damage, accuracy):
        self.name = name
        self.tier = tier
        self.damage = damage
        self.accuracy = accuracy

def rand_tier():
    rng = random.uniform(1,100)
    if rng <= 60:
        tier = "Tier 1 ⬜"
    elif rng > 60 and rng <= 90:
        tier = "Tier 2 🟩"
    elif rng >= 90 and rng <= 99.8:
        tier = "Tier 3 🟪"
    else :
        tier = "Tier 4 🟨"
    return tier


def rand_damage(tier):
    if tier == "Tier 1 ⬜":
        dmg = random.randint(50, 75)
    elif tier == "Tier 2 🟩":
        dmg = random.randint(60, 85)
    elif tier == "Tier 3 🟪":
        dmg = random.randint(75, 100)
    elif tier == "Tier 4 🟨":
        dmg = random.randint(90, 115)
    return dmg


def rand_name(tier):
    if tier == "Tier 1 ⬜":
        prefix = ("Luxurious", "Big", "Strange", "Lucky", "Garbled",
                  "Melted", "Singin'", "Spittin'", "Hardy", "Shining")
        suffix = ("Rattler", "Chungus", "Smidge", "Trickler", "Bronson",
              "Revolt", "Lux", "Repo", "Sidekick", "Stranger")
    elif tier == "Tier 2 🟩":
        prefix = ("Majestic", "Grand", "Equalized", "Enlarged", "Anticipated",
                  "Solid", "Swarmin'", "Heavy", "Handy", "Blazin'")
        suffix = ("Zinger", "Hunger", "Randall", "Blaster", "Boom-Stick",
              "Mulcher", "Mako", "Tsunami", "Alien", "Chunker")
    elif tier == "Tier 3 🟪":
        prefix = ("Marvelous", "Splendid", "Surreal", "Benevolent", "Mighty",
                  "Atrocious", "Nocturnal", "Enamored", "Rock-Solid", "Hardcore")
        suffix = ("Rattle-Snake", "Honeybee", "Queen", "Dragon", "Jackyl",
              "Bane", "Keepsake", "Charlie", "Merry-Go-Round", "Trickster")    
    elif tier == "Tier 4 🟨":
        prefix = ("Glamorous", "Impeccable", "Gleaming", "Grandiose", "Enduring",
                  "Slick", "Impervious", "Inevitable", "Heavy-Metal", "Gorgeous")
        suffix = ("Brimstone", "Ruby", "Dagger", "Ocean", "Circus",
                  "Fairy-Tale", "Skullcracker", "Harold", "Waverider", "Baron")
    rng_suf = random.choice(suffix)
    rng_pref = random.choice(prefix)
    full_name = f"{rng_pref} {rng_suf}"
    return full_name


def rand_accuracy(tier):
    if tier == "Tier 1 ⬜":
        acc = random.randint(60, 75)
    elif tier == "Tier 2 🟩":
        acc = random.randint(70, 85)
    elif tier == "Tier 3 🟪":
        acc = random.randint(80, 100)
    elif tier == "Tier 4 🟨":
        acc = random.randint(90, 100)
    return acc


def add_gun():
    rolled_tier = rand_tier()
    rolled_damage = rand_damage(rolled_tier)
    rolled_accuracy = rand_accuracy(rolled_tier)
    rolled_name = rand_name(rolled_tier)
    rolled_gun = Gun(rolled_name, rolled_tier, rolled_damage, rolled_accuracy)
    return rolled_gun

list_of_guns = []

for i in range(10):
    rolled_gun = add_gun()
    list_of_guns.append(rolled_gun)

for gun in list_of_guns:
    print(f"----{gun.name}----")
    print(f"{gun.tier}\nDamage: {gun.damage}\nAccuracy: {gun.accuracy}%")
    print("-----------------")

```
#### Output:

```
----Handy Chunker----
Tier 2 🟩
Damage: 71
Accuracy: 75%
-----------------
----Shining Chungus----
Tier 1 ⬜
Damage: 54
Accuracy: 69%
-----------------
----Mighty Charlie----
Tier 3 🟪
Damage: 89
Accuracy: 85%
-----------------
----Singin' Chungus----
Tier 1 ⬜
Damage: 57
Accuracy: 63%
-----------------
----Luxurious Chungus----
Tier 1 ⬜
Damage: 51
Accuracy: 71%
-----------------
----Luxurious Sidekick----
Tier 1 ⬜
Damage: 71
Accuracy: 70%
-----------------
----Handy Chunker----
Tier 2 🟩
Damage: 72
Accuracy: 81%
-----------------
----Singin' Revolt----
Tier 1 ⬜
Damage: 69
Accuracy: 67%
-----------------
----Blazin' Alien----
Tier 2 🟩
Damage: 60
Accuracy: 71%
-----------------
----Spittin' Lux----
Tier 1 ⬜
Damage: 71
Accuracy: 66%
-----------------
```
## 18. Functions ✔️

## 19. Default Arguments 🟥

## 20. Keyword Arguments 🟥

## 21. \*args and \*\*kwargs 🟥

## 22. Iterables ✔️

## 23. Memebership Operators ✔️

## 24. List Comprehensions 🟥

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

## 48. PyQt5
