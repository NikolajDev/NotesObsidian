# Built-in Modules and Pip (Sections 1.8, 1.9, 1.12)

A module is a file containing Python definitions and statements. 

## Using Built-in Modules
You can import modules using the `import` statement.

```python
import math
import random

print(math.sqrt(16))
print(random.randint(1, 10))
```

## Package Management (PIP)
`pip` is your friend when you need to install any package from the Python Package Index (PyPI). 

Common terminal commands:
- **Search:** `pip search <query>`
- **Install:** `pip install <package_name>`
- **Upgrade:** `pip install <package_name> --upgrade`
- **List installed:** `pip list`

## Console Output
<div style="background: #0c0c0c; color: #00ff41; padding: 20px; font-family: 'Courier New', monospace; border-radius: 8px; border: 1px solid #333;">
$ python modules.py<br>
4.0<br>
7<br>
<br>
$ pip install requests<br>
Collecting requests<br>
Successfully installed requests-2.28.1
</div>
