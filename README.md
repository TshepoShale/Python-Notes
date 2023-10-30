# Introduction to Python: 
## Week 1: 
## Day 1: 
### What is Python?:
Python is an interpreted language. This means that a new executable file is created when you run your code. The next time that you execute your code, this new executable file is run instead of the original file.
It is a relatively simple language that includes a standard library that provides modules for a large number of processes that programs deal with. This approach keeps Python simple yet reliable programming language. Python has an easy-to-use syntax that is focused on the programmer who must type in the program, read what was typed, and provide formal documentation for the program. Python strikes a good balance between fast compilations and readability, and it is easier to write applications.
Python is implemented in C and relies on the extensive, well understood, portable C libraries. It fits seamlessly with UNIX, Linux, and POSIX environments. Since these standard C libraries are widely available for the various MS-Windows variants, and other non-POSIX operating systems, Python runs similarly in all environments. The Python programming language was created based on lessons learned during language and operating system support. Python is built from concepts in the ABC and Modula-3 languages.
### Comments in Python: 
Comments are added to make the source code easier to understand. Comments in Python start with the hash character, #, and extend to the end of the physical line. A comment may appear at the start of a line or following whitespace or code, but not within a string literal. 
### Creating Applications using Python: 
 Indentation in Python identifies what code belongs to what section of code.
 ### Escape Sequences: 
* Backslash character (\):  e.g \\
* New line feed: \n
* Tab: \t
* Vertical tab: \v
* Backspace: \b
* Carriage return: \r
* Single quote (useful in strings enclosed in single quotes: ‘hello \ ‘World’): \\'
* Double quote (useful in strings enclosed in single quotes: “hello \ “World”): \\"


### Reserved words in Python:
NB: Cannot be used as ordinary identifiers, must be spelled *EXACTLY* as wriiten here:
False      class      finally    is         return
None       continue   for        lambda     try
True       def        from       nonlocal   while
and        del        global     not        with
as         elif       if         or         yield
assert     else       import     pass

# Python 3.5 keywords (added 'async', 'await', 'asynchronous', 'contextlib', 'async for', 'async with')
async      await      async def  async for  async with
asynchronous contextlib

# Python 3.6 keywords (added 'f' for formatted string literals)
f          False      async      await      True

# Python 3.7 keywords (added 'async' and 'await' as non-keyword identifiers, 'contextvars', 'nonlocal', 'dataclasses')
async      await      contextvars dataclasses nonlocal

# Python 3.8 keywords (added 'walrus' operator ':=')
:=

# Python 3.9 keywords (added 'match' statement)
match

### Anaconda Navigator: 
Anaconda is a popular open-source distribution of Python and other data science-related packages. It simplifies the process of installing, managing, and updating Python libraries for data science, machine learning, and scientific computing. Anaconda includes tools such as conda, a powerful package manager, and provides an environment management system, allowing users to create isolated Python environments for different projects, making it easier to manage dependencies and avoid conflicts between packages.

## Day 2: 
## Variables: 
Variables in programming act as temporary storage spaces in a computer's memory, holding various data values. When a variable's value changes, it affects the program's current state. They serve as containers for different data items, and understanding them is essential for programming. Variables are crucial in all programming languages, allowing data transfer between functions and making programming tasks more manageable.
Each variable is created with an initial value. A value can be in *THREE* states: 
1. Variable creation (Declaration)
2. Variable assignment (Initialization)
3. Variable changed (Execution)

NB: Once the code which created the variable has finished executing, the variable is destroyed.

NB: In Python, variables are defined in a standard way, by using the assignment character (=). This changes the value of the variable. Naming conventions specify the way in which variables should be named. This standard is used to make code more readable, and thus easier to understand.

The rules include the start and continuation characters. Variable names may contain any upper or lower case letter (A–Z, a–z), a number, or the underscore character. They may not begin with a number or contain spaces. Continuation characters are any characters except whitespace characters like tab and space.

Here are a few examples of valid variable names:

* c
* ref_number
* admin
* aVeryLongName

  
Here are a few examples of invalid variable names:

* True
* $name
* 12Graph

NB: *In Python identifiers are case sensitive!!!*

NB: *Variables cannot have the same name as Python’s keywords!!!*

We can find out what keywords are in Python, by using the function called dir(). If this function is called with the __builtins__ attribute, it returns a list of Python’s built-in attributes.

The __builtins__ module contains all Python’s built-in attributes, which can be used with the dir()function.

The ones that are returned are identified with the following characteristics:

* Python’s built-in exceptions start with a capital letter.
* The rest are either functions or data type names.
* Identifiers that start and end with one or two underscores are special methods.

  NB: *All of the methods, exceptions, and functions contained in  
