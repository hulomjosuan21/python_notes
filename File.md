## File Manipulation in Python

### Writing to a File
```python
with open("example.txt", "w") as file:
    file.write("Hello, world!\n")
    file.write("This is a test file.\n")
```

### Reading from a File
```python
with open("example.txt", "r") as file:
    content = file.read()
    print(content)
```

### Appending to a File
```python
with open("example.txt", "a") as file:
    file.write("Appending a new line.\n")
```

### Reading a File Line by Line
```python
with open("example.txt", "r") as file:
    for line in file:
        print(line.strip())
```

### Checking if a File Exists
```python
import os
if os.path.exists("example.txt"):
    print("File exists")
else:
    print("File does not exist")
```

### Deleting a File
```python
import os
if os.path.exists("example.txt"):
    os.remove("example.txt")
    print("File deleted")
else:
    print("File does not exist")
```

### Creating a Directory
```python
import os
os.makedirs("new_folder", exist_ok=True)
print("Directory created")
```

### Listing Files in a Directory
```python
import os
files = os.listdir(".")
print("Files in current directory:", files)
```

### Renaming a File
```python
import os
os.rename("example.txt", "renamed_example.txt")
print("File renamed")
