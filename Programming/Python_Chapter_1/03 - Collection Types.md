# Collection Types (Section 1.5)

While types such as `int` and `str` hold a single value, collection types hold multiple values.

## 1. Lists
An ordered, mutable collection of values.
```python
names = ['Alice', 'Bob', 'Craig']
names[0] = 'Ann'
print(names)
```

## 2. Tuples
Similar to a list, but **immutable** (cannot be changed after creation).
```python
ip_address = ('10.20.30.40', 8080)
# ip_address[0] = '192.168.1.1'  <-- This would raise a TypeError
```

## 3. Dictionaries
A collection of key-value pairs.
```python
state_capitals = {
    'Arkansas': 'Little Rock',
    'Colorado': 'Denver'
}
print(state_capitals['Colorado'])
```

## 4. Sets
An unordered collection of unique elements.
```python
first_names = {'Adam', 'Beth', 'Charlie', 'Adam'}
print(first_names)
```

## Console Output
<div style="background: #0c0c0c; color: #00ff41; padding: 20px; font-family: 'Courier New', monospace; border-radius: 8px; border: 1px solid #333;">
$ python collections.py<br>['Ann', 'Bob', 'Craig']<br>
Denver<br>
{'Beth', 'Adam', 'Charlie'}
</div>
