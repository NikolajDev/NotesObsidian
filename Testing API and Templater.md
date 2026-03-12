# Section 1.2: Creating Variables and Assigning Values

## Basic Assignment

To create a variable in Python, specify the name and assign a value:

```python
<variable name> = <value>
```

Python uses `=` to assign values. No need to declare a variable in advance or specify a data type — assigning a value declares and initializes it automatically.

---

## Variable Types

```python
# Integer
a = 2
print(a)
# Output: 2

# Large integer
b = 9223372036854775807
print(b)
# Output: 9223372036854775807

# Floating point
pi = 3.14
print(pi)
# Output: 3.14

# String
c = 'A'
print(c)
# Output: A

# String
name = 'John Doe'
print(name)
# Output: John Doe

# Boolean
q = True
print(q)
# Output: True

# Empty / null
x = None
print(x)
# Output: None
```

---

## Automatic Type Detection

Python automatically picks the most suitable type:

```python
a = 2
print(type(a))
# Output: <class 'int'>

pi = 3.14
print(type(pi))
# Output: <class 'float'>

c = 'A'
print(type(c))
# Output: <class 'str'>

q = True
print(type(q))
# Output: <class 'bool'>

x = None
print(type(x))
# Output: <class 'NoneType'>
```

---

## Variable Naming Rules

1. **Must start with a letter or underscore**
```python
x = True      # valid
_y = True     # valid
9x = False    # SyntaxError: starts with numeral
$y = False    # SyntaxError: starts with symbol
```

2. **Can contain letters, numbers and underscores**
```python
has_0_in_it = "Still Valid"
```

3. **Case sensitive**
```python
x = 9
y = X * 5
# NameError: name 'X' is not defined
```

4. **Cannot use Python keywords**
```python
import keyword
print(keyword.kwlist)
# ['False', 'None', 'True', 'and', 'as', ...]
```

---

## Multiple Assignment

### Assign multiple variables in one line
```python
a, b, c = 1, 2, 3
print(a, b, c)
# Output: 1 2 3
```

### Mismatched count raises ValueError
```python
a, b, c = 1, 2
# ValueError: need more than 2 values to unpack

a, b = 1, 2, 3
# ValueError: too many values to unpack
```

### Use `_` to discard unwanted values
```python
a, b, _ = 1, 2, 3
print(a, b)
# Output: 1 2
```

---

## Cascading Assignment

Assign the same value to multiple variables:

```python
a = b = c = 1
print(a, b, c)
# Output: 1 1 1
```

All three names refer to the **same object** in memory. Reassigning one does not affect others:

```python
a = b = c = 1
b = 2
print(a, b, c)
# Output: 1 2 1
```

### Mutable types behave differently
```python
x = y = [7, 8, 9]   # x and y point to the SAME list
x[0] = 13            # modifying through x
print(y)
# Output: [13, 8, 9] # y is also changed!

x = y = [7, 8, 9]
x = [13, 8, 9]       # x now points to a NEW list
print(y)
# Output: [7, 8, 9]  # y unchanged
```

---

## Dynamic Typing

Variables are not locked to a type — you can reassign to a different type:

```python
a = 2
print(type(a))
# Output: <class 'int'>

a = 'hello'
print(type(a))
# Output: <class 'str'>
```

---

## Invalid Assignment

Assignment goes left to right only:

```python
0 = x
# SyntaxError: can't assign to literal
```

---

## Notes
- Python variables are **names** (references) pointing to objects, not containers
- `=` assigns a reference to the object on the right to the name on the left
- Multiple names can refer to the same object
- 