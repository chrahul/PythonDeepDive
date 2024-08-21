 **"What are Exceptions?"**:

---

### What are Exceptions?

In programming, an **exception** is a type of error that occurs during the execution of a program. Unlike syntax errors, which are detected before the program is run, exceptions occur while the program is running, causing it to terminate abnormally. These are known as **runtime errors**.

#### How Exceptions Differ from Other Errors

Before diving into exceptions, let's recap the different types of errors in a program:

1. **Syntax Errors**: These are errors in the code structure. They occur when the code doesn't conform to the rules of the programming language, such as missing colons or incorrect indentation in Python. If a syntax error is present, the program won't run at all, as Python will fail to convert the code into executable form.

2. **Logical Errors**: These errors occur when the program runs without crashing but produces incorrect results. Logical errors are harder to detect because the program doesn't give any immediate indication of failure—it's the output that is wrong.

3. **Runtime Errors (Exceptions)**: These occur while the program is running. The program starts executing correctly, but something unexpected happens, such as dividing by zero or trying to access a variable that doesn't exist. These errors cause the program to stop running and generate an exception.

#### Understanding Exceptions

Exceptions are Python's way of signaling that something unexpected happened during execution. When an exception occurs, the normal flow of the program is disrupted, and Python provides a traceback, which helps you understand what went wrong and where in the code it happened.

Here are some common exceptions in Python:

- **ZeroDivisionError**: Occurs when you attempt to divide by zero.
- **NameError**: Raised when a local or global name is not found.
- **TypeError**: Triggered when an operation or function is applied to an object of inappropriate type.
- **ValueError**: Raised when a function receives an argument of the correct type but inappropriate value.

#### Example of an Exception

Consider the following code, which divides two numbers:

```python
a = 10
b = 0
result = a / b
print(result)
```

If you run this code, you'll get a `ZeroDivisionError`, because dividing by zero is not mathematically valid:

```
Traceback (most recent call last):
  File "main.py", line 3, in <module>
    result = a / b
ZeroDivisionError: division by zero
```

#### The Importance of Handling Exceptions

If exceptions are not handled, they can cause your program to crash. To make your programs more robust, you can use **exception handling** techniques to gracefully manage these errors. This involves anticipating possible exceptions and providing a way to handle them, ensuring that the program can continue to run or fail gracefully.

In the next sections, we will delve deeper into exception handling in Python, exploring how to catch exceptions, use `try-except` blocks, and understand the full lifecycle of an exception in a Python program.

--- 

This section provides a thorough understanding of what exceptions are and sets the stage for diving deeper into exception handling.
