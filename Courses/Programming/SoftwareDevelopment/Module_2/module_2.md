# Module 2
This is the continuation of the first module! That's an obvious statement, but we're going to expand a little on some of the things that were introduced and make a little bit more sense about how you write actual programs instead of just basic statements.

---

## Lists in Python!
We introduced Lists back in Module 1, but we truly need to emphasize the importance of them. As a quick refresher, Lists are one of the ways of representing a collection of items in Python. They're often referred to as Arrays in other languages, but we'll walk through why they're so vital to programming.

### Examples of Lists
```Python
# A list as a collection of items for a grocery run
grocery_list = ["Apples", "Bananas", "Oatmeal", "Eggs", "Bread"]

# A list of integers that represent ages of friends
friend_ages = [18, 19, 21, 20, 22]

# They can also be a mix of data types, like ints and strings
mixed_example = [100, "Apples", "Bananas", 298374, "mixed"]
```

These are just some basic examples of lists, but we'll touch on some of the more complex stuff after introducing functions

---

## Functions
Functions are nothing more than blocks of code to better organization, reading, and performance. If you have a script that's over 100 lines of code, imagine how difficult that would be to read if you can't just quickly glance at an appropriately named function and quickly recognize what is does.

### Examples
```Python
# Creating your OWN function
def your_first_function():
	# Print out the message
	# This is 'inside the function'
	print("This is the first function I wrote!")
	
print("This is outside the function")
	
# In order to 'execute', you have to first call the function.
your_first_function()

'''
The anatomy of a function:
	1. 'def': How you declare the following code will be a function
	2. Indentation: Python is very specific on the spacing, so all code within that indent is what's contained within the function. 
'''
```

