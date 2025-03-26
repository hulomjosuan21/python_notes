| Exception | Description | Example Code |
|-----------|-------------|-------------|
| `ZeroDivisionError` | Raised when dividing by zero | ```python
try:
    result = 10 / 0
except ZeroDivisionError as e:
    print("Cannot divide by zero:", e)
``` |
| `ValueError` | Raised when an operation receives an argument of the right type but inappropriate value | ```python
try:
    num = int("abc")
except ValueError as e:
    print("Invalid literal for int:", e)
``` |
| `IndexError` | Raised when a sequence index is out of range | ```python
try:
    lst = [1, 2, 3]
    print(lst[5])
except IndexError as e:
    print("List index out of range:", e)
``` |
| `KeyError` | Raised when a dictionary key is not found | ```python
try:
    d = {"a": 1}
    print(d["b"])
except KeyError as e:
    print("Key not found in dictionary:", e)
``` |
| `TypeError` | Raised when an operation is performed on an incorrect type | ```python
try:
    result = "text" + 5
except TypeError as e:
    print("Unsupported operand type:", e)
``` |
| `FileNotFoundError` | Raised when a file is not found | ```python
try:
    with open("nonexistent.txt", "r") as f:
        content = f.read()
except FileNotFoundError as e:
    print("File not found:", e)
``` |
| `AttributeError` | Raised when an invalid attribute reference occurs | ```python
try:
    None.some_method()
except AttributeError as e:
    print("Attribute not found:", e)
``` |
| `ImportError` | Raised when an import statement fails | ```python
try:
    import nonexistent_module
except ImportError as e:
    print("Module not found:", e)
``` |
| `NameError` | Raised when a variable is not defined | ```python
try:
    print(undefined_variable)
except NameError as e:
    print("Variable not defined:", e)
``` |
| `PermissionError` | Raised when a file operation lacks necessary permissions | ```python
try:
    with open("protected_file.txt", "w") as f:
        f.write("data")
except PermissionError as e:
    print("Permission denied:", e)
``` |
| `TimeoutError` | Raised when an operation exceeds the given time limit | ```python
import time
try:
    raise TimeoutError("Operation timed out")
except TimeoutError as e:
    print("Timeout occurred:", e)
``` |
| `OverflowError` | Raised when a mathematical operation exceeds the allowable range | ```python
try:
    import math
    print(math.exp(1000))
except OverflowError as e:
    print("Math range error:", e)
``` |
| `RuntimeError` | Raised when an error does not fall into any other category | ```python
try:
    raise RuntimeError("General runtime error")
except RuntimeError as e:
    print("Runtime error occurred:", e)
``` |
