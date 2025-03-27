# Python Collection Methods

## List Methods
| Method | Description |
|--------|-------------|
| `append(x)` | Adds an item to the end of the list |
| `extend(iterable)` | Extends the list by appending elements from the iterable |
| `insert(i, x)` | Inserts an item at a given position |
| `remove(x)` | Removes the first item from the list with the given value |
| `pop([i])` | Removes the item at the given position and returns it |
| `clear()` | Removes all items from the list |
| `index(x[, start[, end]])` | Returns the index of the first occurrence of the item |
| `count(x)` | Returns the number of occurrences of an item |
| `sort(key=None, reverse=False)` | Sorts the list in place |
| `reverse()` | Reverses the list in place |
| `copy()` | Returns a shallow copy of the list |

## Dictionary Methods
| Method | Description |
|--------|-------------|
| `clear()` | Removes all items from the dictionary |
| `copy()` | Returns a shallow copy of the dictionary |
| `fromkeys(iterable, value=None)` | Creates a dictionary from keys with a default value |
| `get(key, default=None)` | Returns the value for a key, or default if key is missing |
| `items()` | Returns a view object with key-value pairs |
| `keys()` | Returns a view object with dictionary keys |
| `values()` | Returns a view object with dictionary values |
| `pop(key, default=None)` | Removes a key and returns its value |
| `popitem()` | Removes and returns the last key-value pair |
| `setdefault(key, default=None)` | Returns the value of a key, or sets it if missing |
| `update(iterable)` | Updates dictionary with key-value pairs from another dictionary or iterable |

## Set Methods
| Method | Description |
|--------|-------------|
| `add(x)` | Adds an element to the set |
| `clear()` | Removes all elements from the set |
| `copy()` | Returns a shallow copy of the set |
| `difference(*sets)` | Returns the difference between sets |
| `difference_update(*sets)` | Updates the set with the difference of sets |
| `discard(x)` | Removes an element if it exists |
| `intersection(*sets)` | Returns the intersection of sets |
| `intersection_update(*sets)` | Updates the set with the intersection of sets |
| `isdisjoint(set)` | Returns `True` if sets have no elements in common |
| `issubset(set)` | Returns `True` if the set is a subset of another |
| `issuperset(set)` | Returns `True` if the set is a superset of another |
| `pop()` | Removes and returns an arbitrary element |
| `remove(x)` | Removes an element, raises an error if not found |
| `symmetric_difference(set)` | Returns elements that are in one set but not both |
| `symmetric_difference_update(set)` | Updates the set with symmetric difference |
| `union(*sets)` | Returns the union of multiple sets |
| `update(*sets)` | Updates the set with the union of sets |

## Tuple Methods
| Method | Description |
|--------|-------------|
| `count(x)` | Returns the number of occurrences of an item |
| `index(x[, start[, end]])` | Returns the index of the first occurrence of the item |
