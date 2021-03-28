---
title: Python Variables
weight: 20
menu:
  notes:
    name: Variables
    identifier: notes-python-variables
    parent: notes-python
    weight: 20
---

<!-- ========== Creating Variable ============== -->
{{< note title="Creating Variable" size="medium">}}
Python has no command for declaring a variable. A variable is created the moment you first assign a value to it.

```python
x = 5
y = "John"
print(x)
print(y)
```

{{< /note >}}

<!-- ======== Dynamic Type of Variable ============= -->
{{< note title="Dynamic Type" size="medium" >}}
Variables do not need to be declared with any particular type, and can even change type after they have been set.

```python
x = 4       # x is of type int
x = "Sally" # x is now of type str
```

{{< /note >}}

<!-- =============== Variable Casting =============== -->
{{< note title="Casting" >}}

```python
x = str(3)    # x will be '3'
y = int(3)    # y will be 3
z = float(3)  # z will be 3.0
```

{{< /note >}}

<!-- =============== Getting the Type of a variable =============== -->
{{< note title="Getting Type of a Variable" >}}
You can get the data type of a variable with the `type()` function.

```python
x = 5
y = "John"
print(type(x))
print(type(y))
```

{{< /note >}}

<!-- =============== Single Quote vs Double Quote =============== -->
{{< note title="Single Quote vs Double Quote" >}}

```python
x = "John"
# is the same as
x = 'John'
```

{{< /note >}}

<!-- =============== Case sensitivity =============== -->
{{< note title="Case sensitivity" >}}
Variable names are case-sensitive. This will create two variables:

```python
a = 4
A = "Sally"
#A will not overwrite a
```
{{< /note >}}


<!-- =============== Variable Name =============== -->
{{< note title="Variable naming convention" size="large">}}

Variable name must follow the criteria:

- A variable name must start with a letter or the underscore character
- A variable name cannot start with a number
- A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )
- Variable names are case-sensitive (age, Age and AGE are three different variables)

```py
myvar = "John"
my_var = "John"
_my_var = "John"
myVar = "John"
MYVAR = "John"
myvar2 = "John"
```

{{< /note >}}

<!-- =============== Batch Assignment =============== -->
{{< note title="Batch Assignment: Different values at different variable" size="medium">}}
Python allows you to assign values to multiple variables in one line:

```py
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)
```

The number of variable in left side must be equal to the number of values in right side. Otherwise, it will give error.

{{< /note >}}

<!-- =============== Batch Assignment: M:1 =============== -->
{{< note title="Batch Assignment: One value into multiple variables" size="medium">}}
```py
x = y = z = "Orange"
print(x)
print(y)
print(z)
```
{{< /note >}}


<!-- =============== Unpacking a Collection =============== -->
{{< note title="Unpacking a Collection" size="large">}}
If you have a collection of values in a list, tuple etc. Python allows you extract the values into variables. This is called unpacking.

```py
fruits = ["apple", "banana", "cherry"]
x, y, z = fruits
print(x)
print(y)
print(z)
```

{{< /note >}}

<!-- =============== Global Variable =============== -->
{{< note title="Global Variable" size="large">}}
Variables that are created outside of a function (as in all of the examples above) are known as global variables.

Global variables can be used by everyone, both inside of functions and outside.

**Example:**
```py
x = "awesome"

def myfunc():
  x = "fantastic"
  print("Python is " + x)

myfunc()

print("Python is " + x)
```

**Output:**

```bash
Python is fantastic
Python is awesome
```

{{< /note >}}

<!-- =============== Global Variable using `global` Keyword =============== -->
{{< note title="Global Variable using `global` Keyword" size="auto">}}
We can also expose a local variable from inside a function to act as a  global variable using `global` keyword.

**Example 1:**
```py
def myfunc():
  global x
  x = "fantastic"

myfunc()

print("Python is " + x)
```

**Output:**
```bash
Python is fantastic
```

**Example 2:**
```py
x = "awesome"

def myfunc():
  global x
  x = "fantastic"

myfunc()

print("Python is " + x)
```

**Output:**
```bash
Python is fantastic
```

{{< /note >}}

