# Variables and Datatypes

## Creating Variables (Section 1.2)
Python uses `=` to assign values to variables. There's no need to declare a variable in advance. Assigning a value to a variable itself declares and initializes it.

```python
# Integer
a = 2

# Floating point
pi = 3.14

# String
name = 'John Doe'

# Boolean
q = True

# Empty value (Null)
x = None
```

## Datatypes (Section 1.4)
Even though there's no need to specify a data type, Python automatically picks the most suitable built-in type. You can check the type using the `type()` function.

```python
a = 2
b = 3.14
c = 'Hello'

print(type(a))
print(type(b))
print(type(c))
```

## Console Output
<div style="background: #0c0c0c; color: #00ff41; padding: 20px; font-family: 'Courier New', monospace; border-radius: 8px; border: 1px solid #333;">
$ python datatypes.py<br>
&lt;class 'int'&gt;<br>
&lt;class 'float'&gt;<br>
&lt;class 'str'&gt;
</div>
