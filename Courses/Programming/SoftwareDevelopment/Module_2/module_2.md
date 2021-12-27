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

The anatomy of a function:
1. 'def': How you declare the following code will be a function
2. Parentheses: Things contained within the parameters of the function are what the function requires as inputs. If there's nothing between them, then the function doesn't require any parameters.
3. Indentation: Python is very specific on the spacing, so all code within that indent is what's contained within the function. Anything within the function will be within an indentation just after the line that the function is defined. I put in an example of what isn't contained within an example below. 
4. Return: The return statement is a little tricky for some to understand, but I promise whenever you go to actually write the code you want, it'll click. I'll also attach ample examples below

Keep in mind that functions have to be called in order to actually do anything. Below you'll see me create a function, 'your_first_function', and then call the function in order to execute the code contained within in

### Examples

**Calling a function and the basic anatomy**
```Python
'''
def: Telling Python this is the start of a function
your_first_function: The name of the function
(): The function takes in no parameters
(no) return: The function doesn't return anything
'''

def your_first_function():
	# Print out the message
	# This is 'inside the function'
	print("This is the first function I wrote!")

# Like I said, this is outside of the function 'your_first_function'
print("This is outside the function")
	
# In order to 'execute', you have to first call the function.
your_first_function()
```

**Creating a function with parameters and a return statement to do some calculations**
```Python
# Create two integers for parameters
x = 5 # If you want two vars as the same value you can also do x, y = 5
y = 10

# Create the function, 'add_two_variables'
def add_two_variables(x, y):
	# Add the x and y paramaters and set it to 'z'
	z = x + y
	# Return the value of the operation
	return z

# Set a variable result as the result of calling the function with the params
result = add_two_variables(5, 10)

# Print out the result
print(result)
```

Don't worry, there will be tons of practice in the 'Assignment' that's in the module!

Here's a couple great videos for supplementary materials:
1. [Former Google Engineer teaches functions](https://www.youtube.com/watch?v=NSbOtYzIQI0&t=2s)
2. [Great Overall Tutorial on Functions](https://www.youtube.com/watch?v=9Os0o3wzS_I&t=498s)

---

## Variable Scope
**Scope** for a variable is the concept of where variables exist within the project itself. Without getting far too technical below are a couple examples with code comments that make sure to highlight exactly what I'm talking about.

```Python
# These three GLOBAL variables can be used by ALL functions.
my_name = "Kyle"
my_school = "UPenn"
my_age = 22

# We define a function and create some variables within the function itself
def global_or_local_example(my_name, my_school, my_age):
	# Create a LOCAL variable for age
	next_year_age = my_age + 1
	# Print out a message
	print(my_name + "goes to" + my_school + "and next year, I'll be"
		  + next_year_age)

# Call the function with the three global variables
global_or_local_example(my_name, my_school, my_age)

'''
If you wanted to take name, school, and age and manipulate them further in other functions, you could. This is because they are global variables. It becomes different whenever you want to take 'next_year_age' out of the scope of the function, 'global or local...', it's contained within because it's local to that function. Below describes some ways of dealing with this.
'''
```

