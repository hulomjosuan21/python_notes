## Python Exception Handling Table

### ZeroDivisionError
```python
try:
    result = 10 / 0
except ZeroDivisionError as e:
    print("Cannot divide by zero:", e)
```

### ValueError
```python
try:
    num = int("abc")
except ValueError as e:
    print("Invalid literal for int:", e)
```

### IndexError
```python
try:
    lst = [1, 2, 3]
    print(lst[5])
except IndexError as e:
    print("List index out of range:", e)
```

### KeyError
```python
try:
    d = {"a": 1}
    print(d["b"])
except KeyError as e:
    print("Key not found in dictionary:", e)
```

### TypeError
```python
try:
    result = "text" + 5
except TypeError as e:
    print("Unsupported operand type:", e)
```

### FileNotFoundError
```python
try:
    with open("nonexistent.txt", "r") as f:
        content = f.read()
except FileNotFoundError as e:
    print("File not found:", e)
```

### AttributeError
```python
try:
    None.some_method()
except AttributeError as e:
    print("Attribute not found:", e)
```

### ImportError
```python
try:
    import nonexistent_module
except ImportError as e:
    print("Module not found:", e)
```

### NameError
```python
try:
    print(undefined_variable)
except NameError as e:
    print("Variable not defined:", e)
```

### PermissionError
```python
try:
    with open("protected_file.txt", "w") as f:
        f.write("data")
except PermissionError as e:
    print("Permission denied:", e)
```

### TimeoutError
```python
import time
try:
    raise TimeoutError("Operation timed out")
except TimeoutError as e:
    print("Timeout occurred:", e)
```

### OverflowError
```python
try:
    import math
    print(math.exp(1000))
except OverflowError as e:
    print("Math range error:", e)
```

### RuntimeError
```python
try:
    raise RuntimeError("General runtime error")
except RuntimeError as e:
    print("Runtime error occurred:", e)
