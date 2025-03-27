# Python Collection Methods

## List Methods
| Method | Description | Example |
|--------|-------------|---------|
| `append(x)` | Adds an item to the end of the list | `lst.append(5)` |
| `extend(iterable)` | Extends the list by appending elements from the iterable | `lst.extend([6, 7])` |
| `insert(i, x)` | Inserts an item at a given position | `lst.insert(1, 10)` |
| `remove(x)` | Removes the first item from the list with the given value | `lst.remove(5)` |
| `pop([i])` | Removes the item at the given position and returns it | `lst.pop(2)` |
| `clear()` | Removes all items from the list | `lst.clear()` |
| `index(x[, start[, end]])` | Returns the index of the first occurrence of the item | `lst.index(7)` |
| `count(x)` | Returns the number of occurrences of an item | `lst.count(2)` |
| `sort(key=None, reverse=False)` | Sorts the list in place | `lst.sort()` |
| `reverse()` | Reverses the list in place | `lst.reverse()` |
| `copy()` | Returns a shallow copy of the list | `new_lst = lst.copy()` |

## Dictionary Methods
| Method | Description | Example |
|--------|-------------|---------|
| `clear()` | Removes all items from the dictionary | `dct.clear()` |
| `copy()` | Returns a shallow copy of the dictionary | `new_dct = dct.copy()` |
| `fromkeys(iterable, value=None)` | Creates a dictionary from keys with a default value | `dict.fromkeys(['a', 'b'], 0)` |
| `get(key, default=None)` | Returns the value for a key, or default if key is missing | `dct.get('key')` |
| `items()` | Returns a view object with key-value pairs | `dct.items()` |
| `keys()` | Returns a view object with dictionary keys | `dct.keys()` |
| `values()` | Returns a view object with dictionary values | `dct.values()` |
| `pop(key, default=None)` | Removes a key and returns its value | `dct.pop('key')` |
| `popitem()` | Removes and returns the last key-value pair | `dct.popitem()` |
| `setdefault(key, default=None)` | Returns the value of a key, or sets it if missing | `dct.setdefault('key', 0)` |
| `update(iterable)` | Updates dictionary with key-value pairs from another dictionary or iterable | `dct.update({'a': 1})` |

## Set Methods
| Method | Description | Example |
|--------|-------------|---------|
| `add(x)` | Adds an element to the set | `st.add(3)` |
| `clear()` | Removes all elements from the set | `st.clear()` |
| `copy()` | Returns a shallow copy of the set | `new_st = st.copy()` |
| `difference(*sets)` | Returns the difference between sets | `st.difference(st2)` |
| `difference_update(*sets)` | Updates the set with the difference of sets | `st.difference_update(st2)` |
| `discard(x)` | Removes an element if it exists | `st.discard(4)` |
| `intersection(*sets)` | Returns the intersection of sets | `st.intersection(st2)` |
| `intersection_update(*sets)` | Updates the set with the intersection of sets | `st.intersection_update(st2)` |
| `isdisjoint(set)` | Returns `True` if sets have no elements in common | `st.isdisjoint(st2)` |
| `issubset(set)` | Returns `True` if the set is a subset of another | `st.issubset(st2)` |
| `issuperset(set)` | Returns `True` if the set is a superset of another | `st.issuperset(st2)` |
| `pop()` | Removes and returns an arbitrary element | `st.pop()` |
| `remove(x)` | Removes an element, raises an error if not found | `st.remove(3)` |
| `symmetric_difference(set)` | Returns elements that are in one set but not both | `st.symmetric_difference(st2)` |
| `symmetric_difference_update(set)` | Updates the set with symmetric difference | `st.symmetric_difference_update(st2)` |
| `union(*sets)` | Returns the union of multiple sets | `st.union(st2)` |
| `update(*sets)` | Updates the set with the union of sets | `st.update(st2)` |

## Tuple Methods
| Method | Description | Example |
|--------|-------------|---------|
| `count(x)` | Returns the number of occurrences of an item | `tpl.count(3)` |
| `index(x[, start[, end]])` | Returns the index of the first occurrence of the item | `tpl.index(2)` |
