---
tags: [prerequisite, coding, programming, logic]
aliases: [Coding Concepts, Programming Fundamentals]
difficulty: 2
---

# Basic Coding Concepts

## What is Code?
Code is simply a set of instructions for the computer to follow. Just like a recipe tells you how to cook, code tells the computer what to do. All programming languages share these core concepts.

## 1. Variables
A variable is a container that stores data. You give it a name and put a value inside.

```text
user_age = 25
user_name = "Alice"
is_logged_in = true
```
- `user_age` holds the number 25.
- `user_name` holds the text "Alice".
- `is_logged_in` holds a yes/no value (boolean).

## 2. Data Types
Computers need to know what kind of data they are handling.
- **Integer**: Whole numbers (1, 42, -5).
- **String**: Text ("Hello", "Password123").
- **Boolean**: True or False.
- **Float**: Decimal numbers (3.14, 0.01).

## 3. Conditionals (If/Else)
Making decisions based on data.

```text
IF user_age >= 18 THEN
    PRINT "You are an adult."
ELSE
    PRINT "You are a minor."
END IF
```

## 4. Loops
Repeating actions without writing the same code twice.

### For Loop (Repeat X times)
```text
FOR i FROM 1 TO 5:
    PRINT "Hello"
```
*Output: Hello Hello Hello Hello Hello*

### While Loop (Repeat while condition is true)
```text
WHILE battery_level > 0:
    KEEP_RUNNING
```

## 5. Functions
A reusable block of code. Instead of writing the same steps 10 times, you write them once in a function and call the function.

```text
FUNCTION greet(name):
    PRINT "Hello, " + name

greet("Alice")
greet("Bob")
```
*Output: Hello, Alice / Hello, Bob*

## 6. Arrays (Lists)
Storing multiple items in one variable.

```text
fruits = ["Apple", "Banana", "Cherry"]
```
- `fruits[0]` is "Apple".
- `fruits[1]` is "Banana".

## Micro-Challenge
You do not need to install anything yet. Just understand the logic.
1. Write down a "recipe" for making coffee using variables and steps.
2. Identify where you would use an "If/Else" (e.g., IF sugar_requested THEN add_sugar).
3. Identify where you would use a loop (e.g., WHILE cup_not_full POUR_coffee).

> [!TIP] Language Agnostic
> These concepts exist in Python, JavaScript, Java, C++, and almost every other language. Once you learn them once, you just learn the new syntax.
