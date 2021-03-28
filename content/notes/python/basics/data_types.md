---
title: Python Data Types
weight: 30
menu:
  notes:
    name: Data Types
    identifier: notes-python-data-types
    parent: notes-python
    weight: 30
---

<!-- =============== Built-in Data Types =============== -->
{{< note title="Built-in Data Types" size="auto">}}
| Category       | Built-in Data Types                |
| -------------- | ---------------------------------- |
| Text Type      | `str`                              |
| Numeric Types  | `int`, `float`, `complex`          |
| Sequence Types | `list`, `tuple`, `range`           |
| Mapping Type   | `dict`                             |
| Set Types      | `set`, `frozenset`                 |
| Boolean Type   | `bool`                             |
| Binary Types   | `bytes`, `bytearray`, `memoryview` |

{{< /note >}}

<!-- =============== Get Type of a Variable =============== -->
{{< note title="Get Type of a Variable" size="auto">}}
Print the data type of the variable x:

```py
x = 5
print(type(x))
```

Output:

```bash
<class 'int'>
```

{{< /note >}}

<!-- =============== Setting Data-Type of a Variable =============== -->
{{< note title="Setting Data-Type of a Variable" size="large">}}
When we assign something into a variable, python dynamically set it's data type according to the value we are trying to assign.

| Example                                        | Data-Type    |
| ---------------------------------------------- | ------------ |
| `x = "Hello World"`                            | `str`        |
| `x = 20`                                       | `int`        |
| `x = 20.5`                                     | `float`      |
| `x = 1j`                                       | `complex`    |
| `x = ["apple", "banana", "cherry"]`            | `list`       |
| `x = ("apple", "banana", "cherry")`            | `tuple`      |
| `x = range(6)`                                 | `range`      |
| `x = {"name" : "John", "age" : 36}`            | `dict`       |
| `x = {"apple", "banana", "cherry"}`            | `set`        |
| `x = frozenset({"apple", "banana", "cherry"})` | `frozenset`  |
| `x = True`                                     | `bool`       |
| `x = b"Hello"`                                 | `bytes`      |
| `x = bytearray(5)`                             | `bytearray`  |
| `x = memoryview(bytes(5))`                     | `memoryview` |

{{< /note >}}

<!-- =============== Setting specific data type =============== -->
{{< note title="Setting Specific Data-Type" size="auto">}}


| Example                                        | Data Type    |
| ---------------------------------------------- | ------------ |
| `x = str("Hello World")`                       | `str`        |
| `x = int(20)`                                  | `int`        |
| `x = float(20.5)`                              | `float`      |
| `x = complex(1j)`                              | `complex`    |
| `x = list(("apple", "banana", "cherry"))`      | `list`       |
| `x = tuple(("apple", "banana", "cherry"))`     | `tuple`      |
| `x = range(6)`                                 | `range`      |
| `x = dict(name="John", age=36)`                | `dict`       |
| `x = set(("apple", "banana", "cherry"))`       | `set`        |
| `x = frozenset(("apple", "banana", "cherry"))` | `frozenset`  |
| `x = bool(5)`                                  | `bool`       |
| `x = bytes(5)`                                 | `bytes`      |
| `x = bytearray(5)`                             | `bytearray`  |
| `x = memoryview(bytes(5))`                     | `memoryview` |

{{< /note >}}
