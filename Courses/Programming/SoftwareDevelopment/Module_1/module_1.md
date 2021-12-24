# Module 1: The Introduction
This is going to be all about demistifying what programming is, why everyone wants to do it so badly, and why the hell devs make so much money at some companies (it's hard... but manageable!!!)
___

## Programming
[Wikipedia](https://en.wikipedia.org/wiki/Computer_programming) defines programming as: designing and building an executable computer program to accomplish a specific result or to perform a particular task.

According to Charles Isbell, the Dean of the College at Computing for Georgia Institute of Technology, programming can be broken down into three things:
1. Writing to a variable
2. Reading from a variable
3. Conditional branching

".... and everything else is syntactic sugar."  

A variable is a method of storing values within a program and you have to write to a variable in order for it to be initialized and the computer to know where to point to whenever it is referenced. Below is an example of the three things he was talking about.

```Python
# Writing to a variable
x = 10
y = 5

# Reading from a variable(s) in order to do some addition
z = x + y

# Print out the result of the addition
print(z) # Hint: it's 15

# Example of conditional branching
if z > 20:
	print("It's greater than 20!")
else:
	print("The value is not greater than 20.")

```

Conditional branching is the concept that within your code that instructs the computer that is running your code to do something differently if that result is met. Examples of results can be comparing two numbers, if two variables are equal to eachother, etc.
---

## Why Python

---

## Variables and Storing Data
Most people know variables from basic algebra, where 'x' is associated with an integer, but in programming, your scope and perspective has to change a little bit. Think of a variable as a way of storing a value, but that value can be of several different data types. 

Data Types (Just some, when we get to Java, we'll expand a little more):
1. Integer (Ex: 5 or 7)
	1. A whole number representation of a value
2. String (Ex: "Programming" or "GitHub")
	1. String of characters enclosed by Quotations (or single quotes in Python)
3. Float (Ex: 3.76 or 4.20)
	1. Value that can contain 
4. List (also an Array.... Ex: [1, 2, 3, 4] or ["haha", "joke", "was", "funny"])
5. Boolean (Ex: True or False)

More examples and further explanation [Here](https://www.w3schools.com/python/python_datatypes.asp).

---

## What do these look like in Python?

```Python
# This is a comment
```

