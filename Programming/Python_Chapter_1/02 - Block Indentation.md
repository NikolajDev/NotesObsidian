# Block Indentation (Section 1.3)

Python uses indentation to define control and loop constructs. This contributes to Python's readability, however, it requires the programmer to pay close attention to the use of whitespace.

## The Colon `:` and Indentation
All blocks start with a colon `:` and then contain the indented lines below it.

**Rule of thumb:** Always use 4 spaces for indentation (PEP 8 standard). Do not mix tabs and spaces!

```python
def my_function():
    # This line belongs to the function because it's indented
    a = 2
    return a

# This line is OUTSIDE the function block
print(my_function())

# If statements
a = 10
b = 5
if a > b:
    print("A is greater")
else:
    print("B is greater")
```

## Indentation Errors
If you forget to indent, or mix spaces and tabs, Python will raise an `IndentationError`.

## Console Output
<div style="background: #0c0c0c; color: #00ff41; padding: 20px; font-family: 'Courier New', monospace; border-radius: 8px; border: 1px solid #333;">
$ python indentation.py<br>
2<br>
A is greater
</div>
