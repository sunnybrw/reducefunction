#reducefunction
In Python, you can use the reduce function from the functools module to apply a function cumulatively to the items of an iterable, from left to right, so as to reduce the iterable to a single value. 

If you want to use reduce without a lambda function, you can define a regular function and pass it to reduce.

Here's an example:
```
from functools import reduce

## Define a regular function to add two numbers

def add(x, y):
    return x + y

# Use reduce with the add function
numbers = [1, 2, 3, 4, 5]
result = reduce(add, numbers)

print(result)  # Output will be 15

```
In this example, the add function is defined to take two arguments and return their sum. The reduce function then applies add cumulatively to the items in the numbers list, resulting in the sum of all numbers in the list.

Remember to import reduce from functools as it is not a built-in function in Python 3.

