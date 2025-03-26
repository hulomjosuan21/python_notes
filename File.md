## File Manipulation Exception Handling

### FileNotFoundError
```python
with open("nonexistent.txt", "r") as file:
    content = file.read()
```

### PermissionError
```python
with open("/root/protected_file.txt", "w") as file:
    file.write("data")
```

### IsADirectoryError
```python
with open("/home/user/some_directory", "r") as file:
    content = file.read()
```

### NotADirectoryError
```python
import os
os.listdir("some_file.txt")
```

### IOError (OSError)
```python
with open("/dev/full", "w") as file:
    file.write("Test data")
```