dir(__builtins__), dir(__doc__), dir(__name__), and dir(__package__) cannot be used as variable names.*

### Using Variables: 
* All variables are assigned to a data type, be it a STRING, or an INTEGER. 
* Values of the same type can be manipulated together.
* In Python, automatic type conversion, also known as implicit casting, allows the interpreter to automatically convert compatible data types, such as integers to floats or floats to strings, as needed during operations or assignments, simplifying code and enhancing flexibility.

### Casting: 

#### Implicit Casting: 
In Python, automatic type conversion, also known as implicit casting, allows the interpreter to automatically convert compatible data types, such as integers to floats or floats to strings, as needed during operations or assignments, simplifying code and enhancing flexibility. Also ensures that no data is lost when these conversions occur. 

#### Explicit Casting: 
A value cannot be automatically cast from one data type to another if it will result in data loss. Extra code has to be written to ensure that the value stays the same and only the data type changes; like when casting from a floating-point value to an integer value. 

The rules to convert a string to a float are:
* The string should only contain numbers.
* Other than numbers the following are allowed:
* Only one dot (.) character. Indicates the decimal starts after the dot (.) character.
A ‘+’ or ‘−‘ character at the beginning of the string. This indicates that the number is either positive or negative.

## Day 3: 
## Data Types: 

NB: Literals are an alternative to using variables. Literals are values that never change, i.e. they are a constant.
Examples of literals: 
* "\t"
* "This is only a string"
* "2"
### Intergers:
 These represent numbers in an unlimited range. This is only limited by a machine’s memory.
 ### Booleans: 
  Evaluate to ‘True or False’, 1 or 0 respectively.
  ###  Floating point numbers:
  Floating-point numbers represent double-precision numbers.
### Complex numbers:
 Complex numbers represent numbers as a pair of double-precision numbers.
 ### Strings: 
A sequence of Unicode characters e.g. a word or a sentence that can be manipulated.


## Day 4: 
### Operators:  
#### Arithmetic Operators:
Arithmetic operators are used for basic mathematical operations.

x = 10
y = 5

addition = x + y  # Result: 15
subtraction = x - y  # Result: 5
multiplication = x * y  # Result: 50
division = x / y  # Result: 2.0 (in Python 3.x, division always returns a float)
modulus = x % y  # Result: 0 (remainder of x divided by y)
exponentiation = x ** y  # Result: 100000

#### Comparison Operators:
Comparison operators are used to compare two values.

x = 10
y = 5

is_equal = x == y  # Result: False
not_equal = x != y  # Result: True
greater_than = x > y  # Result: True
less_than = x < y  # Result: False
greater_or_equal = x >= y  # Result: True
less_or_equal = x <= y  # Result: False


#### Logical Operators:
Logical operators are used for combining conditional statements.

**x = True
y = False

logical_and = x and y  # Result: False
logical_or = x or y  # Result: True
logical_not = not x  # Result: False

#### Assignment Operators:
Assignment operators are used to assign values to variables.

x = 10

x += 5  # Equivalent to: x = x + 5 (Result: 15)
x -= 3  # Equivalent to: x = x - 3 (Result: 12)
x *= 2  # Equivalent to: x = x * 2 (Result: 24)
x /= 4  # Equivalent to: x = x / 4 (Result: 6.0)

#### Identity Operators:
Identity operators are used to compare the objects, not if they are equal, but if they are actually the same object.

x = [1, 2, 3]
y = [1, 2, 3]

is_same_object = x is y  # Result: False (different objects)
is_not_same_object = x is not y  # Result: True

#### Membership Operators:
Membership operators are used to test if a sequence (such as a list, tuple, or string) contains a specific item.
my_list = [1, 2, 3, 4, 5]

is_present = 3 in my_list  # Result: True
is_not_present = 6 not in my_list  # Result: True

#### Bitwise Operators:
Bitwise operators are used for bitwise operations on integers.
x = 5
y = 3

bitwise_and = x & y  # Result: 1 (bitwise AND of 5 and 3 in binary: 101 & 011 = 001)
bitwise_or = x | y  # Result: 7 (bitwise OR of 5 and 3 in binary: 101 | 011 = 111)
bitwise_xor = x ^ y  # Result: 6 (bitwise XOR of 5 and 3 in binary: 101 ^ 011 = 110)
bitwise_not_x = ~x  # Result: -6 (bitwise NOT of 5 in binary: ~101 = 11111111111111111111111111111010)
left_shift = x << 1  # Result: 10 (left shift 5 by 1 bit: 101 << 1 = 1010)
right_shift = x >> 1  # Result: 2 (right shift 5 by 1 bit: 101 >> 1 = 10)







