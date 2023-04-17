# Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both.
In Python, the variable scope refers to the region of the program where a particular variable is accessible. The scope of a variable can be either local or global.

Local scope refers to the region of the program where a variable is defined within a function, and it can only be accessed within that function. Global scope, on the other hand, refers to the region of the program where a variable is defined outside any function, and it can be accessed from any part of the program.
```
x = 10    # Global variable

def my_func():
    y = 5  # Local variable
    print("x within the function:", x)   # Accessing global variable
    print("y within the function:", y)   # Accessing local variable

my_func()

print("x outside the function:", x)   # Accessing global variable outside function
#print("y outside the function:", y)   # This will give an error as y is not defined in global scope

```
# How do the global and nonlocal keywords work in Python, and in what situations might you use them?
In Python, the global and nonlocal keywords are used to access variables in different scopes.

The global keyword is used to access and modify a variable in the global scope from within a function. The nonlocal keyword is used to access and modify a variable in the parent function from within a nested function.

You might use these keywords when you want to modify a variable that is outside the current function's scope, or when you want to avoid creating a new variable with the same name as an existing variable in a higher scope.

# In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis
Big O notation is used to describe the time and space complexity of an algorithm in terms of the size of its input. It's important because it allows us to compare different algorithms and choose the most efficient one for a given problem



# Based on the Rolling Dice Example, explain how you would simulate a dice roll using Python. Describe how you would use code to calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials

To simulate a dice roll in Python, we can use the random module's randint function to generate a random integer between 1 and 6, which corresponds to the numbers on a standard dice. Here's an example code snippet to simulate a dice roll:
```
import random

# Simulate a dice roll
dice_roll = random.randint(1, 6)
print("The dice roll is:", dice_roll)

```
To calculate the probability of rolling a specific number over a large number of trials, we can use a loop to simulate multiple dice rolls and count the number of times the desired number is rolled. Here's an example code snippet to calculate the probability of rolling a 6 over 10,000 tri
```
import random

num_trials = 10000
num_sixes = 0

for i in range(num_trials):
    dice_roll = random.randint(1, 6)
    if dice_roll == 6:
        num_sixes += 1

probability = num_sixes / num_trials
print("The probability of rolling a 6 is:", probability)

```

In this code, we use a loop to simulate 10,000 dice rolls and count the number of times a 6 is rolled. We then divide the number of sixes by the total number of rolls to get the probability of rolling a 6.
