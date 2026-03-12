# Basic Input and Output (Sections 1.7 & 1.11)

## User Input
To get input from the user, use the `input()` function. Note that `input()` always returns a string (`str`).

```python
name = input("What is your name? ")
print("Hello, " + name)

# For numbers, you must cast the input
age_str = input("Enter your age: ")
age = int(age_str)
```

## String functions: str() vs repr()
There are two functions that can be used to obtain a readable representation of an object.
- `str(x)`: Human-readable string that describes the object.
- `repr(x)`: A representation of `x`. Often contains technical detail.

```python
import datetime
today = datetime.datetime.now()

print(str(today))
print(repr(today))
```

## Console Output
<div style="background: #0c0c0c; color: #00ff41; padding: 20px; font-family: 'Courier New', monospace; border-radius: 8px; border: 1px solid #333;">
$ python io.py<br>
What is your name? Bob<br>
Hello, Bob<br>
2026-03-11 19:34:46.915000<br>
datetime.datetime(2026, 3, 11, 19, 34, 46, 915000)
</div>
