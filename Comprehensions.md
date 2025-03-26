## List Comprehension
```python
arr = [1, 2, 3, 4, 5, 6]
even_list = [i for i in arr if i % 2 == 0]
print(even_list)  # Output: [2, 4, 6]
```

## Dictionary Comprehension
```python
d = {'a': 1, 'b': 5, 'c': 3, 'd': 5}
filtered_dict = {k: v for k, v in d.items() if v != 5}
print(filtered_dict)  # Output: {'a': 1, 'c': 3}
```

## Set Comprehension
```python
arr = [1, 2, 2, 3, 4, 4, 5]
unique_evens = {i for i in arr if i % 2 == 0}
print(unique_evens)  # Output: {2, 4}
```

## Tuple Comprehension (Generator Expression)
```python
arr = (1, 2, 3, 4, 5, 6)
even_gen = (i for i in arr if i % 2 == 0)
print(even_gen)  # Output: <generator object ...>
print(tuple(even_gen))  # Output: (2, 4, 6)
```
