# Recursion

A recursive definition is one in which the defined term appears in the definition itself. Self-referential situations often crop up in real life, even if they aren’t immediately recognizable as such. For example, suppose you wanted to describe the set of people that make up your ancestors. You could describe them this way:

- Your ancestors = {your parents} + {your parents' ancestors}

Notice how the concept that is being defined, ancestors, shows up in its own definition. This is a recursive definition.

## Application

Useful when we need to repeat reference to a object within its own call.

```python

def countdown(n):
    print(n)
    if n == 0:
        return             # Terminate recursion
    else:
        countdown(n - 1)   # Recursive call

countdown(20)

```

### Counting number of items in a list

```python
def count_leaf_items(item_list):
    """Recursively counts and returns the
       number of leaf items in a (potentially
       nested) list.
    """
    count = 0
    for item in item_list:
        if isinstance(item, list):
            count += count_leaf_items(item)
        else:
            count += 1

    return print(count)
```

# Classes

When working on projects, you will most likely find yourself utilizing plenty of self-made functions and variables. You may have even create an entire script filled with functions you created in order to streamline the process of your project.
The purpose of these functions can be for numerous things within your code. From cleaning your DataFrame to training a machine learning model. It’s useful to create a ton of functions in order to organize your Python code but there is another way to make your code look and act more presentable - by using a Python Class!
A class rests on the premise that the item of interest in your program - the object - would consist of both the entities you want to manipulate and the actions you want to perform on those entities. An object is therefore a software entity that contains boh data and procedures. 
- The data contained in an object is known as its attributes.
- Attributes are variables that access data
- Actions (precedures) that objects perform called methods

A class is code that specifies the data attributes and methods of a particulatr type of object

```python
import random
import random

# The Coin class simulates a coin that can be flipped.

class Coin:

# The _ _init_ _ method initializes the
# sideup data attribute with 'Heads'.
    def _ _init_ _(self):
        self.sideup = 'Heads'

# The toss method generates a random number
# in the range of 0 through 1. If the number
# is 0, then sideup is set to 'Heads'.
# Otherwise, sideup is set to 'Tails'.

    def toss(self):
        if random.randint(0, 1) == 0:
              self.sideup = 'Heads'
          else:
              self.sideup = 'Tails'

# The get_sideup method returns the value
# referenced by sideup.

      def get_sideup(self):
          return self.sideup
```


## Encapsulation
Combining code and attrributes (data) together is known as encapsulation.
- Encapsulation is the combination of code and data 