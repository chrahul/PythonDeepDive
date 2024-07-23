### Python Functions: A Detailed Tutorial with Examples

#### How to Write a Function

A function in Python is defined using the `def` keyword, followed by the function name, parentheses, and a colon. The code block within every function starts with a colon (:) and is indented.

**Example:**

```python
def greet(name):
    print(f"Hello, {name}!")

greet("Rahul")
```

#### Positional vs. Keyword Arguments

- **Positional Arguments:** Arguments that are passed to functions in the order they are defined.
- **Keyword Arguments:** Arguments that are passed to functions by explicitly specifying the parameter name.

**Example:**

```python
def describe_person(name, age):
    print(f"{name} is {age} years old.")

# Positional arguments
describe_person("Rahul", 35)

# Keyword arguments
describe_person(age=35, name="Rahul")
```

#### Default Arguments

Default arguments are values that are provided to function parameters if no argument is passed.

**Example:**

```python
def greet(name, msg="Hello"):
    print(f"{msg}, {name}!")

greet("Rahul")
greet("Rahul", "Good Morning")
```

#### Mixed Positional and Keyword Arguments

You can mix positional and keyword arguments. However, positional arguments must be placed before keyword arguments.

**Example:**

```python
def display_info(name, age, city="Hyderabad"):
    print(f"{name} is {age} years old and lives in {city}.")

display_info("Rahul", 35)
display_info("Rahul", 35, city="Bangalore")
```

#### Iterators vs. Generators

- **Iterators:** Objects that implement the iterator protocol (methods `__iter__()` and `__next__()`).

**Example:**

```python
my_list = [1, 2, 3, 4]
iterator = iter(my_list)

print(next(iterator))
print(next(iterator))
```

- **Generators:** Functions that yield values using the `yield` keyword, creating an iterator.

**Example:**

```python
def simple_generator():
    yield 1
    yield 2
    yield 3

gen = simple_generator()

print(next(gen))
print(next(gen))
```

#### Global vs. Local Variables

- **Global Variables:** Declared outside any function and can be accessed anywhere.
- **Local Variables:** Declared inside a function and can be accessed only within that function.

**Example:**

```python
global_var = "I am global"

def my_function():
    local_var = "I am local"
    print(global_var)
    print(local_var)

my_function()
print(global_var)
```

#### Recursive Function

A recursive function is a function that calls itself.

**Example:**

```python
def factorial(n):
    if n == 1:
        return 1
    else:
        return n * factorial(n - 1)

print(factorial(5))
```

#### Python Module

A module is a file containing Python definitions and statements. A module can define functions, classes, and variables. It is different from a function as it can contain multiple functions and other code.

**Example:**

Create a module named `mymodule.py`:

```python
# mymodule.py
def greet(name):
    return f"Hello, {name}!"
```

Use the module in another script:

```python
# main.py
import mymodule

print(mymodule.greet("Rahul"))
```

#### Nested Functions

A nested function is a function defined inside another function.

**Example:**

```python
def outer_function(text):
    def inner_function():
        print(text)
    inner_function()

outer_function("Hello from the inner function!")
```

### Summary

This tutorial covered the following topics:
1. Writing functions in Python.
2. Positional vs. Keyword arguments.
3. Default arguments.
4. Mixing positional and keyword arguments.
5. Iterators vs. Generators.
6. Global vs. Local variables.
7. Recursive functions.
8. Python modules.
9. Nested functions.

Each concept was illustrated with examples to provide a clear understanding of how to use these features in Python programming.
