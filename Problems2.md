```python
def is_prime(n):
    if n <= 1:
        return False
    for i in range(2, n):
        if n % i == 0:
            return False
    return True
```

```python
def find_two_medians(lst):
    lst.sort()  # Sort the list first
    mid = len(lst) // 2
    return lst[mid - 1], lst[mid]
```

```python
def iterate_back_and_forth(start, stop):
    num = start
    direction = 1  # 1 for increasing, -1 for decreasing

    for _ in range((stop - start) * 2 + 1):
        print(num, end=" ")

        if num == stop:  # When reaching the stop value, change direction
            direction = -1
        num += direction
```

```python
text = "josuan"

text = text.lower()

isUpper = True

result = ''
for c in text:
    if isUpper:
        result += c.upper()
    else:
        result += c
    
    isUpper = not isUpper

print(result)
```
