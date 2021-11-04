# sturdy-barnacle
week 3 exception handling (copy of the program from the cmd.exe - python)
Microsoft Windows [Version 10.0.22000.282]
(c) Microsoft Corporation. All rights reserved.

C:\Users\chris\Desktop>python
Python 3.7.9 (tags/v3.7.9:13c94747c7, Aug 17 2020, 16:30:00) [MSC v.1900 64 bit (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.
>>> 1/0
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
ZeroDivisionError: division by zero
>>> y = a + 5
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'a' is not defined
>>> a = [1, 2, 3]
>>> a[10]
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
IndexError: list index out of range
>>> # potential code before try catch
>>> try:
...
  File "<stdin>", line 2

    ^
IndentationError: expected an indented block
>>> a = 1
>>> try:
...     b = int(input("Please enter a number to divide a"))
...     a = a/b
...     print("Success a=", a)
... except:
...     print("There was an error")
...
Please enter a number to divide a1
Success a= 1.0
>>>  a = 1
  File "<stdin>", line 1
    a = 1
    ^
IndentationError: unexpected indent
>>> a = 1
>>> try:
...     b = int(input("Please enter a number to divide a"))
...     a = a/b
...     print("Success! a =  ", a)
... except ZeroDivisionError:
...     print("The number you provided can't divide 1 because it is 0")
... except ValueError:
...     print("You did not provide a number")
... except:
...     print("Something went wrong")
...
Please enter a number to divide a
You did not provide a number
>>> 0
0
>>> 1
1
>>> d
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
NameError: name 'd' is not defined
>>> a = 1
>>> try:
...     b = int(input("Please enter a number to divide a "))
...     a = a/b
... except ZeroDivisionError:
...     print("The number you provided can't divide 1 because it is 0")
...
Please enter a number to divide a 0
The number you provided can't divide 1 because it is 0
>>> try:
... ...     b = int(input("Please enter a number to divide a "))
  File "<stdin>", line 2
    ...     b = int(input("Please enter a number to divide a "))
      ^
IndentationError: expected an indented block
>>> ...     a = a/b
  File "<stdin>", line 1
    ...     a = a/b
            ^
SyntaxError: invalid syntax
>>> ... except ZeroDivisionError:
  File "<stdin>", line 1
    ... except ZeroDivisionError:
             ^
SyntaxError: invalid syntax
>>> a = 1
>>> try:
...     b = int(input("PLease enter a number to divide a "))
...     a = a/b
...     print("Success a= ",a)
... except:
...     print("Something went wrong")
...
PLease enter a number to divide a 0
Something went wrong
>>> a = 1
>>> try:
...     b = int(input("Please enter a number to divide a "))
...     a = a/b
... except ZeroDivisionError:
...     print("The number you provided can't divide 1 because it is 0")
... except ValueError:
...     print("You did not provide a number")
... except:
...     print("Something went wrong")
... else:
...     print("Success! a = ",a)
...
Please enter a number to divide a 1
Success! a =  1.0
>>> a = 1
>>> try:
...     b = int(input("Please enter a number to divide a "))
...     a = a/b
... except ZeroDivisionError:
...     print("The number you provided can't divide 1 because it is 0")
... except ValueError:
...     print("You did not provide a number")
... except:
...     print("Something went wrong")
... else:
...     print("Success! a = ",a)
... finally:
...     print("Processing complete")
...
Please enter a number to divide a s
You did not provide a number
Processing complete
>>>
