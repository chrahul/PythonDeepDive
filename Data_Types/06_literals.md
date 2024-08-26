Let's dive into our next topic: literals.

**What are literals?**

Literals are direct values written in the program. These are the raw data values that we assign directly to variables within the code. Earlier, we discussed how variables are used to store data. For example, if we have a variable `price`, we might store the value `250` in it. This value, `250`, is the data, and because it's directly written in the program, it's called a literal.

**Is there any other way to get data into the program?**

Yes, there are several methods. However, let's focus on two: 
1. Taking input from the user.
2. Directly assigning a value in the program.

Consider a variable `price`. We can store data in `price` either by taking input from the user or by directly assigning a value in the code.

**Example 1: Taking Input**

```python
price = input("Enter the price: ")
```

Here, the user can input a value via the keyboard, which is then stored in the `price` variable. If the user enters `250`, the `price` variable will hold this value. Even though the user entered it, it's still data, and this data becomes a literal once it's assigned to the variable.

**Example 2: Direct Assignment**

```python
price = 250
```

In this case, we've directly written the value `250` in the program. This value is fixed in the code and will always be the same whenever the program runs. Such a value is known as a constant value, which is also referred to as a literal.

**Recap:**

- Variables are used to store values.
- Values can be assigned through user input or directly in the program.
- When a value is directly written in the code, it's called a literal.

**Types of Literals**

Python allows various types of literals:

- **Integer Literals**: Whole numbers, e.g., `10`, `250`, `-42`.
- **Float Literals**: Numbers with a decimal point, e.g., `10.5`, `-0.001`, `3.14`.
- **String Literals**: Text enclosed in quotes, e.g., `"Hello"`, `'John'`.
- **Boolean Literals**: `True` or `False`.
- **Complex Literals**: Numbers with a real and an imaginary part, e.g., `5 + 4j`.

**Integer Literals**

You can directly assign integer values to variables, like:

```python
a = 123
b = 12520
```

To make large numbers more readable, Python allows the use of underscores to separate digits:

```python
b = 12_520
c = 1_234_567_890
```

**Float Literals**

Float numbers are created by including a decimal point in the value:

```python
f = 12.59
g = 13.0  # This is a float because of the .0
```

Python also supports scientific notation for floats:

```python
h = 1.32e2  # This is 1.32 * 10^2, or 132.0
```

Just like with integers, you can use underscores to separate digits for better readability:

```python
f = 123_456.789
g = 123.456_789
```

**Boolean Literals**

Boolean literals represent the truth values in Python:

```python
is_active = True
is_logged_in = False
```

**Complex Literals**

Complex numbers consist of a real part and an imaginary part:

```python
z = 5 + 4j
```

Underscores can also be used to separate digits in complex numbers:

```python
z = 5_000 + 4_000j
```

**String Literals**

Strings can be enclosed in either single or double quotes:

```python
name = 'John'
greeting = "Hello"
```

Even if you store a single character in a variable, it's still considered a string in Python:

```python
char = 'A'  # This is a string, not a character type
```

**Demonstration:**

Let's look at some examples:

- **Integer Literal**:

  ```python
  a = 123_456
  print(a)  # Output: 123456
  ```

- **Float Literal**:

  ```python
  f = 123.45
  print(f)  # Output: 123.45
  ```

- **Complex Literal**:

  ```python
  z = 5_000 + 4_000j
  print(z)  # Output: (5000+4000j)
  ```

- **String Literal**:

  ```python
  name = "John"
  print(name)  # Output: John
  ```

**User Input Example**:

```python
price = input("Enter price: ")
print(price)  # This will output the entered value as a string
```

If you directly assign a value:

```python
price = 250
print(price)  # Output: 250
```

This is a literal.

In the next lecture, we’ll explore more about literals and how they can be used in Python programs. Stay tuned!
