## List Comprehension
```python
arr = [1, 2, 3, 4, 5, 6]
even_list = [i for i in arr if i % 2 == 0]
print(even_list)  # Output: [2, 4, 6]

arr = [1, 2, 3, 4, 5, 6]
even_or_odd = ["Even" if i % 2 == 0 else "Odd" for i in arr]
print(even_or_odd)  # Output: ['Odd', 'Even', 'Odd', 'Even', 'Odd', 'Even']
```

## Dictionary Comprehension
```python
d = {'a': 1, 'b': 5, 'c': 3, 'd': 5}
filtered_dict = {k: v for k, v in d.items() if v != 5}
print(filtered_dict)  # Output: {'a': 1, 'c': 3}

d = {'a': 1, 'b': 5, 'c': 3, 'd': 6}
modified_dict = {k: ("High" if v > 3 else "Low") for k, v in d.items()}
print(modified_dict)  # Output: {'a': 'Low', 'b': 'High', 'c': 'Low', 'd': 'High'}
```

## Set Comprehension
```python
arr = [1, 2, 2, 3, 4, 4, 5]
unique_evens = {i for i in arr if i % 2 == 0}
print(unique_evens)  # Output: {2, 4}

arr = [1, 2, 2, 3, 4, 4, 5]
processed_set = {i if i % 2 == 0 else i * 10 for i in arr}
print(processed_set)  # Output: {2, 4, 10, 30, 50}
```

## Tuple Comprehension (Generator Expression)
```python
arr = (1, 2, 3, 4, 5, 6)
even_gen = (i for i in arr if i % 2 == 0)
print(even_gen)  # Output: <generator object ...>
print(tuple(even_gen))  # Output: (2, 4, 6)

arr = (1, 2, 3, 4, 5, 6)
processed_tuple = tuple(i if i % 2 == 0 else i * 10 for i in arr)
print(processed_tuple)  # Output: (10, 2, 30, 4, 50, 6)
```
