In Python, a **method** is a function that belongs to an object which allows you to access or modify its state.

# Method Syntax in Python

You call methods using dot notation:

```python
object.method_name(arguments)
```

The variable that references the object comes first, then a period `.`, then the method name and parentheses which contain any arguments. Below are some examples; don't worry about the exact objects of methods for now, just the syntax:

```python
my_list.append(5)       # Call append() method on my_list, pass 5 as an argument
my_string.upper()       # Call upper() method on my_string
my_dict.get("key")      # Call get() method on my_dict and pass "key" as an argument
```

Remember, even if a method doesn't require arguments, you still need to include the parentheses when calling it (e.g. `my_string.upper()`{.python}, not `my_string.upper`{.python}).

# Methods Are Tied to Types

Methods only exist for their specific type. You can't call a method that doesn't belong to the type of object:

```py-cell
my_list = [1, 2, 3] # Create a list
my_string = "hello" # Create a string

my_list.append(4)           # Works - lists have append
print(my_list)

my_string.append("!")       # AttributeError - strings don't have append
```
